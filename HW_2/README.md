
OSPF-маршрутизация
============

В схеме **CLOS** собраны 2 `Spine` и 3 `Leaf` коммутатора.

![Схема](CLOS.png "CLOS-топология")


На каждом устройстве настроен OSPF:  `Area` **0.0.0.0**, `Instance` **100**, `RouterID` назначен идентичный IP-адресу **Loopback интерфейса**, `passive-interface` **default**, Loopback-интерфесы добавлены в `Area` **0.0.0.0**
![OSPF](OSPF.png "OSPF-маршрутизация")



На `Spine`-коммутаторах на **ETHERNET[1-3]**: **отключен** `passive-interface`, добавлена `Area` **0.0.0.0**, `network` **point-to-point** 
На `Leaf`-коммутаторах на **ETHERNET[1-3]**: **отключен** `passive-interface`, добавлена `Area` **0.0.0.0**, `network` **point-to-point** 
