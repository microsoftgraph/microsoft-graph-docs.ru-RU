# <a name="manageddevicemobileappconfigurationdevicestatus-resource-type"></a>Тип ресурса managedDeviceMobileAppConfigurationDeviceStatus

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства, наследуемые свойства и действия для MDM состояние конфигурации мобильного приложения для устройства.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список managedDeviceMobileAppConfigurationDeviceStatuses](../api/intune_apps_manageddevicemobileappconfigurationdevicestatus_list.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) коллекции|Свойства списка и связей объектов [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) .|
|[Получение managedDeviceMobileAppConfigurationDeviceStatus](../api/intune_apps_manageddevicemobileappconfigurationdevicestatus_get.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)|Чтение свойства и связи объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) .|
|[Создание managedDeviceMobileAppConfigurationDeviceStatus](../api/intune_apps_manageddevicemobileappconfigurationdevicestatus_create.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)|Создание нового объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) .|
|[Удаление managedDeviceMobileAppConfigurationDeviceStatus](../api/intune_apps_manageddevicemobileappconfigurationdevicestatus_delete.md)|Отсутствует|Удаляет [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md).|
|[Обновление managedDeviceMobileAppConfigurationDeviceStatus](../api/intune_apps_manageddevicemobileappconfigurationdevicestatus_update.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)|Обновление свойства объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|deviceDisplayName|String|Имя устройства в объекте DevicePolicyStatus.|
|userName|String|Имя пользователя в отчете.|
|deviceModel|String|Модель устройства в отчете.|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Дата и время, когда истекает период отсрочки применения политик на устройстве.|
|status|[complianceStatus](../resources/intune_shared_compliancestatus.md)|Состояние соответствия требованиям для отчета о политике. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Дата и время последнего изменения отчета о политике.|
|userPrincipalName|String|Имя участника-пользователя.|

## <a name="relationships"></a>Связи
None
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



