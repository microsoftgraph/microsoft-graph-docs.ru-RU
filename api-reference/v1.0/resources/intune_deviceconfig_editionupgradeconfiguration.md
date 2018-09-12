# <a name="editionupgradeconfiguration-resource-type"></a>Тип ресурса editionUpgradeConfiguration

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Конфигурация обновления выпуска Windows 10.

Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление editionUpgradeConfigurations](../api/intune_deviceconfig_editionupgradeconfiguration_list.md)|Коллекция [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md)|Список свойств и связей объектов [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md).|
|[Получение editionUpgradeConfiguration](../api/intune_deviceconfig_editionupgradeconfiguration_get.md)|[editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md)|Считывание свойств и связей объекта [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md).|
|[Создание editionUpgradeConfiguration](../api/intune_deviceconfig_editionupgradeconfiguration_create.md)|[editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md)|Создание объекта [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md).|
|[Удаление editionUpgradeConfiguration](../api/intune_deviceconfig_editionupgradeconfiguration_delete.md)|Нет|Удаление экземпляра [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md).|
|[Обновление editionUpgradeConfiguration](../api/intune_deviceconfig_editionupgradeconfiguration_update.md)|[editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md)|Обновление свойств объекта [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|description|Строка|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|licenseType|[editionUpgradeLicenseType](../resources/intune_deviceconfig_editionupgradelicensetype.md)|Тип лицензии обновления версии. Возможные значения: `productKey`, `licenseFile`.|
|targetEdition|[windows10EditionType](../resources/intune_deviceconfig_windows10editiontype.md)|Целевой выпуск для обновления. Возможные значения: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.|
|license|Строка|Содержимое файла лицензии для обновления выпуска.|
|productKey|Строка|Ключ продукта для обновления выпуска.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|задания|Коллекция [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|статусы пользователя|Коллекция [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceConfiguration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.editionUpgradeConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "licenseType": "String",
  "targetEdition": "String",
  "license": "String",
  "productKey": "String"
}
```








