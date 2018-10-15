# <a name="managedappprotection-resource-type"></a>Тип ресурса managedAppProtection

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Политика, используемая для настройки расширенных параметров управления для определенного набора приложений.

Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов managedAppProtection](../api/intune_mam_managedappprotection_list.md)|Коллекция объектов [managedAppProtection](../resources/intune_mam_managedappprotection.md)|Список свойств и связей объектов [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|[Получение объекта managedAppProtection](../api/intune_mam_managedappprotection_get.md)|[объект managedAppProtection](../resources/intune_mam_managedappprotection.md)|Чтение свойств и связей объекта [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|[Действие targetApps](../api/intune_mam_managedappprotection_targetapps.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|описание|Строка|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|ид|Строка|Ключ объекта. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|версия|Строка|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|periodOfflineBeforeAccessCheck|Продолжительность|Время до проверки доступа, когда устройство не подключено к Интернету.|
|periodOnlineBeforeAccessCheck|Продолжительность|Время до проверки доступа, когда устройство подключено к Интернету.|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune_mam_managedappdatatransferlevel.md)|Источники, с которых данные могут передаваться. Возможные значения: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune_mam_managedappdatatransferlevel.md)|Назначения, к которым могут передаваться данные. Возможные значения: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Boolean (логический)|Указывает, необходимы ли для использования приложения учетные данные организации.|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune_mam_managedappclipboardsharinglevel.md)|Уровень, на который буфер обмена может делиться между приложениями на управляемом устройстве. Возможные значения: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolean (логический)|Указывает, заблокировано ли резервное копирование данных управляемого приложения.|
|deviceComplianceRequired|Boolean (логический)|Указывает, должно ли устройство соответствовать требованиям.|
|managedBrowserToOpenLinksRequired|Boolean (логический)|Указывает, следует ли открывать интернет-ссылки в управляемом браузере.|
|saveAsBlocked|Boolean (логический)|Указывает, могут ли пользователи сохранять копии защищенных файлов, используя пункт меню "Сохранить как".|
|periodOfflineBeforeWipeIsEnforced|Продолжительность|Время до удаления всех управляемых данных после отключения приложения от Интернета.|
|pinRequired|Boolean (логический)|Указывает, требуется ли ПИН-код на уровне приложения.|
|maximumPinRetries|Int32|Максимальное количество неудачных попыток ввода ПИН-кода до блокировки или стирания управляемого приложения.|
|simplePinBlocked|Boolean (логический)|Указывает, заблокирован ли простой ПИН-код.|
|minimumPinLength|Int32|Минимальная длина ПИН-кода на уровне приложения, если для параметра PinRequired установлено значение True.|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune_mam_managedapppincharacterset.md)|Набор символов, который может использоваться для вывода на уровне приложения, если для параметра PinRequired установлено значение True. Возможные значения: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Продолжительность|Время до сброса универсального ПИН-кода, если для параметра PinRequired установлено значение True.|
|allowedDataStorageLocations|Коллекция [managedAppDataStorageLocation](../resources/intune_mam_managedappdatastoragelocation.md)|Разрешенные места хранения управляемых данных.|
|contactSyncBlocked|Boolean (логический)|Указывает, можно ли синхронизировать контакты с устройством пользователя.|
|printBlocked|Boolean (логический)|Указывает, разрешена ли печать из управляемых приложений.|
|fingerprintBlocked|Boolean (логический)|Указывает, можно ли использовать сканер отпечатков пальцев вместо ПИН-кода, если для параметра PinRequired установлено значение True.|
|disableAppPinIfDevicePinIsSet|Boolean (логический)|Указывает, обязательно ли использовать ПИН-код приложения, если установлен ПИН-код устройства.|
|minimumRequiredOsVersion|Строка|В более старых версиях управляемое приложение не сможет получить доступ к данным компании.|
|minimumWarningOsVersion|Строка|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение о невозможности получить доступ к данным компании.|
|minimumRequiredAppVersion|Строка|В более старых версиях управляемое приложение не сможет получить доступ к данным компании.|
|minimumWarningAppVersion|Строка|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedAppPolicy",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppProtection"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppProtection",
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
  "minimumWarningAppVersion": "String"
}
```








