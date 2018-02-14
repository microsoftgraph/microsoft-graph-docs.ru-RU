# <a name="manageddevicemobileappconfigurationassignment-resource-type"></a>Тип ресурса managedDeviceMobileAppConfigurationAssignment

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства, используемые для назначения конфигурации приложения MDM группе.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список managedDeviceMobileAppConfigurationAssignments](../api/intune_apps_manageddevicemobileappconfigurationassignment_list.md)|Коллекция [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)|Перечисление свойств и связей объектов [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).|
|[Получение managedDeviceMobileAppConfigurationAssignment](../api/intune_apps_manageddevicemobileappconfigurationassignment_get.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)|Считывание свойств и связей объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).|
|[Создание managedDeviceMobileAppConfigurationAssignment](../api/intune_apps_manageddevicemobileappconfigurationassignment_create.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)|Создание объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).|
|[Удаление managedDeviceMobileAppConfigurationAssignment](../api/intune_apps_manageddevicemobileappconfigurationassignment_delete.md)|Отсутствует|Удаление [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).|
|[Обновление managedDeviceMobileAppConfigurationAssignment](../api/intune_apps_manageddevicemobileappconfigurationassignment_update.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)|Обновление свойств объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_apps_deviceandappmanagementassignmenttarget.md)|Объект, для которого назначается политика соблюдения условий.|

## <a name="relationships"></a>Связи
Отсутствуют
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



