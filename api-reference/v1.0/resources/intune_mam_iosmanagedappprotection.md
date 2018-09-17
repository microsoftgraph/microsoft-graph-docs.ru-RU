# <a name="iosmanagedappprotection-resource-type"></a>Тип ресурса iosManagedAppProtection

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Политика, используемая для настройки расширенных параметров управления для определенных групп безопасности и определенного набора приложений на устройстве iOS

Наследуется от [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов IosManagedAppProtection](../api/intune_mam_iosmanagedappprotection_list.md)|Коллекция [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md)|Перечисление свойств и связей объектов [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md).|
|[Получение объекта iosManagedAppProtection](../api/intune_mam_iosmanagedappprotection_get.md)|[iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md)|Чтение свойств и связей объекта [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md).|
|[Создание объекта iosManagedAppProtection](../api/intune_mam_iosmanagedappprotection_create.md)|[iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md)|Создание объекта [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md).|
|[Удаление объекта iosManagedAppProtection](../api/intune_mam_iosmanagedappprotection_delete.md)|Нет|Удаление объекта [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md).|
|[Обновление объекта iosManagedAppProtection](../api/intune_mam_iosmanagedappprotection_update.md)|[iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md)|Обновление свойств объекта [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String (строка)|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|описание|String (строка)|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|ИД|Строка|Ключ объекта. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|версия|String (строка)|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|periodOfflineBeforeAccessCheck|Продолжительность|Время до проверки доступа, когда устройство не подключено к Интернету. Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|periodOnlineBeforeAccessCheck|Продолжительность|Время до проверки доступа, когда устройство подключено к Интернету. Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune_mam_managedappdatatransferlevel.md)|Источники, с которых могут передаваться данные. Наследуется от [managedAppProtection](../resources/intune_mam_managedappprotection.md). Возможные значения: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune_mam_managedappdatatransferlevel.md)|Расположения, в которые разрешено передавать данные. Наследуется от [managedAppProtection](../resources/intune_mam_managedappprotection.md). Возможные значения: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Boolean (логический)|Указывает, необходимы ли для использования приложения учетные данные организации. Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune_mam_managedappclipboardsharinglevel.md)|Разрешенный уровень совместного использования буфера обмена для приложений на управляемом устройстве. Наследуется от [managedAppProtection](../resources/intune_mam_managedappprotection.md). Возможные значения: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolean (логический)|Указывает, заблокировано ли резервное копирование данных управляемого приложения. Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|deviceComplianceRequired|Boolean (логический)|Указывает, обязательно ли соответствие устройства требованиям. Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|managedBrowserToOpenLinksRequired|Boolean (логический)|Указывает, следует ли открывать интернет-ссылки в управляемом браузере. Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|saveAsBlocked|Boolean (логический)|Указывает, могут ли пользователи сохранять копии защищенных файлов, используя пункт меню "Сохранить как". Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|periodOfflineBeforeWipeIsEnforced|Продолжительность|Время до удаления всех управляемых данных после отключения приложения от Интернета. Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|pinRequired|Boolean (логический)|Указывает, обязательно ли использовать ПИН-код на уровне приложения. Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|maximumPinRetries|Int32|Максимальное количество неудачных попыток ввода ПИН-кода до блокировки или стирания управляемого приложения. Наследуется от [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|simplePinBlocked|Boolean (логический)|Указывает, заблокирован ли простой ПИН-код. Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumPinLength|Int32|Минимальная длина ПИН-кода на уровне приложения, если для параметра PinRequired задано значение True. Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune_mam_managedapppincharacterset.md)|Разрешенный набор символов ПИН-кода на уровне приложения, если для параметра PinRequired задано значение True. Наследуется от [managedAppProtection](../resources/intune_mam_managedappprotection.md). Возможные значения: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Продолжительность|Время до сброса универсального ПИН-кода, если для параметра PinRequired задано значение True. Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|allowedDataStorageLocations|Коллекция [managedAppDataStorageLocation](../resources/intune_mam_managedappdatastoragelocation.md)|Разрешенные места хранения управляемых данных. Наследуется от [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|contactSyncBlocked|Boolean (логический)|Указывает, можно ли синхронизировать контакты с устройством пользователя. Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|printBlocked|Boolean (логический)|Указывает, разрешена ли печать из управляемых приложений. Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|fingerprintBlocked|Boolean (логический)|Указывает, можно ли использовать сканер отпечатков пальцев вместо ПИН-кода, если для параметра PinRequired задано значение True. Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|disableAppPinIfDevicePinIsSet|Boolean (логический)|Указывает, обязательно ли использовать ПИН-код приложения, если задан ПИН-код устройства. Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumRequiredOsVersion|String (строка)|В более старых версиях управляемое приложение не сможет получить доступ к данным компании. Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumWarningOsVersion|String (строка)|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение о доступе к данным компании. Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumRequiredAppVersion|String (строка)|В более старых версиях управляемое приложение не сможет получить доступ к данным компании. Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumWarningAppVersion|String (строка)|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение. Наследуется от объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|isAssigned|Boolean (логический)|Указывает, применена ли политика к группам включения. Наследуется от [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md).|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune_mam_managedappdataencryptiontype.md)|Тип шифрования, который следует использовать для данных в управляемом приложении. Возможные значения: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.|
|minimumRequiredSdkVersion|String (строка)|В более старых версиях управляемое приложение не сможет получить доступ к данным компании.|
|deployedAppCount|Int32|Количество приложений, к которым применена текущая политика.|
|faceIdBlocked|Boolean (логический)|Указывает, можно ли использовать FaceID вместо ПИН-кода, если для параметра PinRequired установлено значение True.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|задания|Коллекция [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|Список групп включения и исключения, к которым применяется политика. Наследуется от [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md).|
|приложения|Коллекция [managedMobileApp](../resources/intune_mam_managedmobileapp.md)|Список приложений, к которым применена политика.|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md)|Свойства навигации к сводке по развертыванию конфигурации.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.targetedManagedAppProtection",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosManagedAppProtection"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "periodOfflineBeforeAccessCheck": "String (duration)",
  "periodOnlineBeforeAccessCheck": "String (duration)",
  "allowedInboundDataTransferSources": "String",
  "allowedOutboundDataTransferDestinations": "String",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "String",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "String (duration)",
  "pinRequired": true,
  "maximumPinRetries": 1024,
  "simplePinBlocked": true,
  "minimumPinLength": 1024,
  "pinCharacterSet": "String",
  "periodBeforePinReset": "String (duration)",
  "allowedDataStorageLocations": [
    "String"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String",
  "isAssigned": true,
  "appDataEncryptionType": "String",
  "minimumRequiredSdkVersion": "String",
  "deployedAppCount": 1024,
  "faceIdBlocked": true
}
```


<!-- {
  "type": "#page.annotation",
  "suppressions": [

"Warning: /api-reference/v1.0/resources/intune_mam_androidmanagedappprotection.md/microsoft.graph.androidManagedAppProtection/allowedDataStorageLocations:
      Inconsistent types between parameter (String) and table (Object)",

"Warning: /api-reference/v1.0/resources/intune_mam_defaultmanagedappprotection.md/microsoft.graph.defaultManagedAppProtection/allowedDataStorageLocations:
      Inconsistent types between parameter (String) and table (Object)",

"Warning: /api-reference/v1.0/resources/intune_mam_iosmanagedappprotection.md/microsoft.graph.iosManagedAppProtection/allowedDataStorageLocations:
      Inconsistent types between parameter (String) and table (Object)"

  ],
}
-->