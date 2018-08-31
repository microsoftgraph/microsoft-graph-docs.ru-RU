# <a name="locatedeviceactionresult-resource-type"></a>Тип ресурса locateDeviceActionResult

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Результат действия "Поиск устройства"

Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actionName|Строка|Название действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)|
|actionState|[actionState](../resources/intune_devices_actionstate.md)|Состояние действия унаследованного от [deviceActionResult](../resources/intune_devices_deviceactionresult.md). Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|startDateTime|DateTimeOffset|Время начала действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)|
|lastUpdatedDateTime|DateTimeOffset|Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)|
|deviceLocation|[deviceGeoLocation](../resources/intune_devices_devicegeolocation.md)|Местоположение устройства|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceActionResult",
  "@odata.type": "microsoft.graph.locateDeviceActionResult"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.locateDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "deviceLocation": {"@odata.type": "microsoft.graph.deviceGeoLocation"}
}
```



