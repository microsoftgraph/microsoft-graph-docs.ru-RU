---
title: Тип ресурса managedAppProtection
description: Политика, используемая для настройки расширенных параметров управления для определенного набора приложений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67a925c695b19744b793bcaa6ecce7df3ecbb394
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158144"
---
# <a name="managedappprotection-resource-type"></a>Тип ресурса managedAppProtection

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

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
|displayName|String|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|description|String|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра сущности. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
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
|managedBrowserToOpenLinksRequired|Boolean|Указывает, следует ли открывать интернет-ссылки в управляемом браузере или настраиваемом браузере, указанном в CustomBrowserProtocol (для iOS) или CustomBrowserPackageId/CustomBrowserDisplayName (для Android)|
|saveAsBlocked|Boolean|Указывает, могут ли пользователи сохранять копии защищенных файлов, используя пункт меню "Сохранить как".|
|periodOfflineBeforeWipeIsEnforced|Duration|Время до удаления всех управляемых данных после отключения приложения от Интернета.|
|pinRequired|Boolean|Указывает, требуется ли ПИН-код на уровне приложения.|
|maximumPinRetries|Int32|Максимальное количество неудачных попыток повторной попытки закрепления до блокировки или стирки управляемого приложения.|
|simplePinBlocked|Boolean|Указывает, заблокирован ли простой ПИН-код.|
|minimumPinLength|Int32|Минимальная длина ПИН-кода на уровне приложения, если для параметра PinRequired установлено значение True.|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|Разрешенный набор символов ПИН-кода на уровне приложения, если для параметра PinRequired установлено значение True. Возможные значения: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Duration|Время до сброса универсального ПИН-кода, если для параметра PinRequired установлено значение True.|
|allowedDataStorageLocations|[Коллекция managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)|Разрешенные места хранения управляемых данных.|
|contactSyncBlocked|Boolean|Указывает, можно ли синхронизировать контакты с устройством пользователя.|
|printBlocked|Boolean|Указывает, разрешена ли печать из управляемых приложений.|
|fingerprintBlocked|Boolean|Указывает, можно ли использовать сканер отпечатков пальцев вместо ПИН-кода, если для параметра PinRequired установлено значение True.|
|disableAppPinIfDevicePinIsSet|Boolean|Указывает, обязательно ли использовать ПИН-код приложения, если установлен ПИН-код устройства.|
|maximumRequiredOsVersion|String|Версии, размером больше указанной версии, будут блокировать управляемому приложению доступ к данным компании.|
|maximumWarningOsVersion|String|Версии, размером больше указанной версии, будут блокировать управляемому приложению доступ к данным компании.|
|maximumWipeOsVersion|String|Версии, размером больше указанной версии, будут блокировать управляемому приложению доступ к данным компании.|
|minimumRequiredOsVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании.|
|minimumWarningOsVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение о невозможности получить доступ к данным компании.|
|minimumRequiredAppVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании.|
|minimumWarningAppVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение.|
|minimumWipeOsVersion|String|Версии, которые не равны указанной версии, будут стирать данные управляемого приложения и связанных с ним компаний.|
|minimumWipeAppVersion|String|Версии, не равные указанной версии, будут стирать данные управляемого приложения и связанных с ним компаний.|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения( блокировка или стирка), если устройство либо имеет корневой доступ, либо со стираемой блокировкой, если для DeviceComplianceRequired установлено true. Возможные значения: `block`, `wipe`, `warn`.|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения ( блокировка или стирка) на основе максимального количества неудачных попыток повторной попытки закрепления. Возможные значения: `block`, `wipe`, `warn`.|
|pinRequiredInsteadOfBiometricTimeout|Duration|Время в минутах для пин-кода приложения вместо биометрического пароля|
|allowedOutboundClipboardSharingExceptionLength|Int32|Укажите количество символов, которые можно вырезать или скопировать из данных и учетных записей организации в любое приложение. Этот параметр переопределяет ограничение AllowedOutboundClipboardSharingLevel. Значение по умолчанию "0" означает, что исключение не разрешено.|
|notificationRestriction|[managedAppNotificationRestriction](../resources/intune-mam-managedappnotificationrestriction.md)|Укажите ограничение уведомлений приложения. Возможные значения: `allow`, `blockOrganizationalData`, `block`.|
|previousPinBlockCount|Int32|Требуется, чтобы pin-код был уникальным по номеру, указанному в этом свойстве.|
|managedBrowser|[managedBrowserType](../resources/intune-mam-managedbrowsertype.md)|Указывает, в каких управляемых браузерах должны открываться интернет-ссылки. При настройке этого свойства свойство ManagedBrowserToOpenLinksRequired должно быть истинным. Возможные значения: `notConfigured`, `microsoftEdge`.|
|maximumAllowedDeviceThreatLevel|[managedAppDeviceThreatLevel](../resources/intune-mam-managedappdevicethreatlevel.md)|Максимальный допустимый уровень угроз устройства, о чем сообщает приложение MTD. Возможные значения: `notConfigured`, `secured`, `low`, `medium`, `high`.|
|mobileThreatDefenseRemediationAction|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет, какое действие необходимо принять, если не превышен порог угроз для защиты от угроз для мобильных устройств. Предупреждение не поддерживается для этого свойства. Возможные значения: `block`, `wipe`, `warn`.|
|blockDataIngestionIntoOrganizationDocuments|Boolean|Указывает, может ли пользователь сводить данные в документы организации.|
|allowedDataIngestionLocations|[Коллекция managedAppDataIngestionLocation](../resources/intune-mam-managedappdataingestionlocation.md)|Разрешенные места хранения управляемых данных.|
|appActionIfUnableToAuthenticateUser|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Если этот маркер установлен, он указывает, какое действие необходимо принять в случае, если пользователь не может проверить, так как маркер проверки подлинности недействителен. Это происходит, когда пользователь удаляется или отключается в AAD. Возможные значения: `block`, `wipe`, `warn`.|
|dialerRestrictionLevel|[managedAppPhoneNumberRedirectLevel](../resources/intune-mam-managedappphonenumberredirectlevel.md)|Классы приложений для набора номера, которые могут открывать телефонный номер по щелчку. Возможные значения: `allApps`, `managedApps`, `customApp`, `blocked`.|

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




