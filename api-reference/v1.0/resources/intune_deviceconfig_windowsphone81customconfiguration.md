# <a name="windowsphone81customconfiguration-resource-type"></a>Тип ресурса windowsPhone81CustomConfiguration

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом windowsPhone81CustomConfiguration.

Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление windowsPhone81CustomConfigurations](../api/intune_deviceconfig_windowsphone81customconfiguration_list.md)|Коллекция [windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md)|Перечисление свойств и связей объектов [windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md).|
|[Получение windowsPhone81CustomConfiguration](../api/intune_deviceconfig_windowsphone81customconfiguration_get.md)|[windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md)|Считывание свойств и связей объекта [windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md).|
|[Создание windowsPhone81CustomConfiguration](../api/intune_deviceconfig_windowsphone81customconfiguration_create.md)|[windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md)|Создание нового объекта [windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md).|
|[Удаление windowsPhone81CustomConfiguration](../api/intune_deviceconfig_windowsphone81customconfiguration_delete.md)|None|Удаление экземпляра [windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md).|
|[Обновление windowsPhone81CustomConfiguration](../api/intune_deviceconfig_windowsphone81customconfiguration_update.md)|[windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md)|Обновление свойств объекта [windowsPhone81CustomConfiguration](../resources/intune_deviceconfig_windowsphone81customconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|omaSettings|Коллекция [omaSetting](../resources/intune_deviceconfig_omasetting.md)|Параметры OMA. Эта коллекция может содержать не более 1000 элементов.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPhone81CustomConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "String",
      "description": "String",
      "omaUri": "String",
      "value": 1024
    }
  ]
}
```



