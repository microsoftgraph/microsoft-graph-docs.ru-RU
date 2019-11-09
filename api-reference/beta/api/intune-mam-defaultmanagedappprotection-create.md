---
title: Создание объекта defaultManagedAppProtection
description: Создает объект defaultManagedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 654ce664e1e22ac870948c9375293afa96491e28
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086902"
---
# <a name="create-defaultmanagedappprotection"></a>Создание объекта defaultManagedAppProtection

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создает объект [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).

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
POST /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса добавьте представление объекта defaultManagedAppProtection в формате JSON.

Ниже показаны свойства, которые необходимо указывать при создании объекта defaultManagedAppProtection.

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|description|String|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|roleScopeTagIds|Коллекция String|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|id|String|Ключ объекта. Унаследовано от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|String|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|periodOfflineBeforeAccessCheck|Длительность|Время до проверки доступа, когда устройство не подключено к Интернету. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|periodOnlineBeforeAccessCheck|Длительность|Время до проверки доступа, когда устройство подключено к Интернету. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedInboundDataTransferSources|[манажедаппдататрансферлевел](../resources/intune-mam-managedappdatatransferlevel.md)|Источники, из которых разрешена передача данных. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|[манажедаппдататрансферлевел](../resources/intune-mam-managedappdatatransferlevel.md)|Назначения, в которые разрешена передача данных. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Логический|Указывает, необходимы ли для использования приложения учетные данные организации. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedOutboundClipboardSharingLevel|[манажедаппклипбоардшаринглевел](../resources/intune-mam-managedappclipboardsharinglevel.md)|Разрешенный уровень совместного использования буфера обмена для приложений на управляемом устройстве. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Логический|Указывает, заблокировано ли резервное копирование данных управляемого приложения. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|deviceComplianceRequired|Логический|Указывает, обязательно ли соответствие устройства требованиям. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|managedBrowserToOpenLinksRequired|Логический|Указывает, следует ли открывать интернет-ссылки в управляемом браузере. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|saveAsBlocked|Логический|Указывает, могут ли пользователи сохранять копии защищенных файлов, используя пункт меню "Сохранить как". Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|periodOfflineBeforeWipeIsEnforced|Duration|Время до удаления всех управляемых данных после отключения приложения от Интернета. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|pinRequired|Логический|Указывает, обязательно ли использовать ПИН-код на уровне приложения. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|maximumPinRetries|Int32|Максимальное количество неудачных попыток ввода ПИН-кода перед блокированием или очисткой управляемого приложения. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|simplePinBlocked|Boolean|Указывает, заблокирован ли простой ПИН-код. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumPinLength|Int32|Минимальная длина ПИН-кода на уровне приложения, если для параметра PinRequired установлено значение True. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|pinCharacterSet|[манажедапппинчарактерсет](../resources/intune-mam-managedapppincharacterset.md)|Разрешенный набор символов ПИН-кода на уровне приложения, если для параметра PinRequired установлено значение True. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Duration|Время до сброса универсального ПИН-кода, если для параметра PinRequired установлено значение True. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedDataStorageLocations|Коллекция [манажедаппдатасторажелокатион](../resources/intune-mam-managedappdatastoragelocation.md)|Разрешенные места хранения управляемых данных. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `oneDriveForBusiness`, `sharePoint`, `localStorage`.|
|contactSyncBlocked|Логический|Указывает, можно ли синхронизировать контакты с устройством пользователя. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|printBlocked|Логический|Указывает, разрешена ли печать из управляемых приложений. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|fingerprintBlocked|Логический|Указывает, можно ли использовать сканер отпечатков пальцев вместо ПИН-кода, если для параметра PinRequired установлено значение True. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|disableAppPinIfDevicePinIsSet|Boolean|Указывает, обязательно ли использовать ПИН-код приложения, если установлен ПИН-код устройства. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumRequiredOsVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWarningOsVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение о невозможности получить доступ к данным компании. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumRequiredAppVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWarningAppVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|минимумвипеосверсион|String|Версии, меньшие или равные указанной версии, будут очищать управляемое приложение и связанные данные компании. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|минимумвипеаппверсион|String|Версии, меньшие или равные указанной версии, будут очищать управляемое приложение и связанные данные компании. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|аппактионифдевицекомплианцерекуиред|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения (блокировка или очистка), когда устройство находится в корневом режиме или с защитой от удаления, если для Девицекомплианцерекуиред задано значение true. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `block`, `wipe`, `warn`.|
|аппактионифмаксимумпинретриесексцеедед|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения (блокировка или очистка) на основе максимального количества неудачных попыток ввода ПИН-кода. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `block`, `wipe`, `warn`.|
|пинрекуирединстеадофбиометриктимеаут|Длительность|Время ожидания ПИН-кода приложения (в минутах), а не биометрического кода, унаследованного от [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|алловедаутбаундклипбоардшаринжексцептионленгс|Int32|Укажите количество символов, которое может быть вырезано или скопировано из данных Организации и учетных записей в любое приложение. Этот параметр переопределяет ограничение Алловедаутбаундклипбоардшаринглевел. Значение по умолчанию "0" означает, что исключение не разрешено. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|нотификатионрестриктион|[managedAppNotificationRestriction](../resources/intune-mam-managedappnotificationrestriction.md)|Укажите ограничение уведомления приложения, унаследованное от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `allow`, `blockOrganizationalData`, `block`.|
|превиауспинблокккаунт|Int32|Требует уникальности ПИН-кода на основе числа, указанного в этом свойстве. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|манажедбровсер|[манажедбровсертипе](../resources/intune-mam-managedbrowsertype.md)|Указывает, в каких управляемых браузерах следует открывать Интернет-ссылки. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `notConfigured`, `microsoftEdge`.|
|максимумалловеддевицесреатлевел|[managedAppDeviceThreatLevel](../resources/intune-mam-managedappdevicethreatlevel.md)|Максимально допустимый уровень угроз для устройства, как это было сообщено приложением МТД, унаследованным из [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `notConfigured`, `secured`, `low`, `medium`, `high`.|
|мобилесреатдефенсеремедиатионактион|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет, какое действие необходимо предпринять, если не достигнут порог угроз для защиты от угроз для мобильных устройств. Предупреждение не является поддерживаемым значением для этого свойства, наследуемого из [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `block`, `wipe`, `warn`.|
|appDataEncryptionType|[манажедаппдатаенкриптионтипе](../resources/intune-mam-managedappdataencryptiontype.md)|Необходимый тип шифрования данных в управляемом приложении (только для iOS). Возможные значения: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.|
|screenCaptureBlocked|Boolean|Указывает, заблокированы ли снимки экрана. (только для Android).|
|encryptAppData|Логический|Указывает, следует ли шифровать данные управляемых приложений (только для Android).|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Логический|Если этот параметр включен, шифрование на уровне приложения отключается, если включено шифрование на уровне устройства. (только для Android).|
|minimumRequiredSdkVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании. (только для iOS)|
|customSettings|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Набор, состоящий из пар ключа и значения строки, которые отправляются затронутым пользователям в неизменном виде.|
|deployedAppCount|Int32|Количество приложений, к которым применена текущая политика.|
|minimumRequiredPatchVersion|String|Определите самый старый уровень обновления для системы безопасности Android, необходимый для безопасного доступа к приложению. (только для Android).|
|minimumWarningPatchVersion|String|Определите самый старый уровень обновления для системы безопасности Android, рекомендуемый для безопасного доступа к приложению. (только для Android).|
|exemptedAppProtocols|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Приложения для iOS из этого списка не будут исключаться из политики и смогут получать данные из управляемых приложений. (только для iOS)|
|exemptedAppPackages|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Пакеты приложений Android из этого списка не будут исключены из политики и смогут получать данные из управляемых приложений. (только для Android).|
|faceIdBlocked|Boolean|Указывает, можно ли использовать FaceID вместо ПИН-кода, если для параметра PinRequired установлено значение True. (только для iOS)|
|Свойства minimumwipesdkversion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании.|
|минимумвипепатчверсион|String|Уровень обновления для системы безопасности Android, меньший или равный указанному значению, приведет к очистке управляемого приложения и связанных данных компании. (только для Android).|
|allowedIosDeviceModels|String|Разделенный на точку с запятой список моделей устройств, допустимых в виде строки, для работы управляемого приложения. (только для iOS)|
|appActionIfIosDeviceModelNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения: блок или очистка, если указанная модель устройства не разрешена. (только для iOS). Возможные значения: `block`, `wipe`, `warn`.|
|allowedAndroidDeviceManufacturers|String|Разделенный список производителей устройств с точкой с запятой, разрешенный для работы управляемого приложения в виде строки. (только для Android).|
|appActionIfAndroidDeviceManufacturerNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения (блокировка или очистка, если заданный изготовителем устройства не разрешено). (Только для Android). Возможные значения: `block`, `wipe`, `warn`.|
|Свойства thirdpartykeyboardsblocked|Логический|Определяет, разрешены ли клавиатуры сторонних производителей при доступе к управляемому приложению. (только для iOS)|
|filterOpenInToOnlyManagedApps|Логический|Определяет, поддерживается ли операция открытия в управляемом приложении для выбранных расположений филешаринг. Этот параметр применяется только в том случае, если для Алловедаутбаунддататрансфердестинатионс задано значение Манажедаппс, а для свойства свойства disableprotectionofmanagedoutboundopenindata задано значение false. (только для iOS)|
|Свойства disableprotectionofmanagedoutboundopenindata|Логический|Отключить защиту данных, передаваемых в другие приложения с помощью функции IOS Open in. Этот параметр может иметь значение true, только если для параметра Алловедаутбаунддататрансфердестинатионс задано значение Манажедаппс. (только для iOS)|
|protectInboundDataFromUnknownSources|Логический|Защита входящих данных из неизвестного источника. Этот параметр может иметь значение true, только если для параметра Алловединбаунддататрансферсаурцес задано значение Аллаппс. (только для iOS)|
|рекуиредандроидсафетинетдевицеаттестатионтипе|[androidManagedAppSafetyNetDeviceAttestationType](../resources/intune-mam-androidmanagedappsafetynetdeviceattestationtype.md)|Определяет требование к аттестации устройств Android SafetyNet для работы управляемого приложения. Возможные значения: `none`, `basicIntegrity`, `basicIntegrityAndDeviceCertification`.|
|аппактионифандроидсафетинетдевицеаттестатионфаилед|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения (предупреждение или блокируется, если заданное рекуирмент аттестации SafetyNet для Android завершается с ошибкой). Возможные значения: `block`, `wipe`, `warn`.|
|рекуиредандроидсафетинетаппсверификатионтипе|[androidManagedAppSafetyNetAppsVerificationType](../resources/intune-mam-androidmanagedappsafetynetappsverificationtype.md)|Определяет требования к проверке приложений Android SafetyNet для работы управляемого приложения. Возможные значения: `none`, `enabled`.|
|аппактионифандроидсафетинетаппсверификатионфаилед|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения: либо warn, либо Block, если заданное приложение проверки приложений Android рекуирмент завершается с ошибкой. Возможные значения: `block`, `wipe`, `warn`.|
|кустомбровсерпротокол|String|Настраиваемый протокол браузера для открытия Weblink на iOS. (только для iOS)|
|кустомбровсерпаккажеид|String|Уникальный идентификатор настраиваемого браузера для открытия Weblink на Android. (только для Android).|
|кустомбровсердисплайнаме|String|Понятное имя предпочтительного настраиваемого браузера для открытия Weblink на Android. (только для Android).|
|минимумрекуиредкомпанипорталверсион|String|Минимальная версия корпоративного портала, которая должна быть установлена на устройстве или в доступе к приложениям, будет заблокирована|
|минимумварнингкомпанипорталверсион|String|Минимальная версия корпоративного портала, который должен быть установлен на устройстве, или пользователь будет получать предупреждение|
|минимумвипекомпанипорталверсион|String|Будет стерта минимальная версия корпоративного портала, который должен быть установлен на устройстве или данные компании в приложении.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections
Content-type: application/json
Content-length: 4217

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
  "minimumWipeCompanyPortalVersion": "Minimum Wipe Company Portal Version value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4389

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
  "minimumWipeCompanyPortalVersion": "Minimum Wipe Company Portal Version value"
}
```






