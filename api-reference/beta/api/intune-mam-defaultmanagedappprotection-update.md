---
title: Обновление объекта defaultManagedAppProtection
description: Обновляет свойства объекта defaultManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df848c2a266b5ae097c971201ec7f5ef872d4783
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157003"
---
# <a name="update-defaultmanagedappprotection"></a>Обновление объекта defaultManagedAppProtection

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновляет свойства объекта [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).

## <a name="prerequisites"></a>Необходимые условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса добавьте представление объекта [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) в формате JSON.

Ниже показаны свойства, которые необходимо указывать при создании объекта [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|description|String|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра сущности. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|id|String|Ключ объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|version|String|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|periodOfflineBeforeAccessCheck|Duration|Время до проверки доступа, когда устройство не подключено к Интернету. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|periodOnlineBeforeAccessCheck|Duration|Время до проверки доступа, когда устройство подключено к Интернету. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Источники, из которых разрешена передача данных. Наследуется [от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Назначения, в которые разрешена передача данных. Наследуется [от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Boolean|Указывает, необходимы ли для использования приложения учетные данные организации. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|Разрешенный уровень совместного использования буфера обмена для приложений на управляемом устройстве. Наследуется [от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolean|Указывает, заблокировано ли резервное копирование данных управляемого приложения. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|deviceComplianceRequired|Boolean|Указывает, обязательно ли соответствие устройства требованиям. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|managedBrowserToOpenLinksRequired|Boolean|Указывает, следует ли открывать интернет-ссылки в управляемом браузере или настраиваемый браузер, указанный customBrowserProtocol (для iOS) или CustomBrowserPackageId/CustomBrowserDisplayName (для Android), унаследованный от [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|saveAsBlocked|Boolean|Указывает, могут ли пользователи сохранять копии защищенных файлов, используя пункт меню "Сохранить как". Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|periodOfflineBeforeWipeIsEnforced|Duration|Время до удаления всех управляемых данных после отключения приложения от Интернета. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|pinRequired|Boolean|Указывает, обязательно ли использовать ПИН-код на уровне приложения. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|maximumPinRetries|Int32|Максимальное количество неудачных попыток повторной попытки закрепления до блокировки или стирки управляемого приложения. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|simplePinBlocked|Boolean|Указывает, заблокирован ли простой ПИН-код. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumPinLength|Int32|Минимальная длина ПИН-кода на уровне приложения, если для параметра PinRequired установлено значение True. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|Разрешенный набор символов ПИН-кода на уровне приложения, если для параметра PinRequired установлено значение True. Наследуется [от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Duration|Время до сброса универсального ПИН-кода, если для параметра PinRequired установлено значение True. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedDataStorageLocations|[Коллекция managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)|Разрешенные места хранения управляемых данных. Наследуется [от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `oneDriveForBusiness`, `sharePoint`, `box`, `localStorage`.|
|contactSyncBlocked|Boolean|Указывает, можно ли синхронизировать контакты с устройством пользователя. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|printBlocked|Boolean|Указывает, разрешена ли печать из управляемых приложений. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|fingerprintBlocked|Boolean|Указывает, можно ли использовать сканер отпечатков пальцев вместо ПИН-кода, если для параметра PinRequired установлено значение True. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|disableAppPinIfDevicePinIsSet|Boolean|Указывает, обязательно ли использовать ПИН-код приложения, если установлен ПИН-код устройства. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|maximumRequiredOsVersion|String|Версии, размером больше указанной версии, будут блокировать управляемому приложению доступ к данным компании. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|maximumWarningOsVersion|String|Версии, размером больше указанной версии, будут блокировать управляемому приложению доступ к данным компании. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|maximumWipeOsVersion|String|Версии, размером больше указанной версии, будут блокировать управляемому приложению доступ к данным компании. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumRequiredOsVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWarningOsVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение о невозможности получить доступ к данным компании. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumRequiredAppVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWarningAppVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWipeOsVersion|String|Версии, которые не равны указанной версии, будут стирать данные управляемого приложения и связанных с ним компаний. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWipeAppVersion|String|Версии, которые не равны указанной версии, будут стирать данные управляемого приложения и связанных с ним компаний. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения( блокировка или стирка), если устройство либо имеет корневой доступ, либо со стираемой блокировкой, если для DeviceComplianceRequired установлено true. Наследуется [от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `block`, `wipe`, `warn`.|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения ( блокировка или стирка) на основе максимального количества неудачных попыток повторной попытки закрепления. Наследуется [от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `block`, `wipe`, `warn`.|
|pinRequiredInsteadOfBiometricTimeout|Duration|Время в минутах для пин-кода приложения вместо биометрического пароля. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedOutboundClipboardSharingExceptionLength|Int32|Укажите количество символов, которые можно вырезать или скопировать из данных и учетных записей организации в любое приложение. Этот параметр переопределяет ограничение AllowedOutboundClipboardSharingLevel. Значение по умолчанию "0" означает, что исключение не разрешено. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|notificationRestriction|[managedAppNotificationRestriction](../resources/intune-mam-managedappnotificationrestriction.md)|Укажите ограничение уведомлений приложения. [Наследуется от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `allow`, `blockOrganizationalData`, `block`.|
|previousPinBlockCount|Int32|Требуется, чтобы pin-код был уникальным по номеру, указанному в этом свойстве. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|managedBrowser|[managedBrowserType](../resources/intune-mam-managedbrowsertype.md)|Указывает, в каких управляемых браузерах должны открываться интернет-ссылки. При настройке этого свойства свойство ManagedBrowserToOpenLinksRequired должно быть истинным. Наследуется [от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `notConfigured`, `microsoftEdge`.|
|maximumAllowedDeviceThreatLevel|[managedAppDeviceThreatLevel](../resources/intune-mam-managedappdevicethreatlevel.md)|Максимальный допустимый уровень угроз устройства, о чем сообщает приложение MTD. Наследуется от [managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `notConfigured`, `secured`, `low`, `medium`, `high`.|
|mobileThreatDefenseRemediationAction|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет, какое действие необходимо принять, если не превышен порог угроз для защиты от угроз для мобильных устройств. Предупреждение не поддерживается для этого свойства Inherited from [managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `block`, `wipe`, `warn`.|
|blockDataIngestionIntoOrganizationDocuments|Boolean|Указывает, может ли пользователь сводить данные в документы организации. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedDataIngestionLocations|[Коллекция managedAppDataIngestionLocation](../resources/intune-mam-managedappdataingestionlocation.md)|Разрешенные места хранения управляемых данных. Наследуется [от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `oneDriveForBusiness`, `sharePoint`, `camera`.|
|appActionIfUnableToAuthenticateUser|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Если этот маркер установлен, он указывает, какое действие необходимо принять в случае, если пользователь не может проверить подлинность, так как его маркер проверки подлинности недействителен. Это происходит, когда пользователь удаляется или отключается в AAD. Наследуется [от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `block`, `wipe`, `warn`.|
|dialerRestrictionLevel|[managedAppPhoneNumberRedirectLevel](../resources/intune-mam-managedappphonenumberredirectlevel.md)|Классы приложений для набора номера, которые могут открывать телефонный номер по щелчку. Наследуется [от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `allApps`, `managedApps`, `customApp`, `blocked`.|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune-mam-managedappdataencryptiontype.md)|Необходимый тип шифрования данных в управляемом приложении (Только для iOS). Возможные значения: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.|
|screenCaptureBlocked|Boolean|Указывает, заблокированы ли снимки экрана. (только для Android).|
|encryptAppData|Boolean|Указывает, следует ли шифровать данные управляемых приложений (только для Android).|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolean|Если этот параметр включен, шифрование на уровне приложения отключено, если включено шифрование на уровне устройства. (только для Android).|
|minimumRequiredSdkVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании. (Только для iOS)|
|customSettings|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Набор, состоящий из пар ключа и значения строки, которые отправляются затронутым пользователям в неизменном виде.|
|deployedAppCount|Int32|Количество приложений, к которым применена текущая политика.|
|minimumRequiredPatchVersion|String|Определите самый старый уровень обновления для системы безопасности Android, необходимый для безопасного доступа к приложению. (только для Android).|
|minimumWarningPatchVersion|String|Определите самый старый уровень обновления для системы безопасности Android, рекомендуемый для безопасного доступа к приложению. (только для Android).|
|exemptedAppProtocols|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Приложения iOS в этом списке будут исключены из политики и смогут получать данные из управляемых приложений. (Только для iOS)|
|exemptedAppPackages|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Пакеты приложений Android из этого списка будут исключены из политики и смогут получать данные из управляемых приложений. (только для Android).|
|faceIdBlocked|Boolean|Указывает, можно ли использовать FaceID вместо ПИН-кода, если для параметра PinRequired установлено значение True. (Только для iOS)|
|minimumWipeSdkVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании.|
|minimumWipePatchVersion|String|Уровень исправлений системы безопасности Android меньше или равен указанному значению, при этом управляемое приложение и связанные с ним данные компании будут стираться. (только для Android).|
|allowedIosDeviceModels|String|Разделенный с запамяти список моделей устройств, разрешенный в качестве строки для работы управляемого приложения. (Только для iOS)|
|appActionIfIosDeviceModelNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения ( блокировка или стирка), если указанная модель устройства не разрешена. (Только для iOS). Возможные значения: `block`, `wipe`, `warn`.|
|allowedAndroidDeviceManufacturers|String|Список изготовителей устройств с запамяти, разрешенный в качестве строки, чтобы управляемое приложение работало. (только для Android).|
|appActionIfAndroidDeviceManufacturerNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения ( блокировка или стирка), если указанный производитель устройства не разрешен. (только для Android). Возможные значения: `block`, `wipe`, `warn`.|
|thirdPartyKeyboardsBlocked|Boolean|Определяет, разрешены ли сторонние клавиатуры при доступе к управляемому приложению. (Только для iOS)|
|filterOpenInToOnlyManagedApps|Boolean|Определяет, поддерживается ли операция открытия из управляемого приложения в выбранные расположения для размещения файлов. Этот параметр применяется, только если параметр AllowedOutboundDataTransferDestinations имеет параметр ManagedApps, а параметр DisableProtectionOfManagedOutboundOpenInData — false. (Только для iOS)|
|disableProtectionOfManagedOutboundOpenInData|Boolean|Отключать защиту данных, перенесенных в другие приложения, с помощью параметра IOS OpenIn. Этот параметр может иметь true, только если для параметра AllowedOutboundDataTransferDestinations задан параметр ManagedApps. (Только для iOS)|
|protectInboundDataFromUnknownSources|Boolean|Защита входящих данных из неизвестного источника. Этот параметр может иметь значение True, только если для параметра AllowedInboundDataTransferSources установлено значение AllApps. (Только для iOS)|
|requiredAndroidSafetyNetDeviceAttestationType|[androidManagedAppSafetyNetDeviceAttestationType](../resources/intune-mam-androidmanagedappsafetynetdeviceattestationtype.md)|Определяет требование проверки безопасности устройств Android для работы управляемого приложения. Возможные значения: `none`, `basicIntegrity`, `basicIntegrityAndDeviceCertification`.|
|appActionIfAndroidSafetyNetDeviceAttestationFailed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения , предупреждающее или блокирование, если указанное предупреждение Android SafetyNet Attestation не удается. Возможные значения: `block`, `wipe`, `warn`.|
|requiredAndroidSafetyNetAppsVerificationType|[androidManagedAppSafetyNetAppsVerificationType](../resources/intune-mam-androidmanagedappsafetynetappsverificationtype.md)|Определяет требование проверки приложений SafetyNet для Android, чтобы управляемое приложение работало. Возможные значения: `none`, `enabled`.|
|appActionIfAndroidSafetyNetAppsVerificationFailed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения( предупреждать или блокировать), если указанное подтверждение для приложения Android не удается. Возможные значения: `block`, `wipe`, `warn`.|
|customBrowserProtocol|String|Настраиваемый протокол браузера для открытия веб-ссылки на iOS. (только для iOS)|
|customBrowserPackageId|String|Уникальный идентификатор настраиваемого браузера для открытия веб-ссылки на Android. (только для Android).|
|customBrowserDisplayName|String|Удобное имя предпочитаемого настраиваемого браузера для открытия веб-ссылки на Android. (только для Android).|
|minimumRequiredCompanyPortalVersion|String|Минимальная версия портала компании, которая должна быть установлена на устройстве или в приложении, будет заблокирована|
|minimumWarningCompanyPortalVersion|String|Минимальная версия портала компании, которая должна быть установлена на устройстве или пользователь получит предупреждение|
|minimumWipeCompanyPortalVersion|String|Минимальная версия портала компании, которая должна быть установлена на устройстве или данные компании в приложении, будет стираться|
|allowedAndroidDeviceModels|Коллекция String|Список моделей устройств, разрешенных в качестве строки для работы управляемого приложения. (Только для Android)|
|appActionIfAndroidDeviceModelNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения ( блокировка или стирка), если указанная модель устройства не разрешена. (Только для Android). Возможные значения: `block`, `wipe`, `warn`.|
|customDialerAppProtocol|String|Протокол пользовательского приложения для набора номера для открытия номера телефона в iOS, например skype:.|
|customDialerAppPackageId|String|PackageId настраиваемого приложения для набора номера для открытия номера телефона на Android.|
|customDialerAppDisplayName|String|Удобное имя настраиваемого приложения для набора номера телефона на Android.|
|biometricAuthenticationBlocked|Boolean|Указывает, разрешено ли использование биометрической проверки подлинности на месте пин-кода, если для Параметра PinRequired установлено true. (Только для Android)|
|requiredAndroidSafetyNetEvaluationType|[androidManagedAppSafetyNetEvaluationType](../resources/intune-mam-androidmanagedappsafetynetevaluationtype.md)|Определяет требования к типу оценки "Android SafetyNet", чтобы управляемое приложение работало. (Только для Android). Возможные значения: `basic`, `hardwareBacked`.|
|blockAfterCompanyPortalUpdateDeferralInDays|Int32|На устройстве может быть отложено обновление портала компании в течение максимального количества дней, иначе доступ к приложению будет заблокирован.|
|warnAfterCompanyPortalUpdateDeferralInDays|Int32|Максимальное количество дней, в течение которое обновление на портале компании может быть отложено на устройстве или пользователь получит предупреждение|
|wipeAfterCompanyPortalUpdateDeferralInDays|Int32|Максимальное количество дней отложенного обновления портала компании на устройстве или стирания данных компании в приложении|
|deviceLockRequired|Boolean|Определяет, требуется ли какая-либо блокировка на устройстве. (только android)|
|appActionIfDeviceLockNotSet|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения( предупреждать, блокировать или стирать, если блокировка экрана требуется на устройстве, но не настроена. (только android). Возможные значения: `block`, `wipe`, `warn`.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
Content-type: application/json
Content-length: 5308

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "maximumRequiredOsVersion": "Maximum Required Os Version value",
  "maximumWarningOsVersion": "Maximum Warning Os Version value",
  "maximumWipeOsVersion": "Maximum Wipe Os Version value",
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "appActionIfDeviceComplianceRequired": "wipe",
  "appActionIfMaximumPinRetriesExceeded": "wipe",
  "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
  "allowedOutboundClipboardSharingExceptionLength": 14,
  "notificationRestriction": "blockOrganizationalData",
  "previousPinBlockCount": 5,
  "managedBrowser": "microsoftEdge",
  "maximumAllowedDeviceThreatLevel": "secured",
  "mobileThreatDefenseRemediationAction": "wipe",
  "blockDataIngestionIntoOrganizationDocuments": true,
  "allowedDataIngestionLocations": [
    "sharePoint"
  ],
  "appActionIfUnableToAuthenticateUser": "wipe",
  "dialerRestrictionLevel": "managedApps",
  "appDataEncryptionType": "afterDeviceRestart",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "faceIdBlocked": true,
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true,
  "requiredAndroidSafetyNetDeviceAttestationType": "basicIntegrity",
  "appActionIfAndroidSafetyNetDeviceAttestationFailed": "wipe",
  "requiredAndroidSafetyNetAppsVerificationType": "enabled",
  "appActionIfAndroidSafetyNetAppsVerificationFailed": "wipe",
  "customBrowserProtocol": "Custom Browser Protocol value",
  "customBrowserPackageId": "Custom Browser Package Id value",
  "customBrowserDisplayName": "Custom Browser Display Name value",
  "minimumRequiredCompanyPortalVersion": "Minimum Required Company Portal Version value",
  "minimumWarningCompanyPortalVersion": "Minimum Warning Company Portal Version value",
  "minimumWipeCompanyPortalVersion": "Minimum Wipe Company Portal Version value",
  "allowedAndroidDeviceModels": [
    "Allowed Android Device Models value"
  ],
  "appActionIfAndroidDeviceModelNotAllowed": "wipe",
  "customDialerAppProtocol": "Custom Dialer App Protocol value",
  "customDialerAppPackageId": "Custom Dialer App Package Id value",
  "customDialerAppDisplayName": "Custom Dialer App Display Name value",
  "biometricAuthenticationBlocked": true,
  "requiredAndroidSafetyNetEvaluationType": "hardwareBacked",
  "blockAfterCompanyPortalUpdateDeferralInDays": 11,
  "warnAfterCompanyPortalUpdateDeferralInDays": 10,
  "wipeAfterCompanyPortalUpdateDeferralInDays": 10,
  "deviceLockRequired": true,
  "appActionIfDeviceLockNotSet": "wipe"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5480

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "77064c51-4c51-7706-514c-0677514c0677",
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "maximumRequiredOsVersion": "Maximum Required Os Version value",
  "maximumWarningOsVersion": "Maximum Warning Os Version value",
  "maximumWipeOsVersion": "Maximum Wipe Os Version value",
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "appActionIfDeviceComplianceRequired": "wipe",
  "appActionIfMaximumPinRetriesExceeded": "wipe",
  "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
  "allowedOutboundClipboardSharingExceptionLength": 14,
  "notificationRestriction": "blockOrganizationalData",
  "previousPinBlockCount": 5,
  "managedBrowser": "microsoftEdge",
  "maximumAllowedDeviceThreatLevel": "secured",
  "mobileThreatDefenseRemediationAction": "wipe",
  "blockDataIngestionIntoOrganizationDocuments": true,
  "allowedDataIngestionLocations": [
    "sharePoint"
  ],
  "appActionIfUnableToAuthenticateUser": "wipe",
  "dialerRestrictionLevel": "managedApps",
  "appDataEncryptionType": "afterDeviceRestart",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "faceIdBlocked": true,
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true,
  "requiredAndroidSafetyNetDeviceAttestationType": "basicIntegrity",
  "appActionIfAndroidSafetyNetDeviceAttestationFailed": "wipe",
  "requiredAndroidSafetyNetAppsVerificationType": "enabled",
  "appActionIfAndroidSafetyNetAppsVerificationFailed": "wipe",
  "customBrowserProtocol": "Custom Browser Protocol value",
  "customBrowserPackageId": "Custom Browser Package Id value",
  "customBrowserDisplayName": "Custom Browser Display Name value",
  "minimumRequiredCompanyPortalVersion": "Minimum Required Company Portal Version value",
  "minimumWarningCompanyPortalVersion": "Minimum Warning Company Portal Version value",
  "minimumWipeCompanyPortalVersion": "Minimum Wipe Company Portal Version value",
  "allowedAndroidDeviceModels": [
    "Allowed Android Device Models value"
  ],
  "appActionIfAndroidDeviceModelNotAllowed": "wipe",
  "customDialerAppProtocol": "Custom Dialer App Protocol value",
  "customDialerAppPackageId": "Custom Dialer App Package Id value",
  "customDialerAppDisplayName": "Custom Dialer App Display Name value",
  "biometricAuthenticationBlocked": true,
  "requiredAndroidSafetyNetEvaluationType": "hardwareBacked",
  "blockAfterCompanyPortalUpdateDeferralInDays": 11,
  "warnAfterCompanyPortalUpdateDeferralInDays": 10,
  "wipeAfterCompanyPortalUpdateDeferralInDays": 10,
  "deviceLockRequired": true,
  "appActionIfDeviceLockNotSet": "wipe"
}
```




