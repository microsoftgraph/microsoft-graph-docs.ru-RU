---
title: Тип ресурса defaultManagedAppProtection
description: Политика, используемая для настройки расширенных параметров управления для определенного набора приложений для всех пользователей, к которым не применяется политика TargetedManagedAppProtection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 627ab8f1bc0740fc8799503549aa6344d15b2139
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157591"
---
# <a name="defaultmanagedappprotection-resource-type"></a>Тип ресурса defaultManagedAppProtection

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политика, используемая для настройки расширенных параметров управления для определенного набора приложений для всех пользователей, к которым не применяется политика TargetedManagedAppProtection


Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов DefaultManagedAppProtection](../api/intune-mam-defaultmanagedappprotection-list.md)|Коллекция [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|Перечисление свойств и связей объектов [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).|
|[Получение объекта defaultManagedAppProtection](../api/intune-mam-defaultmanagedappprotection-get.md)|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|Чтение свойств и связей объекта [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).|
|[Создание объекта defaultManagedAppProtection](../api/intune-mam-defaultmanagedappprotection-create.md)|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|Создание объекта [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).|
|[Удаление объекта defaultManagedAppProtection](../api/intune-mam-defaultmanagedappprotection-delete.md)|Нет|Удаление объекта [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).|
|[Обновление объекта defaultManagedAppProtection](../api/intune-mam-defaultmanagedappprotection-update.md)|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|Обновление свойств объекта [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).|

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
|periodOfflineBeforeAccessCheck|Duration|Время до проверки доступа, когда устройство не подключено к Интернету. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|periodOnlineBeforeAccessCheck|Duration|Время до проверки доступа, когда устройство подключено к Интернету. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Источники, из которых разрешена передача данных. Наследуется [от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Назначения, в которые разрешена передача данных. Наследуется [от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Boolean|Указывает, необходимы ли для использования приложения учетные данные организации. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|Разрешенный уровень совместного использования буфера обмена для приложений на управляемом устройстве. Наследуется [от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolean|Указывает, заблокировано ли резервное копирование данных управляемого приложения. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|deviceComplianceRequired|Boolean|Указывает, обязательно ли соответствие устройства требованиям. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|managedBrowserToOpenLinksRequired|Boolean|Указывает, следует ли открывать интернет-ссылки в управляемом браузере или любой настраиваемый браузер, указанный customBrowserProtocol (для iOS) или CustomBrowserPackageId/CustomBrowserDisplayName (для Android), унаследованный от [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|saveAsBlocked|Boolean|Указывает, могут ли пользователи сохранять копии защищенных файлов, используя пункт меню "Сохранить как". Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|periodOfflineBeforeWipeIsEnforced|Duration|Время до удаления всех управляемых данных после отключения приложения от Интернета. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|pinRequired|Boolean|Указывает, обязательно ли использовать ПИН-код на уровне приложения. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|maximumPinRetries|Int32|Максимальное количество неудачных попыток повторной попытки закрепления до блокировки или стирки управляемого приложения. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|simplePinBlocked|Boolean|Указывает, заблокирован ли простой ПИН-код. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumPinLength|Int32|Минимальная длина ПИН-кода на уровне приложения, если для параметра PinRequired установлено значение True. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|Разрешенный набор символов ПИН-кода на уровне приложения, если для параметра PinRequired установлено значение True. Наследуется [от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Duration|Время до сброса универсального ПИН-кода, если для параметра PinRequired установлено значение True. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedDataStorageLocations|[Коллекция managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)|Разрешенные места хранения управляемых данных. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
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
|minimumWipeOsVersion|String|Версии, не равные указанной версии, будут стирать данные управляемого приложения и связанных с ним компаний. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWipeAppVersion|String|Версии, которые не равны указанной версии, будут стирать данные управляемого приложения и связанных с ним компаний. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения( блокировка или стирка), когда устройство либо имеет корневой доступ, либо со схваченной блокировкой, если для DeviceComplianceRequired установлено true. Наследуется [от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `block`, `wipe`, `warn`.|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения ( блокировка или стирка) на основе максимального количества неудачных попыток повторной попытки закрепления. Наследуется [от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `block`, `wipe`, `warn`.|
|pinRequiredInsteadOfBiometricTimeout|Duration|Время в минутах для пин-кода приложения вместо биометрического пароля. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedOutboundClipboardSharingExceptionLength|Int32|Укажите количество символов, которые можно вырезать или скопировать из данных и учетных записей организации в любое приложение. Этот параметр переопределяет ограничение AllowedOutboundClipboardSharingLevel. Значение по умолчанию "0" означает, что исключения не разрешены. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|notificationRestriction|[managedAppNotificationRestriction](../resources/intune-mam-managedappnotificationrestriction.md)|Укажите ограничение уведомлений приложения. [Наследуется от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `allow`, `blockOrganizationalData`, `block`.|
|previousPinBlockCount|Int32|Требуется, чтобы pin-код был уникальным по номеру, указанному в этом свойстве. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|managedBrowser|[managedBrowserType](../resources/intune-mam-managedbrowsertype.md)|Указывает, в каких управляемых браузерах должны открываться интернет-ссылки. При настройке этого свойства свойство ManagedBrowserToOpenLinksRequired должно иметь true. Наследуется [от managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `notConfigured`, `microsoftEdge`.|
|maximumAllowedDeviceThreatLevel|[managedAppDeviceThreatLevel](../resources/intune-mam-managedappdevicethreatlevel.md)|Максимальный допустимый уровень угроз устройства, о чем сообщает приложение MTD. Наследуется от [managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `notConfigured`, `secured`, `low`, `medium`, `high`.|
|mobileThreatDefenseRemediationAction|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет, какое действие необходимо принять, если не превышен порог угроз для защиты от угроз для мобильных устройств. Warn не поддерживает значение для этого свойства Inherited from [managedAppProtection.](../resources/intune-mam-managedappprotection.md) Возможные значения: `block`, `wipe`, `warn`.|
|blockDataIngestionIntoOrganizationDocuments|Boolean|Указывает, может ли пользователь вводить данные в документы организации. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedDataIngestionLocations|[Коллекция managedAppDataIngestionLocation](../resources/intune-mam-managedappdataingestionlocation.md)|Разрешенные места хранения управляемых данных. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
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
|allowedAndroidDeviceManufacturers|String|Список производителей устройств с запамятий, разрешенных в качестве строки, чтобы управляемое приложение работало. (только для Android).|
|appActionIfAndroidDeviceManufacturerNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения , блок или стирать, если указанный производитель устройства не разрешен. (только для Android). Возможные значения: `block`, `wipe`, `warn`.|
|thirdPartyKeyboardsBlocked|Boolean|Определяет, разрешены ли сторонние клавиатуры при доступе к управляемому приложению. (Только для iOS)|
|filterOpenInToOnlyManagedApps|Boolean|Определяет, поддерживается ли операция открытия из управляемого приложения в выбранные расположения для открытия файлов. Этот параметр применяется, только если параметр AllowedOutboundDataTransferDestinations имеет параметр ManagedApps, а параметр DisableProtectionOfManagedOutboundOpenInData — false. (Только для iOS)|
|disableProtectionOfManagedOutboundOpenInData|Boolean|Отключать защиту данных, перенесенных в другие приложения, с помощью параметра IOS OpenIn. Этот параметр может иметь true, только если для параметра AllowedOutboundDataTransferDestinations заданы параметры ManagedApps. (Только для iOS)|
|protectInboundDataFromUnknownSources|Boolean|Защита входящих данных из неизвестного источника. Этот параметр может иметь значение True, только если для параметра AllowedInboundDataTransferSources установлено значение AllApps. (Только для iOS)|
|requiredAndroidSafetyNetDeviceAttestationType|[androidManagedAppSafetyNetDeviceAttestationType](../resources/intune-mam-androidmanagedappsafetynetdeviceattestationtype.md)|Определяет требование проверки безопасности устройств Android для работы управляемого приложения. Возможные значения: `none`, `basicIntegrity`, `basicIntegrityAndDeviceCertification`.|
|appActionIfAndroidSafetyNetDeviceAttestationFailed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения , предупреждающее или блокирование, если указанное предупреждение Android SafetyNet Attestation не удастся. Возможные значения: `block`, `wipe`, `warn`.|
|requiredAndroidSafetyNetAppsVerificationType|[androidManagedAppSafetyNetAppsVerificationType](../resources/intune-mam-androidmanagedappsafetynetappsverificationtype.md)|Определяет требование проверки приложений SafetyNet для Android, чтобы управляемое приложение работало. Возможные значения: `none`, `enabled`.|
|appActionIfAndroidSafetyNetAppsVerificationFailed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения, предупреждающее или блокируют, если указанное подтверждение для приложения Android не удается получить. Возможные значения: `block`, `wipe`, `warn`.|
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
|blockAfterCompanyPortalUpdateDeferralInDays|Int32|Максимальное количество дней, в течение которое обновление на портале компании может быть отложено на устройстве, или доступ к приложению будет заблокирован.|
|warnAfterCompanyPortalUpdateDeferralInDays|Int32|Максимальное количество дней, в течение которое обновление на портале компании может быть отложено на устройстве или пользователь получит предупреждение|
|wipeAfterCompanyPortalUpdateDeferralInDays|Int32|Максимальное количество дней отложенного обновления портала компании на устройстве или стирания данных компании в приложении|
|deviceLockRequired|Boolean|Определяет, требуется ли какая-либо блокировка на устройстве. (только android)|
|appActionIfDeviceLockNotSet|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения( предупреждать, блокировать или стирать, если блокировка экрана требуется на устройстве, но не настроена. (только android). Возможные значения: `block`, `wipe`, `warn`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|apps|Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Список приложений, к которым применена политика.|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|Свойства навигации к сводке по развертыванию конфигурации.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
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
  "dialerRestrictionLevel": "String",
  "appDataEncryptionType": "String",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "deployedAppCount": 1024,
  "minimumRequiredPatchVersion": "String",
  "minimumWarningPatchVersion": "String",
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "faceIdBlocked": true,
  "minimumWipeSdkVersion": "String",
  "minimumWipePatchVersion": "String",
  "allowedIosDeviceModels": "String",
  "appActionIfIosDeviceModelNotAllowed": "String",
  "allowedAndroidDeviceManufacturers": "String",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "String",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true,
  "requiredAndroidSafetyNetDeviceAttestationType": "String",
  "appActionIfAndroidSafetyNetDeviceAttestationFailed": "String",
  "requiredAndroidSafetyNetAppsVerificationType": "String",
  "appActionIfAndroidSafetyNetAppsVerificationFailed": "String",
  "customBrowserProtocol": "String",
  "customBrowserPackageId": "String",
  "customBrowserDisplayName": "String",
  "minimumRequiredCompanyPortalVersion": "String",
  "minimumWarningCompanyPortalVersion": "String",
  "minimumWipeCompanyPortalVersion": "String",
  "allowedAndroidDeviceModels": [
    "String"
  ],
  "appActionIfAndroidDeviceModelNotAllowed": "String",
  "customDialerAppProtocol": "String",
  "customDialerAppPackageId": "String",
  "customDialerAppDisplayName": "String",
  "biometricAuthenticationBlocked": true,
  "requiredAndroidSafetyNetEvaluationType": "String",
  "blockAfterCompanyPortalUpdateDeferralInDays": 1024,
  "warnAfterCompanyPortalUpdateDeferralInDays": 1024,
  "wipeAfterCompanyPortalUpdateDeferralInDays": 1024,
  "deviceLockRequired": true,
  "appActionIfDeviceLockNotSet": "String"
}
```




