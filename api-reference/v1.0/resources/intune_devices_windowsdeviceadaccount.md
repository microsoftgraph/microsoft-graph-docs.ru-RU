# <a name="windowsdeviceadaccount-resource-type"></a>Тип ресурса windowsDeviceADAccount

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Н/Д

Наследуется от [windowsDeviceAccount](../resources/intune_devices_windowsdeviceaccount.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|password|String|Н/Д. Наследуется от [windowsDeviceAccount](../resources/intune_devices_windowsdeviceaccount.md)|
|domainName|String|Н/Д|
|userName|String|Н/Д|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.windowsDeviceAccount",
  "@odata.type": "microsoft.graph.windowsDeviceADAccount"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDeviceADAccount",
  "password": "String",
  "domainName": "String",
  "userName": "String"
}
```



