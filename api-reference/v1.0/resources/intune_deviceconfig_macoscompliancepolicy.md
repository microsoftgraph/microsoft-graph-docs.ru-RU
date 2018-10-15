# <a name="macoscompliancepolicy-resource-type"></a>Тип ресурса macOSCompliancePolicy

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Этот класс содержит параметры обеспечения соответствия требованиям для Mac OS.

Наследуется от [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление macOSCompliancePolicies](../api/intune_deviceconfig_macoscompliancepolicy_list.md)|Коллекция [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md)|Список свойств и связей объектов [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md).|
|[Получение macOSCompliancePolicy](../api/intune_deviceconfig_macoscompliancepolicy_get.md)|[macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md)|Считывание свойств и связей объекта [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md).|
|[Создание macOSCompliancePolicy](../api/intune_deviceconfig_macoscompliancepolicy_create.md)|[macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md)|Создание объекта [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md).|
|[Удаление macOSCompliancePolicy](../api/intune_deviceconfig_macoscompliancepolicy_delete.md)|None|Удаление экземпляра [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md).|
|[Обновление macOSCompliancePolicy](../api/intune_deviceconfig_macoscompliancepolicy_update.md)|[macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md)|Обновление свойств объекта [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|passwordRequired|Boolean|Определяет, нужно ли запрашивать ввод пароля.|
|passwordBlockSimple|Boolean|Указывает, требуется ли блокировать простые пароли.|
|passwordExpirationDays|Int32|Количество дней до окончания срока действия пароля. Допустимые значения: от 1 до 65 535.|
|passwordMinimumLength|Int32|Минимальная длина пароля. Допустимые значения: от 4 до 14.|
|passwordMinutesOfInactivityBeforeLock|Int32|Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.|
|passwordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей, которые требуется блокировать. Допустимые значения: от 1 до 24.|
|passwordMinimumCharacterSetCount|Int32|Количество наборов символов, которые требуются для пароля.|
|passwordRequiredType|[requiredPasswordType](../resources/intune_deviceconfig_requiredpasswordtype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|osMinimumVersion|String|Минимальная версия iOS.|
|osMaximumVersion|String|Максимальная версия iOS.|
|systemIntegrityProtectionEnabled|Boolean|Указывает на то, что защита целостности системы для устройств должна быть включена.|
|deviceThreatProtectionEnabled|Boolean|Указывает, что защита от угроз для устройств должна быть включена.|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям. Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.|
|storageRequireEncryption|Boolean|Указывает, обязательно ли шифрование данных на устройствах с Mac OS.|
|firewallEnabled|Boolean|Указывает, должен ли быть включен брандмауэр.|
|firewallBlockAllIncoming|Boolean|Соответствует параметру "Блокировать все входящие подключения".|
|firewallEnableStealthMode|Boolean|Соответствует параметру "Включить скрытый режим".|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|scheduledActionsForRule|Коллекция [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|Список запланированных действий для этого правила. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|deviceStatuses|Коллекция объектов [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md)|Список DeviceComplianceDeviceStatus. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|userStatuses|Коллекция объектов [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|Список DeviceComplianceUserStatus. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|Обзор состояния обеспечения соответствия требованиям для устройств. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|Обзор состояния обеспечения соответствия требованиям для устройств, указанного для пользователей. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Сводка данных о состоянии настройки обеспечения соответствия требованиям для устройств. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|assignments|Коллекция [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|Коллекция назначений для этой политики соответствия требованиям. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.deviceCompliancePolicy",
  "@odata.type": "microsoft.graph.macOSCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```



