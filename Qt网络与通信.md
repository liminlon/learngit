# 获取本机网络信息
* **QString localHosName=QHostInfo::localHostName()** 获取本机主机名<br/>
* **QHostInfo hostInfo=QHostInfo::fromName(localHostName)** 通过主机名查找IP地址信息<br/>
* **QList<QHostAddress> listAddress=hostInfo.addresses()** 获取主机的IP地址列表<br/>
* **QList<QNetworkInterface> list=QNetworkInterface::allInterfaces()** QNetworkInterface类提供了一个主机IP地址和网络接口列表<br/>
* **interface.name()** 获取网络接口的名称<br/>
* **interface.hardwareAddress()** 获取网络接口的硬件地址<br/>
* **interface.addressEntries()** 每个网络接口包括0个或多个IP地址，每个IP地址与一个子网掩码和（或）一个广播地址相关联。QNetworkAddressEntry类存储了被网络接口支持的一个IP地址，同时还包括与之相关的子网掩码和广播地址。<br/>