# <a name="devicecompliancepolicysettingstate-resource-type"></a>Тип ресурса deviceCompliancePolicySettingState

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Состояние параметров политики соответствия требованиям для определенного устройства.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|setting|String (строка)|Параметр для отчета|
|settingName|String (строка)|Локализованное или понятное имя параметра для отчета|
|instanceDisplayName|String (строка)|Имя экземпляра параметра для отчета|
|state|[complianceStatus](../resources/intune_shared_compliancestatus.md)|Состояние соответствия параметра. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.|
|errorCode|Int64|Код ошибки для параметра|
|errorDescription|String (строка)|Описание ошибки|
|userId|String (строка)|ИД пользователя|
|userName|String (строка)|Имя пользователя|
|userEmail|String (строка)|Электронный адрес пользователя|
|userPrincipalName|String (строка)|Имя участника-пользователя.|
|sources|Коллекция [settingSource](../resources/intune_deviceconfig_settingsource.md)|Соответствующие политики|
|currentValue|String (строка)|Текущее значение параметра на устройстве|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
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
```



