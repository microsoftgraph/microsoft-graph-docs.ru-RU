# <a name="iosupdateconfiguration-resource-type"></a>Тип ресурса iosUpdateConfiguration

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Конфигурация обновления iOS. Позволяет настраивать	временной промежуток в рамках недели для установки обновлений iOS.

Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление iosUpdateConfigurations](../api/intune_deviceconfig_iosupdateconfiguration_list.md)|Коллекция [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)|Список свойств и связей объектов [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).|
|[Получение iosUpdateConfiguration](../api/intune_deviceconfig_iosupdateconfiguration_get.md)|[iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)|Считывание свойств и связей объекта [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).|
|[Создание iosUpdateConfiguration](../api/intune_deviceconfig_iosupdateconfiguration_create.md)|[iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)|Создание объекта [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).|
|[Удаление iosUpdateConfiguration](../api/intune_deviceconfig_iosupdateconfiguration_delete.md)|None|Удаление экземпляра [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).|
|[Обновление iosUpdateConfiguration](../api/intune_deviceconfig_iosupdateconfiguration_update.md)|[iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md)|Обновление свойств объекта [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|activeHoursStart|TimeOfDay|Начало периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).|
|activeHoursEnd|TimeOfDay|Завершение периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).|
|scheduledInstallDays|Коллекция String|Дни недели, для которых настраивается период активности. Эта коллекция может содержать не более 7 элементов.|
|utcTimeOffsetInMinutes|Int32|Сдвиг по времени от UTC (в минутах).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства для каждого пользователя. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Обзор состояния параметров конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosUpdateConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)",
  "scheduledInstallDays": [
    "String"
  ],
  "utcTimeOffsetInMinutes": 1024
}
```



