# <a name="iosmobileappconfiguration-resource-type"></a>тип ресурса iosMobileAppConfiguration

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства, унаследованные свойства и действия для конфигураций мобильного приложения для iOS.

Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список iosMobileAppConfigurations](../api/intune_apps_iosmobileappconfiguration_list.md)|коллекция [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md)|Список свойств и связей объектов [iosUpdateConfiguration](../resources/intune_apps_iosmobileappconfiguration.md).|
|[Получить iosMobileAppConfiguration](../api/intune_apps_iosmobileappconfiguration_get.md)|[iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md)|Считывание свойств и связей объекта [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md).|
|[Создать iosMobileAppConfiguration](../api/intune_apps_iosmobileappconfiguration_create.md)|[iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md)|Создание нового объекта [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md).|
|[Удалить iosMobileAppConfiguration](../api/intune_apps_iosmobileappconfiguration_delete.md)|Отсутствует|Удаляет [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md).|
|[Обновить iosMobileAppConfiguration](../api/intune_apps_iosmobileappconfiguration_update.md)|[iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md)|Обновление свойств объекта [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String (строка)|Ключ объекта. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md);|
|targetedMobileApps|Коллекция String|приложение-обработчик Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md);|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md);|
|описание|String (строка)|Администратор предоставил описание конфигурация устройства. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md);|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md);|
|displayName|String (строка)|Администратор предоставил название конфигурации устройства. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md);|
|версия|Int32|Версия конфигурации устройства. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md);|
|encodedSettingXml|Двоичный|конфигурация приложения службы управления мобильными устройствами двоичная Base64.|
|параметры|коллекция [appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md)|элементы параметра конфигурации приложения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)|Список заданий группы для настройки приложения. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)|
|deviceStatuses|Коллекция [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)|Список ManagedDeviceMobileAppConfigurationDeviceStatus. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)|
|userStatuses|Коллекция [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md)|Список объектов ManagedDeviceMobileAppConfigurationUserStatus. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md);|
|deviceStatusSummary|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|Общие сведения о состоянии устройства, связанном с настройкой приложения. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md);|
|userStatusSummary|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|Общие сведения о состоянии пользователя, связанном с настройкой приложения. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md);|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedDeviceMobileAppConfiguration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosMobileAppConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "encodedSettingXml": "binary",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "String",
      "appConfigKeyType": "String",
      "appConfigKeyValue": "String"
    }
  ]
}
```








