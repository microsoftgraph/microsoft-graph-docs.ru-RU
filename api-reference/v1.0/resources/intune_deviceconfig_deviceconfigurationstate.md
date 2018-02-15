# <a name="deviceconfigurationstate-resource-type"></a>Тип ресурса deviceConfigurationState

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Состояние конфигурации определенного устройства.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceConfigurationState](../api/intune_deviceconfig_deviceconfigurationstate_list.md)|Коллекция [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)|Список свойств и связей объектов [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md).|
|[Получение объекта deviceConfigurationState](../api/intune_deviceconfig_deviceconfigurationstate_get.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)|Чтение свойств и связей объекта [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md).|
|[Создание объекта deviceConfigurationState](../api/intune_deviceconfig_deviceconfigurationstate_create.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)|Создание объекта [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md).|
|[Удаление объекта deviceConfigurationState](../api/intune_deviceconfig_deviceconfigurationstate_delete.md)|Нет|Удаляет объект [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md).|
|[Обновление объекта deviceConfigurationState](../api/intune_deviceconfig_deviceconfigurationstate_update.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)|Обновление свойств объекта [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|settingStates|Коллекция [deviceConfigurationSettingState](../resources/intune_deviceconfig_deviceconfigurationsettingstate.md)|Н/Д|
|displayName|String|Имя политики для этой основы|
|version|Int32|Версия политики|
|platformType|String|Тип платформы, к которой относится политика. Возможные значения: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.|
|state|String|Состояние соответствия требованиям для политики. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.|
|settingCount|Int32|Количество параметров, которые включает политики|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationState",
  "id": "String (identifier)",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationSettingState",
      "setting": "String",
      "settingName": "String",
      "instanceDisplayName": "String",
      "state": "String",
      "errorCode": 1024,
      "errorDescription": "String",
      "userId": "String",
      "userName": "String",
      "userEmail": "String",
      "userPrincipalName": "String",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "String",
          "displayName": "String"
        }
      ],
      "currentValue": "String"
    }
  ],
  "displayName": "String",
  "version": 1024,
  "platformType": "String",
  "state": "String",
  "settingCount": 1024
}
```



