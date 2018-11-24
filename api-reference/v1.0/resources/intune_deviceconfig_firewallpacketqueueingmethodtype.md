# <a name="firewallpacketqueueingmethodtype-enum-type"></a>Тип перечисления firewallPacketQueueingMethodType

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения для firewallPacketQueueingMethod
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|deviceDefault|0|Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию|
|Этот параметр отключен|1|Отключение очереди пакетов|
|queueInbound|2|В очередь входящие зашифрованные пакеты|
|queueOutbound|3|Очередь расшифрован исходящих пакетов для пересылки|
|queueBoth|4|Очередь входящих и исходящих пакетов|



