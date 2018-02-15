# <a name="devicecompliancepolicystate-resource-type"></a>Тип ресурса deviceCompliancePolicyState

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Состояние политики соответствия требованиям для определенного устройства.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceCompliancePolicyState](../api/intune_deviceconfig_devicecompliancepolicystate_list.md)|Коллекция [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)|Список свойств и связей объектов [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md).|
|[Получение объекта deviceCompliancePolicyState](../api/intune_deviceconfig_devicecompliancepolicystate_get.md)|[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)|Чтение свойств и связей объекта [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md).|
|[Создание объекта deviceCompliancePolicyState](../api/intune_deviceconfig_devicecompliancepolicystate_create.md)|[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)|Создание объекта [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md).|
|[Удаление объекта deviceCompliancePolicyState](../api/intune_deviceconfig_devicecompliancepolicystate_delete.md)|Нет|Удаляет объект [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md).|
|[Обновление объекта deviceCompliancePolicyState](../api/intune_deviceconfig_devicecompliancepolicystate_update.md)|[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)|Обновление свойств объекта [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|settingStates|Коллекция [deviceCompliancePolicySettingState](../resources/intune_deviceconfig_devicecompliancepolicysettingstate.md)|Н/Д|
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
  "@odata.type": "microsoft.graph.deviceCompliancePolicyState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
  "id": "String (identifier)",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState",
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



