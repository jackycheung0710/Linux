### ESXI

#### VMware vSphere 7.0新特性

- vSphere Lifecycle Manager：新一代基础架构镜像管理器，使用预期状态模型修补、更新或升级ESXI集群
- vCenter Server Profile：用于vCenter Server预期状态配置管理功能，帮助用户为多个vCenter Server定义、验证、应用配置。
- vCenter Server Update Planner：针对升级场景管理vCenter的兼容性和互操作性，能够生成互操作性和预检查报告，帮助用户针对升级进行规划
- 内容库：管理控制和版本控制功能，支持简单有效地击中管理虚拟机模板、虚拟设备、ISO镜像和脚本。
- 借助ADFS实施联合身份验证：保护访问和客户安全
- vSphere Trust Authority：用于敏感工作负载进行远程认证
- Dynamic DirectPath IO：用于支持vGPU和DirectPath I/O初始虚拟机。
- DRS：重新设计的DRS采用以工作负载为中心的方法，可以平衡分配资源给集群
- vMotion：无关虚拟机的大小，vMotion都能提供无中断操作，这对大型负载和关键应用负载非常有用
- vSphere 7.0 with Kubernetes：基于VMware Cloud Foundation服务，通过Kubernetes API为开发人员提供实时基础架构访问权限。
  - VMware Cloud Foundation Services
  - Tanzu Runtime Services
  - Hybrid Infrastructure Services
  - Tanzu Kubernetes Grid服务
  - vSphere pod服务
  - 存储卷服务
  - 网络服务
  - 镜像仓库服务

#### VMware ESXI系统硬件要求

- 处理器
- 内存
- 网卡
- 存储适配器
- 硬盘

### vCenter Server

利用vCenter Server，可以集中管理多个ESXI主机及其虚拟机。

在VMware vSphere架构中，可以在ESXI主机上部署vCenter Server Appliance（VCSA）。VCSA可以实现多个高级功能，如DRS、HA、Fault Tolerance、vMotion和Storage vMotion。

#### vCenter Server架构

- vSphere Client：使用客户端连接vCenter Server，可以集中管理ESXI主机
- vCenter Server数据库：vCenter Server数据库是vCenter Server最重要组件。数据库用于存储vCenter Server清单项、安全角色、资源池、性能数据及其重要信息。
- 托管主机：可以使用vCenter Server管理ESXI主机和在这些主机上运行的虚拟机。

#### SSO

vCenter Single Sign On（SSO），本质上是一个在vSphere应用和Authentication源之间的一个安全交互组件。它通过AD或Open LDAP之类的Identity Sources的通信来实现Authentication。

#### 增强型链接模式

对于中小企业来说，通常部署一个vCenter Server用于管理生产环境中的ESXI主机及虚拟机。一个vCenter Server可以管理大量的设备，但对于一些大型企业或者特殊应用来说，一个vCenter Server无法满足其需求，如果单独部署多个vCenter Server，因为不能统一管理又给管理带来很多问题，VMware vSphere提供了增强型链接模式来解决这个问题。通过增强型连接模式，用户登录任意一个vCenter Server就可以查看和管理所有vCenter Server。

vCenter Server 7.0的增强型链接模式新增功能：

- 无须外部Platform Services Controller支持，简化了部署
- 简化的备份和还原过程，不需负载均衡器
- 最多可将15个vCenter Server链接到一起，并在一个清单视图中显示。
- 对于vCenter HA集群，三个节点视为一个逻辑vCenter Server节点。一个vCenter HA集群需要一个vCenter Server标准许可证。

#### vCenter Server管理后台

端口：5480

vCenter Server管理后台内置有备份功能，通过日常的备份，可以快速重新部署vCenter Server。vCenter内置的备份并不是完整的虚拟机备份，仅备份了vCenter的数据库、配置等信息，通过这些信息重新部署vCenter Server。

### 创建和使用虚拟机

#### 虚拟机

虚拟机与物理机一样，都是运行操作系统和应用程序的计算机。虚拟机包含一组规范和配置文件，并由主机的物理资源提供支持。每个虚拟机都具有一些虚拟设备，这些设备可提供与物理硬件相同的功能，并且可移植性强、更安全且更易于管理。虚拟机包含若干文件（配置、虚拟磁盘、NVRAM设备和日志文件），这些文件存储在存储设备上。

#### 虚拟机组成

- 配置文件：虚拟机名称.vmx。记录了操作系统版本、内存大小、硬盘类型及大小、虚拟网卡MAC地址等信息。
- 交换文件：虚拟机名称.vswp。类似于Windows系统的页面文件，主要用于虚拟机开关机时进行内存交换。
- BIOS文件：虚拟机名称.nvram。为了与物理服务器相同，用于产生虚拟机的BIOS。
- 日志文件：vmware.log。它是虚拟机的日志文件。
- 硬盘描述文件：虚拟机名称.vmdk。它是虚拟硬盘的描述文件，与虚拟硬盘有差别
- 硬盘数据文件：虚拟机名称.flat.vmdk。它是虚拟机使用的虚拟硬盘，实际所使用的虚拟硬盘的容量就是此文件的大小。
- 挂起状态文件：虚拟机名称.vmss。它是虚拟机进入挂起状态时产生的文件
- 快照数据文件：虚拟机名称.vmsn。如果虚拟机快照包含内存状态，就会产生此文件。
- 快照硬盘文件：虚拟机名称.delta.vmdk。使用快照时，源.vmdk文件会保持源状态同时产生delta.vmdk文件，所有的操作都是在.delta.vmdk文件上进行。
- 模板文件：虚拟机名称.vmtx。它是虚拟机创建模板后产生的文件。

#### 虚拟机硬件

创建虚拟机时必须配置相对应的硬件资源。VMware vSphere7.0虚拟机使用发布的虚拟机硬件17版。

#### 虚拟机硬件资源支持

1、VMware vSphere7.0与其他版本支持的虚拟机硬件资源对比

| 最大支持    | VMware vSphere版本 |      |      |      |
| ----------- | ------------------ | ---- | ---- | ---- |
|             | 6.0                | 6.5  | 6.7  | 7.0  |
| vCPU per VM | 128                | 128  | 128  | 256  |
| vRAM per VM | 4TB                | 6TB  | 6TB  | 6TB  |

2、ESXI主机与各个版本的虚拟机硬件兼容性

| ESXi版本           | 虚拟机硬件版本 |
| ------------------ | -------------- |
| VMware ESXi 7.0    | 17             |
| VMware ESXi 6.7 U2 | 16             |
| VMware ESXi 6.7    | 14             |
| VMware ESXi 6.5    | 12、13         |
| VMware ESXi 6.0    | 11             |
| VMware ESXi 5.5    | 10             |
| VMware ESXi 5.1    | 9              |
| VMware ESXi 5.0    | 8              |
| VMware ESXi 4.X    | 7              |

3、ESXi主机及虚拟机支持的存储适配器

​      ESXi支持不同类别的适配器，包括SCSI、iSCSI、RAID、光纤通道、以太网光纤通道（Fibre Channel over Ethernet，FCoE）和以太网。

4、虚拟机磁盘类型

- Thick Provision Lazy Zeroed：厚置备延迟置零。创建虚拟机磁盘时的默认类型，所有空间都被分配，但是源来在磁盘上写入的数据不被删除。存储空间中的现有数据不被删除而是留在物理磁盘上，擦除数据和格式化只在第一次写入磁盘时进行，这会降低性能。阵列集成存储API（vStorage API for Array Integration，vAAI）的块置零特性极大地减轻了这种性能降低的现象。
- Thick Provision Eager Zeroed：厚置备置零。所有磁盘空间被保留，数据完全从磁盘上删除，磁盘创建时进行格式化，创建这样的磁盘花费时间比延迟置零长，但增强了安全性，同时，写入磁盘性能要比延迟置零好。
- Thin Privision：精简置备。使用此类型，.vmdk文件不会一开始就全部使用，而是随数据的增加而增加，例如，虚拟机设置了40GB虚拟磁盘空间，安装操作系统使用了10GB空间，那么.vmdk文件大小应该是10G，而不是40GB，好处是节省了磁盘空间。可以通过UNMAP命令对未使用空间进行回收操作。

5、虚拟机磁盘模式

- Independent Persistent：独立持久。虚拟机的所有硬盘读写都写入.vmdk文件中，这中模式提供最佳性能。
- Independent Nonpersistent：独立非持久。虚拟机启动后进行的所有修改被写入一个文件，此模式的性能不是很好。

6、虚拟网络适配器

对于虚拟机使用的网络适配器，ESXi7.0推荐使用VMXNET3。

- E1000E：Intel 82574L以太网网卡的仿真版本。是Windows8和Windows Server 2012的默认适配器。
- E1000：Intel 82545EM以太网网卡的仿真版本。
- Vlance：AMD 79C970 PCnet32 LANCE网卡的仿真版本。
- VMXNET2（增强型）：基于VMXNET适配器，只适用于ESXI3.5及更高版本客户机操作系统，不支持ESXI6.7及更高版本。
- VMXNET3：专为提高性能而设计的半虚拟化网卡。可提供VMXNET2中的所有可用功能并新增几种功能，如多队列支持、IPv6卸载和MSI/MSI-X中断传递。
- SR-IOV直通
- vSphere DirectPath I/O：允许虚拟机上的客户机操作系统直接访问连接到主机的物理PCI和PCIe设备。直通设备能够高效利用资源和提高性能。可以使用vSphere Client在虚拟机上配置直通PCI设备。
- PVRDMA：允许多个客户机通过使用行业标准结构Verbs API来访问RDMA设备，应用可使用PVRDMA客户机驱动程序与底层物理设备通信。

#### 安装VMware Tools

虚拟机安装操作系统后已经可以使用，但由于其特殊性，只有在安装了VMware Tools后，许多VMware功能才可以被使用。如果虚拟机中未安装VMware Tools，则不能使用工具栏中的关机或者重新启动选项，只能使用电源选项。同时VMware Tools针对虚拟硬件使用专用驱动程序替换了通用驱动程序，该进了虚拟机管理。

CentOS 7版本或其他新版本Linux系统在安装过程中会检测系统是否是虚拟化平台，如果是虚拟化平台，会自动安装open-vm-tools。精简版Linux可能不会自动安装，需要手动进行安装。

```shell
# 卸载非VMware官方vm-tools
yum remove open-vm-tools
# 挂载安装VMware Tools
mount -t iso9660 /dev/cdrom /mnt/cdrom
cp /mnt/cdrom/VMwareTools-10.3.21-14772444.tar.gz /tmp
# tar 解压
# 进入VMwareTools
cd vmware-tools-distrib/
./vmware-install.pl
```

#### 虚拟机模板

Virtual Machine Template，使用虚拟机模板可以在企业环境中大量快速部署虚拟机，并且不容易出现错误。模板是虚拟机的副本，可用于创建和调配新的虚拟机。

#### 克隆虚拟机

​	克隆虚拟机是通过复制源虚拟机的方式创建一台新的虚拟机，新的虚拟机是原有虚拟机的精确副本，在克隆过程中，虚拟机可以是开启或关闭状态。如果要克隆的虚拟机处于开启状态，则克隆虚拟机时，服务和应用不会自动进入静默状态。

- 虚拟机模板会占用存储空间，因此必须相应地规划存储空间。
- 使用模板部署虚拟机比克隆正在运行的虚拟机更快，特别是在第一次部署多个虚拟机的情况下。
- 当使用模板部署多台虚拟机时，所有虚拟机都以相同的基础镜像作为起点，从正在运行的虚拟机克隆虚拟机可能不会创建完全相同的虚拟机，具体取决于克隆虚拟机时，该虚拟机中进行的活动。
- 同时部署具有相同客户机操作系统设置的虚拟机和克隆虚拟机时可能会发生冲突，使用客户机操作系统进行自定义即可避免该问题。

1、创建虚拟机定义规范

​	从VMware vSphere7开始，自定义规范只能自定义网络设置，如IP地址、DNS服务器及网关，无须关闭或重启虚拟机即可更改这些设置。

2、即时克隆操作

​	即时克隆虚拟机时，源虚拟机不会因为克隆过程而丢失其状态。鉴于这种操作的速度和状态保持特性，可以转为即时调配。在即时克隆操作期间，源虚拟机将`昏迷`片刻（少于1秒）。当源虚拟机昏迷时，系统将为每个虚拟磁盘生成一个新的可写增量磁盘，同时选取一个检查点将其传输到目标虚拟机，目标虚拟机将使用源虚拟机的检查点启动，目标虚拟机完全启动后，源虚拟机也将恢复运行。即时克隆的虚拟机是完全独立的vCenter Server清单对象，可以想管理常规虚拟机那样管理即时克隆虚拟机，没有任何限制。

​	对于大规模应用部署，即时克隆非常方便，它能确保内存效率，可以在单个主机上创建大量虚拟机。避免网络冲突，可以在执行即时克隆操作期间自定义目标虚拟机的虚拟硬件。例如，可以自定义目标虚拟机的虚拟网卡的MAC地址或者串行和并行端口配置。

#### 内容库

内容库是由OVF模板和其他文件组成的存储库，这些模板和文件可以在不同的vCenter Server之间进行共享和同步。借助内容库，运维人员可以将OVF模板、ISO镜像或其他文件类型存储在一个中心位置上，可以发布这些模板、镜像和文件，并且其他内容库可以订阅和下载这些内容。













