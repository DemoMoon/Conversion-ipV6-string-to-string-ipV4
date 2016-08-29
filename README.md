# Conversion-ipV6-string-to-string-ipV4
Conversion ipV6 string to string ipV4

DNS64

DNS64说白了是用来帮助host获取IPv6地址的，传统的DNS服务器可以把域名转换成IPv4地址，但我们的iPhone设备如果处于IPv6环境下，只能去获取IPv6的地址。
DNS64就像一个中间代理，把传统服务器返回的IPv4地址通过特殊的映射方式转换成一个看着像IPv6地址的地址（IPv4的核，IPv6的壳），
转换其实很简单，用公式可以这样表达：

64:ff9b::IPv4 = IPv6

NAT64

DNS64帮助拿到IPv6的地址后，接下来就是NAT64登场，帮助IPv6的Packet顺利接入IPv4的公网当中。IPv4的公网环境路由器只认识IPv4的地址，所有这里当然也需要一个中间设备来做协议转换。NAT64就扮演这个角色。

