# <a name="manageddeviceoverview-resource-type"></a>Тип ресурса managedDeviceOverview

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Сводные данные для управляемых устройств
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта managedDeviceOverview](../api/intune_devices_manageddeviceoverview_get.md)|[managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md)|Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md).|
|[Обновление объекта managedDeviceOverview](../api/intune_devices_manageddeviceoverview_update.md)|[managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md)|Обновление свойств объекта [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String (строка)|Уникальный идентификатор сводки.|
|enrolledDeviceCount|Int32|Общее количество зарегистрированных устройств. Не включает устройства ПК, которыми управляет агент Intune для ПК.|
|mdmEnrolledCount|Int32|Количество устройств, зарегистрированных в MDM.|
|dualEnrolledDeviceCount|Int32|Количество устройств, зарегистрированных как в MDM, так и в EAS.|
|deviceOperatingSystemSummary|[deviceOperatingSystemSummary](../resources/intune_devices_deviceoperatingsystemsummary.md)|Общие сведения об операционной системе устройства.|
|deviceExchangeAccessStateSummary|[deviceExchangeAccessStateSummary](../resources/intune_devices_deviceexchangeaccessstatesummary.md)|Распределение состояния доступа Exchange Access State в Intune|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceOverview"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "String (identifier)",
  "enrolledDeviceCount": 1024,
  "mdmEnrolledCount": 1024,
  "dualEnrolledDeviceCount": 1024,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 1024,
    "iosCount": 1024,
    "macOSCount": 1024,
    "windowsMobileCount": 1024,
    "windowsCount": 1024,
    "unknownCount": 1024
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 1024,
    "blockedDeviceCount": 1024,
    "quarantinedDeviceCount": 1024,
    "unknownDeviceCount": 1024,
    "unavailableDeviceCount": 1024
  }
}
```








