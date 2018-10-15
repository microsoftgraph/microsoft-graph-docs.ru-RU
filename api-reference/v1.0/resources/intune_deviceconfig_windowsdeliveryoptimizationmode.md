# <a name="windowsdeliveryoptimizationmode-enum-type"></a>Тип перечисления windowsDeliveryOptimizationMode

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Режим оптимизации доставки для распределения кэширующих узлов
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Разрешить пользователю задать настройку.|
|httpOnly|1|только HTTP, не пиринг|
|httpWithPeeringNat|2|Операционная система по умолчанию — Http, смешанные пирингом, вне переводчика того же сетевого адреса|
|httpWithPeeringPrivateGroup|3|HTTP смешанные с пирингом в частной группе|
|httpWithInternetPeering|4|HTTP смешанные пирингом Интернета|
|simpleDownload|99|Режим простой загрузки без пиринга|
|bypassMode|100|Режим обхода. Не используйте Оптимизацию доставки и вместо нее используйте BITS|








