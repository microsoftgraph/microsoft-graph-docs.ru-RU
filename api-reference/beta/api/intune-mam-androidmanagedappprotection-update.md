---
title: >
  Обновление androidManagedAppProtection
description: Обновление свойств объекта androidManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a9382d7ff13860db626acca32a23e6602b54ae58
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157479"
---
# <a name="update-androidmanagedappprotection"></a>Обновление androidManagedAppProtection


> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).

## <a name="prerequisites"></a>Необходимые разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) в формате JSON.

В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|description|String|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|id|String|Ключ объекта. Унаследовано от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|Строка|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|periodOfflineBeforeAccessCheck|Длительность|Время до проверки доступа, когда устройство не подключено к Интернету. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|periodOnlineBeforeAccessCheck|Продолжительность|Время до проверки доступа, когда устройство подключено к Интернету. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedInboundDataTransferSources|[Манажедаппдататрансферлевел](../resources/intune-mam-managedappdatatransferlevel.md)|Источники, из которых разрешена передача данных. НаСледуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|[Манажедаппдататрансферлевел](../resources/intune-mam-managedappdatatransferlevel.md)|Расположения, в которые разрешено передавать данные. НаСледуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Логический|Указывает, необходимы ли для использования приложения учетные данные организации. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedOutboundClipboardSharingLevel|[Манажедаппклипбоардшаринглевел](../resources/intune-mam-managedappclipboardsharinglevel.md)|Разрешенный уровень совместного использования буфера обмена для приложений на управляемом устройстве. НаСледуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Логический|Указывает, заблокировано ли резервное копирование данных управляемого приложения. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|deviceComplianceRequired|Логический|Указывает, обязательно ли соответствие устройства требованиям. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|managedBrowserToOpenLinksRequired|Логический|Указывает, следует ли открывать интернет-ссылки в управляемом браузере. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|saveAsBlocked|Boolean|Указывает, могут ли пользователи сохранять копии защищенных файлов, используя пункт меню "Сохранить как". Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|periodOfflineBeforeWipeIsEnforced|Длительность|Время до удаления всех управляемых данных после отключения приложения от Интернета. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|pinRequired|Логический|Указывает, обязательно ли использовать ПИН-код на уровне приложения. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|maximumPinRetries|Int32|Максимальное количество неудачных попыток ввода ПИН-кода перед блокированием или очисткой управляемого приложения. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|simplePinBlocked|Логический|Указывает, заблокирован ли простой ПИН-код. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumPinLength|Int32|Минимальная длина ПИН-кода на уровне приложения, если для параметра PinRequired задано значение True. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|pinCharacterSet|[Манажедапппинчарактерсет](../resources/intune-mam-managedapppincharacterset.md)|Разрешенный набор символов ПИН-кода на уровне приложения, если для параметра PinRequired задано значение True. НаСледуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Продолжительность|Время до сброса универсального ПИН-кода, если для параметра PinRequired задано значение True. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedDataStorageLocations|Коллекция [манажедаппдатасторажелокатион](../resources/intune-mam-managedappdatastoragelocation.md)|Разрешенные места хранения управляемых данных. НаСледуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `oneDriveForBusiness`, `sharePoint`, `localStorage`.|
|contactSyncBlocked|Логический|Указывает, можно ли синхронизировать контакты с устройством пользователя. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|printBlocked|Логический|Указывает, разрешена ли печать из управляемых приложений. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|fingerprintBlocked|Логический|Указывает, можно ли использовать сканер отпечатков пальцев вместо ПИН-кода, если для параметра PinRequired задано значение True. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|disableAppPinIfDevicePinIsSet|Логический|Указывает, обязательно ли использовать ПИН-код приложения, если задан ПИН-код устройства. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumRequiredOsVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWarningOsVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение о доступе к данным компании. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumRequiredAppVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWarningAppVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|Минимумвипеосверсион|String|Версии, меньшие или равные указанной версии, будут очищать управляемое приложение и связанные данные компании. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|Минимумвипеаппверсион|String|Версии, меньшие или равные указанной версии, будут очищать управляемое приложение и связанные данные компании. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|Аппактионифдевицекомплианцерекуиред|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения (блокировка или очистка), когда устройство находится в корневом режиме или с защитой от удаления, если для Девицекомплианцерекуиред задано значение true. НаСледуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `block`, `wipe`, `warn`.|
|Аппактионифмаксимумпинретриесексцеедед|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения (блокировка или очистка) на основе максимального количества неудачных попыток ввода ПИН-кода. НаСледуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `block`, `wipe`, `warn`.|
|Пинрекуирединстеадофбиометриктимеаут|Длительность|Время ожидания ПИН-кода приложения (в минутах), а не биометрического кода, унаследованного от [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|isAssigned|Логический|Указывает, применена ли политика к группам включения. Наследуется от [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).|
|Таржетедаппманажементлевелс|[Аппманажементлевел](../resources/intune-mam-appmanagementlevel.md)|Предполагаемые уровни управления приложениями для этой политики наСледуются от [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md). Возможные значения: `unspecified`, `unmanaged`, `mdm`, `androidEnterprise`.|
|screenCaptureBlocked|Boolean|Указывает, может ли управляемый пользователь делать снимки экрана управляемых приложений.|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolean|Если этот параметр включен, шифрование на уровне приложения отключается, если включено шифрование на уровне устройства.|
|encryptAppData|Boolean|Указывает, следует ли шифровать данные управляемых приложений.|
|deployedAppCount|Int32|Количество приложений, к которым применена текущая политика.|
|minimumRequiredPatchVersion|String|Определите самый старый уровень обновления для системы безопасности Android, необходимый для безопасного доступа к приложению.|
|minimumWarningPatchVersion|String|Определите самый старый уровень обновления для системы безопасности Android, рекомендуемый для безопасного доступа к приложению.|
|exemptedAppPackages|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Пакеты приложений из этого списка не будут исключены из политики и смогут получать данные из управляемых приложений.|
|Минимумвипепатчверсион|String|Уровень обновления для системы безопасности Android, меньший или равный указанному значению, приведет к очистке управляемого приложения и связанных данных компании.|
|allowedAndroidDeviceManufacturers|String|Разделенный список производителей устройств с точкой с запятой, разрешенный для работы управляемого приложения в виде строки.|
|appActionIfAndroidDeviceManufacturerNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения (блокировка или очистка, если заданный изготовителем устройства не разрешено). Возможные значения: `block`, `wipe`, `warn`.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
Content-type: application/json
Content-length: 2460

{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
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
  "isAssigned": true,
  "targetedAppManagementLevels": "unmanaged",
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe"
}
```

### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2632

{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "cf517ced-7ced-cf51-ed7c-51cfed7c51cf",
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
  "isAssigned": true,
  "targetedAppManagementLevels": "unmanaged",
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe"
}
```




