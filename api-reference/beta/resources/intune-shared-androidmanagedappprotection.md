---
title: Тип ресурса androidManagedAppProtection
description: Политика, используемая для настройки расширенных параметров управления для определенных групп безопасности и определенного набора приложений на устройстве Android
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6298b24fb5d0dffef0b1381eb18e599e723fa639
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439951"
---
# <a name="androidmanagedappprotection-resource-type"></a>Тип ресурса androidManagedAppProtection

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политика, используемая для настройки расширенных параметров управления для определенных групп безопасности и определенного набора приложений на устройстве Android


Наследуется от [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов AndroidManagedAppProtection](../api/intune-shared-androidmanagedappprotection-list.md)|Коллекция [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md)|Перечисление свойств и связей объектов [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md).|
|[Получение объекта androidManagedAppProtection](../api/intune-shared-androidmanagedappprotection-get.md)|[androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md)|Чтение свойств и связей объекта [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md).|
|[Создание объекта androidManagedAppProtection](../api/intune-shared-androidmanagedappprotection-create.md)|[androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md)|Создание объекта [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md).|
|[Удаление объекта androidManagedAppProtection](../api/intune-shared-androidmanagedappprotection-delete.md)|Нет|Удаление объекта [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md).|
|[Обновление объекта androidManagedAppProtection](../api/intune-shared-androidmanagedappprotection-update.md)|[androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md)|Обновление свойств объекта [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md).|
|**Набор политик**|
|[Действие hasPayloadLinks](../api/intune-shared-androidmanagedappprotection-haspayloadlinks.md)|[Коллекция hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|displayName|Строка|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|description|Строка|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|Идентификаторы roleScopeTagId|Коллекция строк|Список тегов области для этого экземпляра сущности. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|version|String|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|periodOfflineBeforeAccessCheck|Duration|Время до проверки доступа, когда устройство не подключено к Интернету. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|periodOnlineBeforeAccessCheck|Duration|Время до проверки доступа, когда устройство подключено к Интернету. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Источники, из которых разрешена передача данных. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Назначения, в которые разрешена передача данных. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Boolean|Указывает, необходимы ли для использования приложения учетные данные организации. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|Разрешенный уровень совместного использования буфера обмена для приложений на управляемом устройстве. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolean|Указывает, заблокировано ли резервное копирование данных управляемого приложения. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|deviceComplianceRequired|Boolean|Указывает, обязательно ли соответствие устройства требованиям. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|managedBrowserToOpenLinksRequired|Boolean|Указывает, следует ли открывать интернет-ссылки в управляемом браузере. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|saveAsBlocked|Boolean|Указывает, могут ли пользователи сохранять копии защищенных файлов, используя пункт меню "Сохранить как". Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|periodOfflineBeforeWipeIsEnforced|Duration|Время до удаления всех управляемых данных после отключения приложения от Интернета. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|pinRequired|Boolean|Указывает, обязательно ли использовать ПИН-код на уровне приложения. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|maximumPinRetries|Int32|Максимальное число попыток повторного закрепления перед блокировкой или очисткой управляемого приложения. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|simplePinBlocked|Boolean|Указывает, заблокирован ли простой ПИН-код. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumPinLength|Int32|Минимальная длина ПИН-кода на уровне приложения, если для параметра PinRequired установлено значение True. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|Разрешенный набор символов ПИН-кода на уровне приложения, если для параметра PinRequired установлено значение True. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Duration|Время до сброса универсального ПИН-кода, если для параметра PinRequired установлено значение True. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedDataStorageLocations|[Коллекция managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)|Разрешенные места хранения управляемых данных. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|contactSyncBlocked|Boolean|Указывает, можно ли синхронизировать контакты с устройством пользователя. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|printBlocked|Boolean|Указывает, разрешена ли печать из управляемых приложений. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|fingerprintBlocked|Boolean|Указывает, можно ли использовать сканер отпечатков пальцев вместо ПИН-кода, если для параметра PinRequired установлено значение True. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|disableAppPinIfDevicePinIsSet|Boolean|Указывает, обязательно ли использовать ПИН-код приложения, если установлен ПИН-код устройства. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumRequiredOsVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWarningOsVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение о невозможности получить доступ к данным компании. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumRequiredAppVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWarningAppVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWipeOsVersion|Строка|Версии, которые меньше или равны указанной версии, очищают управляемое приложение и связанные с ним данные компании. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWipeAppVersion|Строка|Версии, которые меньше или равны указанной версии, очищают управляемое приложение и связанные с ним данные компании. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения ( блокировка или очистка), если устройство имеет доступ к корневому каталогу или снято со снятой защитой, если свойство DeviceComplianceRequired имеет значение true. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `block`, `wipe`, `warn`.|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения ( блокировку или очистку) на основе максимального количества неверных попыток повторной попытки закрепления. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `block`, `wipe`, `warn`.|
|pinRequiredInofBiometricTimeout|Длительность|Время ожидания в минутах для пин-кода приложения вместо секретного кода, не являющегося биометрическим, унаследованным от [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedOutboundClipboardSharingExceptionLength|Int32|Укажите количество символов, которые могут быть вырезаны или скопированы из данных и учетных записей организации в любое приложение. Этот параметр переопределяет ограничение AllowedOutboundClipboardSharingLevel. Значение по умолчанию "0" означает, что исключение не допускается. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|notificationRestriction|[managedAppNotificationRestriction](../resources/intune-mam-managedappnotificationrestriction.md)|Укажите ограничение уведомлений приложения, [унаследованного от managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `allow`, `blockOrganizationalData`, `block`.|
|isAssigned|Boolean|Указывает, применена ли политика к группам включения. Наследуется от [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).|
|targetedAppManagementLevels|[appManagementLevel](../resources/intune-mam-appmanagementlevel.md)|Предполагаемые уровни управления приложениями для этой политики, унаследованные от [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md). Возможные значения: `unspecified`, `unmanaged`, `mdm`, `androidEnterprise`.|
|screenCaptureBlocked|Boolean|Указывает, может ли управляемый пользователь делать снимки экрана управляемых приложений.|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolean|Когда этот параметр включен, шифрование на уровне приложения отключается, если включено шифрование на уровне устройства.|
|encryptAppData|Boolean|Указывает, следует ли шифровать данные управляемых приложений.|
|deployedAppCount|Int32|Количество приложений, к которым применена текущая политика.|
|minimumRequiredPatchVersion|String|Определите самый старый уровень обновления для системы безопасности Android, необходимый для безопасного доступа к приложению.|
|minimumWarningPatchVersion|String|Определите самый старый уровень обновления для системы безопасности Android, рекомендуемый для безопасного доступа к приложению.|
|exemptedAppPackages|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Пакеты приложений в этом списке будут исключены из политики и смогут получать данные из управляемых приложений.|
|minimumWipePatchVersion|Строка|Уровень исправлений системы безопасности Android меньше или равен указанному значению, чтобы очистить управляемое приложение и связанные с ним данные компании.|
|allowedAndroidDeviceManufacturers|Строка|Разделенный точкой с запятой список производителей устройств, разрешенных в виде строки для работы управляемого приложения.|
|appActionIfAndroidDeviceManufacturerNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения , блокирование или очистку, если указанный производитель устройства не разрешен. Возможные значения: `block`, `wipe`, `warn`.|
|requiredAndroidSafetyNetDeviceAttestationType|[androidManagedAppSafetyNetDeviceAttestationType](../resources/intune-mam-androidmanagedappsafetynetdeviceattestationtype.md)|Определяет требование аттестации устройств Android SafetyNet для работы управляемого приложения. Возможные значения: `none`, `basicIntegrity`, `basicIntegrityAndDeviceCertification`.|
|appActionIfAndroidSafetyNetDeviceAttestationFailed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения( предупреждать или блокировать), если указанное подтверждение аттестации SafetyNet для Android завершается сбоем. Возможные значения: `block`, `wipe`, `warn`.|
|requiredAndroidSafetyNetAppsVerificationType|[androidManagedAppSafetyNetAppsVerificationType](../resources/intune-mam-androidmanagedappsafetynetappsverificationtype.md)|Определяет требование проверки приложений Android SafetyNet для работы управляемого приложения. Возможные значения: `none`, `enabled`.|
|appActionIfAndroidSafetyNetAppsVerificationFailed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемого приложения( предупреждать или блокировать), если указанное подтверждение проверки приложения Android завершается сбоем. Возможные значения: `block`, `wipe`, `warn`.|
|customBrowserPackageId|Строка|Уникальный идентификатор настраиваемого браузера для открытия веб-ссылки на Android.|
|customBrowserDisplayName|Строка|Понятное имя предпочтительного настраиваемого браузера для открытия веб-ссылки на Android.|
|minimumRequiredCompanyPortalVersion|Строка|Минимальная версия корпоративного портала, которая должна быть установлена на устройстве или в приложении, будет заблокирована.|
|minimumWarningCompanyPortalVersion|Строка|Минимальная версия корпоративного портала, которая должна быть установлена на устройстве, или пользователь получит предупреждение|
|minimumWipeCompanyPortalVersion|String|Минимальная версия корпоративного портала, которая должна быть установлена на устройстве или данные компании в приложении, будут очищены.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Управление мобильным приложением (MAM)**|
|assignments|Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|Свойство навигации для списка групп включения и исключения, к которым применяется политика. Наследуется от [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).|
|apps|Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Список приложений, к которым применена политика.|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|Свойства навигации к сводке по развертыванию конфигурации.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
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
  "isAssigned": true,
  "targetedAppManagementLevels": "String",
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 1024,
  "minimumRequiredPatchVersion": "String",
  "minimumWarningPatchVersion": "String",
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "minimumWipePatchVersion": "String",
  "allowedAndroidDeviceManufacturers": "String",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "String",
  "requiredAndroidSafetyNetDeviceAttestationType": "String",
  "appActionIfAndroidSafetyNetDeviceAttestationFailed": "String",
  "requiredAndroidSafetyNetAppsVerificationType": "String",
  "appActionIfAndroidSafetyNetAppsVerificationFailed": "String",
  "customBrowserPackageId": "String",
  "customBrowserDisplayName": "String",
  "minimumRequiredCompanyPortalVersion": "String",
  "minimumWarningCompanyPortalVersion": "String",
  "minimumWipeCompanyPortalVersion": "String"
}
```



