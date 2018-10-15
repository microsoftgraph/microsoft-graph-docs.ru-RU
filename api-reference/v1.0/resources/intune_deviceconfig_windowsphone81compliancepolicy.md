# <a name="windowsphone81compliancepolicy-resource-type"></a>Тип ресурса windowsPhone81CompliancePolicy

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Этот класс содержит параметры обеспечения соответствия требованиям для Windows 8.1 Mobile.

Наследуется от [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление windowsPhone81CompliancePolicies](../api/intune_deviceconfig_windowsphone81compliancepolicy_list.md)|Коллекция [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md)|Список свойств и связей объектов [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md).|
|[Получение windowsPhone81CompliancePolicy](../api/intune_deviceconfig_windowsphone81compliancepolicy_get.md)|[windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md)|Считывание свойств и связей объекта [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md).|
|[Создание windowsPhone81CompliancePolicy](../api/intune_deviceconfig_windowsphone81compliancepolicy_create.md)|[windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md)|Создание объекта [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md).|
|[Удаление windowsPhone81CompliancePolicy](../api/intune_deviceconfig_windowsphone81compliancepolicy_delete.md)|Нет|Удаление экземпляра [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md).|
|[Обновление windowsPhone81CompliancePolicy](../api/intune_deviceconfig_windowsphone81compliancepolicy_update.md)|[windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md)|Обновление свойств объекта [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|дата и время создания|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|description|Строка|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|дата и время последних изменений|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|отображаемое имя|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|версия|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|простой блокирующий пароль|Логический|Определяет, нужно ли блокировать синхронизацию календаря.|
|дни до истечения срока действия пароля|Int32|Количество дней до окончания срока действия пароля.|
|минимальная длина пароля|Int32|Минимальная длина паролей.|
|минуты бездействия при вводе пароля перед блокировкой|Int32|Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.|
|настройка счётчика минимального количества символов пароля|Int32|Количество наборов символов, которые требуются для пароля.|
|passwordRequiredType|[требуемый тип пароля](../resources/intune_deviceconfig_requiredpasswordtype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей, которые требуется блокировать. Допустимые значения: от 0 до 24.|
|требуемый пароль|Логический|Определяет, нужно ли запрашивать ввод пароля.|
|минимальная версия оп|Строка|Минимальная версия Windows Phone.|
|максимальная версия оп|Строка|Максимальная версия Windows Phone.|
|необходимое шифрование для хранилища|Логический|Указывает на то, что шифрование на устройствах с Windows Phone должно быть обязательным.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|запланированные действия для контроля|Коллекция [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|Список запланированных действий для этого правила. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|статусы устройства|Коллекция объектов [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md)|Список DeviceComplianceDeviceStatus. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|статусы пользователя|Коллекция объектов [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|Список DeviceComplianceUserStatus. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|обзор статусов устройства|[обзор отчёта по соответствию устройства](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|Обзор состояния обеспечения соответствия требованиям для устройств. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|userStatusOverview|[обзор отчёта по соответствию устройства пользователя](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|Обзор состояния обеспечения соответствия требованиям для устройств, указанного для пользователей. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Сводка данных о состоянии настройки обеспечения соответствия требованиям для устройств. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|задания|Коллекция [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|Коллекция назначений для этой политики соответствия требованиям. Наследуется от объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceCompliancePolicy",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPhone81CompliancePolicy"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequired": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "storageRequireEncryption": true
}
```








