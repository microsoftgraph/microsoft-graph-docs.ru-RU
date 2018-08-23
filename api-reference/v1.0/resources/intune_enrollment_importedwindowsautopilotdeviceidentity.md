# <a name="importedwindowsautopilotdeviceidentity-resource-type"></a>Тип ресурса importedWindowsAutopilotDeviceIdentity

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Импортированные устройства с Windows AutoPilot
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список importedWindowsAutopilotDeviceIdentities](../api/intune_enrollment_importedwindowsautopilotdeviceidentity_list.md)|Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)|Список свойств и связей между объектами[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).|
|[Получение importedWindowsAutopilotDeviceIdentity](../api/intune_enrollment_importedwindowsautopilotdeviceidentity_get.md)|[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)|Чтение свойств и связей между объектами[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).|
|[Создание importedWindowsAutopilotDeviceIdentity](../api/intune_enrollment_importedwindowsautopilotdeviceidentity_create.md)|[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)|Создание нового объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).|
|[Удаление importedWindowsAutopilotDeviceIdentity](../api/intune_enrollment_importedwindowsautopilotdeviceidentity_delete.md)|Отсутствует|Удаляет [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).|
|[Обновление importedWindowsAutopilotDeviceIdentity](../api/intune_enrollment_importedwindowsautopilotdeviceidentity_update.md)|[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)|Обновляет свойства объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|GUID объекта|
|orderIdentifier|Строка|Номер заказа устройства Windows Autopilot.|
|serialNumber|Строка|Серийный номер устройства Windows Autopilot.|
|productKey|Строка|Ключ продукта устройства Windows Autopilot.|
|hardwareIdentifier|Двоичный|Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.|
|state|[importedWindowsAutopilotDeviceIdentityState](../resources/intune_enrollment_importedwindowsautopilotdeviceidentitystate.md)|Текущее состояние импортированного устройства.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "String (identifier)",
  "orderIdentifier": "String",
  "serialNumber": "String",
  "productKey": "String",
  "hardwareIdentifier": "binary",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "String",
    "deviceRegistrationId": "String",
    "deviceErrorCode": 1024,
    "deviceErrorName": "String"
  }
}
```



