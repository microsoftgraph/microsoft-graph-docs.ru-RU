---
title: Тип ресурса managedAppProtection
description: Политика, используемая для настройки расширенных параметров управления для определенного набора приложений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6119daa33b3340470bfed4432533308181edc1ff
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806609"
---
# <a name="managedappprotection-resource-type"></a>Тип ресурса managedAppProtection

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политика, используемая для настройки расширенных параметров управления для определенного набора приложений.


Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов managedAppProtection](../api/intune-mam-managedappprotection-list.md)|Коллекция объектов [managedAppProtection](../resources/intune-mam-managedappprotection.md)|Список свойств и связей объектов [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|[Получение объекта managedAppProtection](../api/intune-mam-managedappprotection-get.md)|[managedAppProtection](../resources/intune-mam-managedappprotection.md)|Чтение свойств и связей объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|[Действие targetApps](../api/intune-mam-managedappprotection-targetapps.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|description|Строка|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|id|String|Ключ объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|version|String|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|periodOfflineBeforeAccessCheck|Duration|Время до проверки доступа, когда устройство не подключено к Интернету.|
|periodOnlineBeforeAccessCheck|Duration|Время до проверки доступа, когда устройство подключено к Интернету.|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Источники, из которых разрешена передача данных. Возможные значения: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Места, в которые разрешена передача данных. Возможные значения: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Boolean|Указывает, необходимы ли для использования приложения учетные данные организации.|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|Разрешенный уровень совместного использования буфера обмена для приложений на управляемом устройстве. Возможные значения: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolean|Указывает, заблокировано ли резервное копирование данных управляемого приложения.|
|deviceComplianceRequired|Boolean|Указывает, должно ли устройство соответствовать требованиям.|
|managedBrowserToOpenLinksRequired|Boolean|Указывает, следует ли открывать интернет-ссылки в управляемом браузере или любом настраиваемом браузере, указанном CustomBrowserProtocol (для iOS) или CustomBrowserPackageId/CustomBrowserDisplayName (для Android)|
|saveAsBlocked|Boolean|Указывает, могут ли пользователи сохранять копии защищенных файлов, используя пункт меню "Сохранить как".|
|periodOfflineBeforeWipeIsEnforced|Duration|Время до удаления всех управляемых данных после отключения приложения от Интернета.|
|pinRequired|Boolean|Указывает, требуется ли ПИН-код на уровне приложения.|
|maximumPinRetries|Int32|Максимальное количество неправильных попыток повторить пин-код до блокировки или стирки управляемого приложения.|
|simplePinBlocked|Boolean|Указывает, заблокирован ли простой ПИН-код.|
|minimumPinLength|Int32|Минимальная длина ПИН-кода на уровне приложения, если для параметра PinRequired установлено значение True.|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|Разрешенный набор символов ПИН-кода на уровне приложения, если для параметра PinRequired установлено значение True. Возможные значения: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Duration|Время до сброса универсального ПИН-кода, если для параметра PinRequired установлено значение True.|
|allowedDataStorageLocations|[коллекция managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)|Разрешенные места хранения управляемых данных.|
|contactSyncBlocked|Boolean|Указывает, можно ли синхронизировать контакты с устройством пользователя.|
|printBlocked|Boolean|Указывает, разрешена ли печать из управляемых приложений.|
|fingerprintBlocked|Boolean|Указывает, можно ли использовать сканер отпечатков пальцев вместо ПИН-кода, если для параметра PinRequired установлено значение True.|
|disableAppPinIfDevicePinIsSet|Boolean|Указывает, обязательно ли использовать ПИН-код приложения, если установлен ПИН-код устройства.|
|maximumRequiredOsVersion|Строка|Версии, размером больше указанной версии, заблокируют доступ к данным компании управляемому приложению.|
|maximumWarningOsVersion|Строка|Версии, размером больше указанной версии, заблокируют доступ к данным компании управляемому приложению.|
|maximumWipeOsVersion|Строка|Версии, размером больше указанной версии, заблокируют доступ к данным компании управляемому приложению.|
|minimumRequiredOsVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании.|
|minimumWarningOsVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение о невозможности получить доступ к данным компании.|
|minimumRequiredAppVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании.|
|minimumWarningAppVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение.|
|minimumWipeOsVersion|Строка|Версии, менее или равные указанной версии, стирают управляемое приложение и связанные с ним данные компании.|
|minimumWipeAppVersion|Строка|Версии, менее или равные указанной версии, стирают управляемое приложение и связанные с ним данные компании.|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет управляемое поведение приложения, блок или стирка, когда устройство либо коренится, либо jailbroken, если устройствоComplianceRequired настроено на верность. Возможные значения: `block`, `wipe`, `warn`.|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет управляемое поведение приложения, блок или стирка, основываясь на максимальном количестве попыток повторного повторного действия пин-кода. Возможные значения: `block`, `wipe`, `warn`.|
|pinRequiredInsteadOfBiometricTimeout|Длительность|Время в минутах для пин-кода приложения вместо код-код без биометрии|
|allowedOutboundClipboardSharingExceptionLength|Int32|Укажите количество символов, которые могут быть сокращены или скопированы из данных и учетных записей Org в любое приложение. Этот параметр переопределяет ограничение AllowedOutboundClipboardSharingLevel. Значение "0" по умолчанию означает, что исключений не допускается.|
|notificationRestriction|[managedAppNotificationRestriction](../resources/intune-mam-managedappnotificationrestriction.md)|Укажите ограничение уведомлений приложения. Возможные значения: `allow`, `blockOrganizationalData`, `block`.|
|предыдущийPinBlockCount|Int32|Требуется, чтобы пин-код был уникальным из числа, указанного в этом свойстве.|
|managedBrowser|[managedBrowserType](../resources/intune-mam-managedbrowsertype.md)|Указывает, в каких управляемых браузерах (ы) необходимо открыть ссылки в Интернете. Когда это свойство настроено, managedBrowserToOpenLinksRequired должно быть верным. Возможные значения: `notConfigured`, `microsoftEdge`.|
|maximumAllowedDeviceThreatLevel|[managedAppDeviceThreatLevel](../resources/intune-mam-managedappdevicethreatlevel.md)|Максимально допустимый уровень угрозы устройства, как сообщается в приложении MTD. Возможные значения: `notConfigured`, `secured`, `low`, `medium`, `high`.|
|mobileThreatDefenseRemediationAction|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет, какие действия необходимо принять, если порог угрозы для защиты от мобильных угроз не установлен. Предупреждение не является поддерживаемой ценностью для этого свойства. Возможные значения: `block`, `wipe`, `warn`.|
|blockDataIngestionIntoOrganizationDocuments|Логический|Указывает, может ли пользователь приносить данные в документы орг.|
|allowedDataIngestionLocations|[коллекция managedAppDataIngestionLocation](../resources/intune-mam-managedappdataingestionlocation.md)|Разрешенные места хранения управляемых данных.|
|appActionIfUnableToAuthenticateUser|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|При наборе будет указано, какие действия необходимо принять в случае, если пользователь не может проверить, так как маркер проверки подлинности является недействительным. Это происходит, когда пользователь удаляется или отключен в AAD. Возможные значения: `block`, `wipe`, `warn`.|
|dialerRestrictionLevel|[managedAppPhoneNumberRedirectLevel](../resources/intune-mam-managedappphonenumberredirectlevel.md)|Классы приложений-дозвонищ, которые могут открывать телефонный номер. Возможные значения: `allApps`, `managedApps`, `customApp`, `blocked`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
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
  "maximumRequiredOsVersion": "String",
  "maximumWarningOsVersion": "String",
  "maximumWipeOsVersion": "String",
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String",
  "minimumWipeOsVersion": "String",
  "minimumWipeAppVersion": "String",
  "appActionIfDeviceComplianceRequired": "String",
  "appActionIfMaximumPinRetriesExceeded": "String",
  "pinRequiredInsteadOfBiometricTimeout": "String (duration)",
  "allowedOutboundClipboardSharingExceptionLength": 1024,
  "notificationRestriction": "String",
  "previousPinBlockCount": 1024,
  "managedBrowser": "String",
  "maximumAllowedDeviceThreatLevel": "String",
  "mobileThreatDefenseRemediationAction": "String",
  "blockDataIngestionIntoOrganizationDocuments": true,
  "allowedDataIngestionLocations": [
    "String"
  ],
  "appActionIfUnableToAuthenticateUser": "String",
  "dialerRestrictionLevel": "String"
}
```



