# <a name="devicecompliancesettingstate-resource-type"></a>Тип ресурса deviceComplianceSettingState

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Состояние параметров соответствия требованиям для определенного устройства.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceComplianceSettingState](../api/intune_deviceconfig_devicecompliancesettingstate_list.md)|Коллекция [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)|Список свойств и связей объектов [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).|
|[Получение объекта deviceComplianceSettingState](../api/intune_deviceconfig_devicecompliancesettingstate_get.md)|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)|Чтение свойств и связей объекта [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).|
|[Создание объекта deviceComplianceSettingState](../api/intune_deviceconfig_devicecompliancesettingstate_create.md)|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)|Создание объекта [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).|
|[Удаление объекта deviceComplianceSettingState](../api/intune_deviceconfig_devicecompliancesettingstate_delete.md)|Нет|Удаляет объект [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).|
|[Обновление объекта deviceComplianceSettingState](../api/intune_deviceconfig_devicecompliancesettingstate_update.md)|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)|Обновление свойств объекта [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта|
|setting|String|Имя класса параметров и свойства.|
|settingName|String|Имя параметра в отчете|
|deviceId|String|ИД устройства в отчете|
|deviceName|String|Имя устройства в отчете|
|userId|String|ИД пользователя в отчете|
|userEmail|String|Электронный адрес пользователя в отчете|
|userName|String|Имя пользователя в отчете|
|userPrincipalName|String|Имя участника-пользователя в отчете|
|deviceModel|String|Модель устройства в отчете|
|state|String|Состояние соответствия требованиям для параметра. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Дата и время истечения льготного периода соответствия требования для устройства|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "String (identifier)",
  "setting": "String",
  "settingName": "String",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userEmail": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "deviceModel": "String",
  "state": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)"
}
```



