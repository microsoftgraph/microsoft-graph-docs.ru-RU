# <a name="devicemanagement-resource-type"></a>Тип ресурса deviceManagement

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Ресурс deviceManagement представляет идентификаторы устройств из коллекции клиента, которые были предварительно подготовлены в Intune, и профили регистрации, которые можно назначать идентификаторам устройств, поддерживающим конфигурацию до регистрации.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceManagement](../api/intune_enrollment_devicemanagement_get.md)|[deviceManagement](../resources/intune_enrollment_devicemanagement.md)|Чтение свойств и связей объекта [deviceManagement](../resources/intune_enrollment_devicemanagement.md).|
|[Обновление объекта deviceManagement](../api/intune_enrollment_devicemanagement_update.md)|[deviceManagement](../resources/intune_enrollment_devicemanagement.md)|Обновление свойств объекта [deviceManagement](../resources/intune_enrollment_devicemanagement.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID объекта.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|importedWindowsAutopilotDeviceIdentities|Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)|Коллекция импортированных устройств Windows AutoPilot.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



