# <a name="settingstatedevicesummary-resource-type"></a>Тип ресурса settingStateDeviceSummary

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Сводка по состоянию параметра конфигурации и политики соответствия требованиям для устройств
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов settingStateDeviceSummary](../api/intune_deviceconfig_settingstatedevicesummary_list.md)|Коллекция [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Список свойств и связей объектов [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).|
|[Получение объекта settingStateDeviceSummary](../api/intune_deviceconfig_settingstatedevicesummary_get.md)|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Чтение свойств и связей объекта [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).|
|[Создание объекта settingStateDeviceSummary](../api/intune_deviceconfig_settingstatedevicesummary_create.md)|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Создание объекта [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).|
|[Удаление объекта settingStateDeviceSummary](../api/intune_deviceconfig_settingstatedevicesummary_delete.md)|Нет|Удаляет объект [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).|
|[Обновление объекта settingStateDeviceSummary](../api/intune_deviceconfig_settingstatedevicesummary_update.md)|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Обновление свойств объекта [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String (строка)|Ключ объекта.|
|settingName|String (строка)|Имя параметра.|
|instancePath|String (строка)|Имя пути к экземпляру для параметра.|
|unknownDeviceCount|Int32|Количество неизвестных устройств для параметра.|
|notApplicableDeviceCount|Int32|Количество неприменимых устройств для параметра.|
|compliantDeviceCount|Int32|Количество соответствующих устройств для параметра.|
|remediatedDeviceCount|Int32|Количество соответствующих устройств для параметра.|
|nonCompliantDeviceCount|Int32|Количество несоответствующих устройств для параметра.|
|errorDeviceCount|Int32|Количество ошибок устройств для параметра.|
|conflictDeviceCount|Int32|Количество конфликтов устройств для параметра|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.settingStateDeviceSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "String (identifier)",
  "settingName": "String",
  "instancePath": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```








