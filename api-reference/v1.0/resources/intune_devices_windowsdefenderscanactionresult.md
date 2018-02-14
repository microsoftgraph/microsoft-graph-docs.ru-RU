# <a name="windowsdefenderscanactionresult-resource-type"></a>Тип ресурса windowsDefenderScanActionResult

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Результат последнего сканирования, выполненного Защитником Windows

Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actionName|String|Название действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md).|
|actionState|String|Состояние действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md). Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|startDateTime|DateTimeOffset|Время начала действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md).|
|lastUpdatedDateTime|DateTimeOffset|Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md).|
|scanType|String|Тип сканирования (полное или краткое).|

## <a name="relationships"></a>Связи
Отсутствуют
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderScanActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "scanType": "String"
}
```



