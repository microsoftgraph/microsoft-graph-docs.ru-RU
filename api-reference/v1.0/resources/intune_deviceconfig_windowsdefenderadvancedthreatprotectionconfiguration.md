# <a name="windowsdefenderadvancedthreatprotectionconfiguration-resource-type"></a>Тип ресурса windowsDefenderAdvancedThreatProtectionConfiguration

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Конфигурация Advanced Threat Protection в Защитника Windows.

Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов windowsDefenderAdvancedThreatProtectionConfiguration](../api/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration_list.md)|Коллекция [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md)|Список свойств и связей объектов [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).|
|[Получение объекта windowsDefenderAdvancedThreatProtectionConfiguration](../api/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration_get.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md)|Чтение свойств и связей объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).|
|[Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration](../api/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration_create.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md)|Создание объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).|
|[Удаление объекта windowsDefenderAdvancedThreatProtectionConfiguration](../api/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration_delete.md)|Нет|Удаляет объект [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).|
|[Обновление объекта windowsDefenderAdvancedThreatProtectionConfiguration](../api/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration_update.md)|[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md)|Обновление свойств объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|description|String (строка)|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|String (строка)|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|allowSampleSharing|Boolean (логический)|Правило "Разрешить общий доступ к выборкам" службы Advanced Threat Protection в Защитнике Windows|
|enableExpeditedTelemetryReporting|Boolean (логический)|Повышение частоты отправки отчетов о телеметрии службой Advanced Threat Protection в Защитнике Windows.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.deviceConfiguration",
  "@odata.type": "microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```



