---
title: Тип ресурса defaultManagedAppProtection
description: Политика, используемая для настройки расширенных параметров управления для определенного набора приложений для всех пользователей, к которым не применяется политика TargetedManagedAppProtection
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2ec70076f7ee0fa30d40d527c1531258479a592b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945225"
---
# <a name="defaultmanagedappprotection-resource-type"></a>Тип ресурса defaultManagedAppProtection

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

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
|displayName|Строка|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|описание|Строка|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|id|Строка|Ключ объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|version|Строка|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|periodOfflineBeforeAccessCheck|Продолжительность|Время до проверки доступа, когда устройство не подключено к Интернету. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|periodOnlineBeforeAccessCheck|Продолжительность|Время до проверки доступа, когда устройство подключено к Интернету. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Источники, из которых разрешена передача данных. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Расположения, в которые разрешено передавать данные. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Boolean|Указывает, необходимы ли для использования приложения учетные данные организации. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|Разрешенный уровень совместного использования буфера обмена для приложений на управляемом устройстве. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolean|Указывает, заблокировано ли резервное копирование данных управляемого приложения. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|deviceComplianceRequired|Boolean|Указывает, обязательно ли соответствие устройства требованиям. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|managedBrowserToOpenLinksRequired|Boolean|Указывает, следует ли открывать интернет-ссылки в управляемом браузере. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|saveAsBlocked|Boolean|Указывает, могут ли пользователи сохранять копии защищенных файлов, используя пункт меню "Сохранить как". Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|periodOfflineBeforeWipeIsEnforced|Продолжительность|Время до удаления всех управляемых данных после отключения приложения от Интернета. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|pinRequired|Boolean|Указывает, обязательно ли использовать ПИН-код на уровне приложения. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|maximumPinRetries|Int32|Максимальное количество неправильный ПИН-код повторных попыток перед блокировке или очистить управляемые приложения. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|simplePinBlocked|Boolean|Указывает, заблокирован ли простой ПИН-код. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumPinLength|Int32|Минимальная длина ПИН-кода на уровне приложения, если для параметра PinRequired задано значение True. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|Разрешенный набор символов ПИН-кода на уровне приложения, если для параметра PinRequired задано значение True. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md). Возможные значения: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Продолжительность|Время до сброса универсального ПИН-кода, если для параметра PinRequired задано значение True. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedDataStorageLocations|[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) коллекции|Разрешенные места хранения управляемых данных. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|contactSyncBlocked|Boolean|Указывает, можно ли синхронизировать контакты с устройством пользователя. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|printBlocked|Boolean|Указывает, разрешена ли печать из управляемых приложений. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|fingerprintBlocked|Boolean|Указывает, можно ли использовать сканер отпечатков пальцев вместо ПИН-кода, если для параметра PinRequired задано значение True. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|disableAppPinIfDevicePinIsSet|Boolean|Указывает, обязательно ли использовать ПИН-код приложения, если задан ПИН-код устройства. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumRequiredOsVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWarningOsVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение о доступе к данным компании. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumRequiredAppVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании. Наследуется от объекта [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWarningAppVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение. Наследуется от [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune-mam-managedappdataencryptiontype.md)|Необходимый тип шифрования данных в управляемом приложении. (только для iOS.) Возможные значения: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.|
|screenCaptureBlocked|Boolean|Указывает, заблокированы ли снимки экрана. (только для Android).|
|encryptAppData|Boolean|Указывает, следует ли шифровать данные управляемых приложений (только для Android).|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolean|Если этот параметр включен, шифрование на уровне приложения отключено, если включено шифрование на уровне устройства. (только для Android).|
|minimumRequiredSdkVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании. (только для iOS)|
|customSettings|Коллекция [keyValuePair](../resources/intune-mam-keyvaluepair.md)|Набор, состоящий из пар ключа и значения строки, которые отправляются затронутым пользователям в неизменном виде.|
|deployedAppCount|Int32|Количество приложений, к которым применена текущая политика.|
|minimumRequiredPatchVersion|String|Определите самый старый уровень обновления для системы безопасности Android, необходимый для безопасного доступа к приложению. (только для Android).|
|minimumWarningPatchVersion|String|Определите самый старый уровень обновления для системы безопасности Android, рекомендуемый для безопасного доступа к приложению. (только для Android).|
|faceIdBlocked|Boolean|Указывает, можно ли использовать FaceID вместо ПИН-кода, если для параметра PinRequired установлено значение True. (только для iOS)|

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
  "faceIdBlocked": true
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-defaultmanagedappprotection.md/microsoft.graph.defaultManagedAppProtection/allowedDataStorageLocations:
      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->



