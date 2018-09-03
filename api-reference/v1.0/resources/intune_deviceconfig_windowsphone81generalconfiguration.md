# <a name="windowsphone81generalconfiguration-resource-type"></a>Тип ресурса windowsPhone81GeneralConfiguration

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом windowsPhone81GeneralConfiguration.

Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов windowsPhone81GeneralConfiguration](../api/intune_deviceconfig_windowsphone81generalconfiguration_list.md)|Коллекция [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md)|Перечисление свойств и связей объектов [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).|
|[Получение объекта windowsPhone81GeneralConfiguration](../api/intune_deviceconfig_windowsphone81generalconfiguration_get.md)|[windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md)|Чтение свойств и связей объекта [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).|
|[Создание объекта windowsPhone81GeneralConfiguration](../api/intune_deviceconfig_windowsphone81generalconfiguration_create.md)|[windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md)|Создание объекта [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).|
|[Удаление объекта windowsPhone81GeneralConfiguration](../api/intune_deviceconfig_windowsphone81generalconfiguration_delete.md)|Нет|Удаление объекта [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).|
|[Обновление объекта windowsPhone81GeneralConfiguration](../api/intune_deviceconfig_windowsphone81generalconfiguration_update.md)|[windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md)|Обновление свойств объекта [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|description|Строка​|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|Строка​|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|applyOnlyToWindowsPhone81|Логический|Указывает, применяется ли эта политика только к Windows Phone 8.1. Это свойство доступно только для чтения.|
|appsBlockCopyPaste|Логический|Указывает, следует ли заблокировать копирование данных.|
|bluetoothBlocked|Логический|Указывает, следует ли заблокировать Bluetooth.|
|cameraBlocked|Логический|Указывает, следует ли заблокировать камеру.|
|cellularBlockWifiTethering|Логический|Указывает, следует ли заблокировать модем Wi-Fi. Ни на что не влияет, если Wi-Fi заблокирован.|
|compliantAppsList|Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)|Список приложений (разрешенных или заблокированных в зависимости от значения свойства CompliantAppListType). Эта коллекция может содержать не более 10 000 элементов.|
|compliantAppListType|[appListType](../resources/intune_deviceconfig_applisttype.md)|Список свойства AppComplianceList. Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|diagnosticDataBlockSubmission|Логический|Указывает, следует ли заблокировать отправку диагностических данных.|
|emailBlockAddingAccounts|Логический|Указывает, следует ли заблокировать пользовательские учетные записи электронной почты.|
|locationServicesBlocked|Логический|Указывает, следует ли заблокировать службы определения местоположения.|
|microsoftAccountBlocked|Логический|Указывает, следует ли запретить использовать учетную запись Майкрософт.|
|nfcBlocked|Логический|Указывает, следует ли заблокировать NFC.|
|passwordBlockSimple|Логический|Указывает, следует ли заблокировать синхронизацию календаря.|
|passwordExpirationDays|Int32|Количество дней до окончания срока действия пароля.|
|passwordMinimumLength|Int32|Минимальная длина паролей.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Время с момента последнего действия до отключения экрана (в минутах).|
|passwordMinimumCharacterSetCount|Int32|Количество наборов символов, которые должен содержать пароль.|
|passwordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей, которые требуется блокировать. Допустимые значения: от 0 до 24|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Количество неудачных попыток входа до восстановления заводских настроек.|
|passwordRequiredType|[requiredPasswordType](../resources/intune_deviceconfig_requiredpasswordtype.md)|Необходимый тип пароля. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordRequired|Логический|Указывает, обязательно ли использовать пароль.|
|screenCaptureBlocked|Логический|Указывает, следует ли запретить делать снимки экрана.|
|storageBlockRemovableStorage|Логический|Указывает, следует ли запретить использовать съемные носители.|
|storageRequireEncryption|Логический|Указывает, обязательно ли шифрование.|
|webBrowserBlocked|Логический|Указывает, следует ли заблокировать веб-браузер.|
|wifiBlocked|Логический|Указывает, следует ли заблокировать Wi-Fi.|
|wifiBlockAutomaticConnectHotspots|Логический|Указывает, следует ли заблокировать автоматическое подключение к хот-спотам Wi-Fi. Ни на что не влияет, если Wi-Fi заблокирован.|
|wifiBlockHotspotReporting|Логический|Указывает, следует ли запретить устройству сообщать об обнаруженных хот-спотах Wi-Fi. Ни на что не влияет, если Wi-Fi заблокирован.|
|windowsStoreBlocked|Логический|Указывает, следует ли заблокировать Microsoft Store.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Device configuration installation status by user. Унаследовано от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.deviceConfiguration",
  "@odata.type": "microsoft.graph.windowsPhone81GeneralConfiguration",
  "@odata.annotations": [
    {
      "property": "applyOnlyToWindowsPhone81",
      "capabilities": {
        "computed": true,
        "permissions": "Read"
      }
    }
  ]
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "compliantAppListType": "String",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordRequiredType": "String",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```



