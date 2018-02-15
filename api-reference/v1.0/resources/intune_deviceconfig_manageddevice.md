# <a name="manageddevice-resource-type"></a>Тип ресурса managedDevice

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Устройства, которые управляются или предварительно регистрируются с помощью Intune
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов managedDevice](../api/intune_deviceconfig_manageddevice_list.md)|Коллекция [managedDevice](../resources/intune_deviceconfig_manageddevice.md)|Список свойств и связей объектов [managedDevice](../resources/intune_deviceconfig_manageddevice.md).|
|[Получение объекта managedDevice](../api/intune_deviceconfig_manageddevice_get.md)|[managedDevice](../resources/intune_deviceconfig_manageddevice.md)|Чтение свойств и связей объекта [managedDevice](../resources/intune_deviceconfig_manageddevice.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Н/Д|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|deviceConfigurationStates|Коллекция [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)|Состояния конфигурации этого устройства.|
|deviceCompliancePolicyStates|Коллекция [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)|Состояния политики соответствия требованиям для этого устройства.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)"
}
```



