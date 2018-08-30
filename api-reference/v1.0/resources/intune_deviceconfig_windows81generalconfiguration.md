# <a name="windows81generalconfiguration-resource-type"></a>Тип ресурса windows81GeneralConfiguration

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом windows81GeneralConfiguration.

Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов windows81GeneralConfiguration](../api/intune_deviceconfig_windows81generalconfiguration_list.md)|Коллекция [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)|Перечисление свойств и связей объектов [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).|
|[Получение объекта windows81GeneralConfiguration](../api/intune_deviceconfig_windows81generalconfiguration_get.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)|Чтение свойств и связей объекта [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).|
|[Создание объекта windows81GeneralConfiguration](../api/intune_deviceconfig_windows81generalconfiguration_create.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)|Создание объекта [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).|
|[Удаление объекта windows81GeneralConfiguration](../api/intune_deviceconfig_windows81generalconfiguration_delete.md)|Нет|Удаление объекта [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).|
|[Обновление объекта windows81GeneralConfiguration](../api/intune_deviceconfig_windows81generalconfiguration_update.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)|Обновление свойств объекта [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|description|Строка​|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|Строка​|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|accountsBlockAddingNonMicrosoftAccountEmail|Логический|Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.|
|applyOnlyToWindows81|Логический|Указывает, применяется ли эта политика только к Windows 8.1. Это свойство доступно только для чтения.|
|browserBlockAutofill|Логический|Указывает, следует ли заблокировать автозаполнение.|
|browserBlockAutomaticDetectionOfIntranetSites|Логический|Указывает, следует ли заблокировать автоматическое обнаружение сайтов интрасети.|
|browserBlockEnterpriseModeAccess|Логический|Указывает, следует ли заблокировать доступ к корпоративному режиму.|
|browserBlockJavaScript|Логический|Указывает, следует ли запретить использование JavaScript.|
|browserBlockPlugins|Логический|Указывает, следует ли заблокировать подключаемые модули.|
|browserBlockPopups|Логический|Указывает, следует ли блокировать всплывающие окна.|
|browserBlockSendingDoNotTrackHeader|Логический|Указывает, следует ли запретить пользователю отправлять заголовок DNT.|
|browserBlockSingleWordEntryOnIntranetSites|Логический|Указывает, следует ли блокировать переход на сайты интрасети при вводе одного слова.|
|browserRequireSmartScreen|Логический|Указывает, обязательно ли использовать фильтр Smart Screen.|
|browserEnterpriseModeSiteListLocation|Строка​|Расположение списка сайтов, запускаемых в корпоративном режиме. Это может быть локальный файл, локальная сеть или HTTP-адрес.|
|browserInternetSecurityLevel|[internetSiteSecurityLevel](../resources/intune_deviceconfig_internetsitesecuritylevel.md)|Уровень интернет-безопасности. Возможные значения: `userDefined`, `medium`, `mediumHigh`, `high`.|
|browserIntranetSecurityLevel|[siteSecurityLevel](../resources/intune_deviceconfig_sitesecuritylevel.md)|Уровень безопасности интрасети. Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.|
|browserLoggingReportLocation|Строка​|Расположение хранения отчетов.|
|browserRequireHighSecurityForRestrictedSites|Логический|Указывает, обязателен ли высокий уровень безопасности для опасных сайтов.|
|browserRequireFirewall|Логический|Указывает, обязательно ли использовать брандмауэр.|
|browserRequireFraudWarning|Логический|Указывает, обязательно ли предупреждение о мошенничестве.|
|browserTrustedSitesSecurityLevel|[siteSecurityLevel](../resources/intune_deviceconfig_sitesecuritylevel.md)|Уровень безопасности надежных сайтов. Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.|
|cellularBlockDataRoaming|Логический|Указывает, следует ли блокировать передачу данных в роуминге.|
|diagnosticsBlockDataSubmission|Логический|Указывает, следует ли блокировать отправку диагностических данных.|
|passwordBlockPicturePasswordAndPin|Логический|Указывает, следует ли запретить использование графического пароля и ПИН-кода.|
|passwordExpirationDays|Int32|Срок действия пароля (в днях).|
|passwordMinimumLength|Int32|Минимальная длина пароля.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Время бездействия до отключения экрана (в минутах).|
|passwordMinimumCharacterSetCount|Int32|Количество наборов символов, которые требуются для пароля.|
|passwordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей, повторное использование которых следует запретить. Допустимые значения: от 0 до 24|
|passwordRequiredType|[requiredPasswordType](../resources/intune_deviceconfig_requiredpasswordtype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Количество неудачных попыток входа до восстановления заводских настроек.|
|storageRequireDeviceEncryption|Логический|Указывает, обязательно ли шифрование данных на мобильном устройстве.|
|updatesRequireAutomaticUpdates|Логический|Указывает, обязательно ли автоматическое обновление.|
|userAccountControlSettings|[windowsUserAccountControlSettings](../resources/intune_deviceconfig_windowsuseraccountcontrolsettings.md)|Настройки контроля учетных записей. Возможные значения: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.|
|workFoldersUrl|Строка​|URL-адрес рабочей папки.|

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
  "@odata.type": "microsoft.graph.windows81GeneralConfiguration",
  "@odata.annotations": [
    {
      "property": "applyOnlyToWindows81",
      "capabilities": {
        "computed": true,
        "permissions": "Read"
      }
    }
  ]
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "String",
  "browserInternetSecurityLevel": "String",
  "browserIntranetSecurityLevel": "String",
  "browserLoggingReportLocation": "String",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "String",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "String",
  "workFoldersUrl": "String"
}
```



