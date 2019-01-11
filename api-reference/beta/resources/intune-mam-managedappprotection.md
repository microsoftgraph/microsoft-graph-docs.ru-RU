---
title: Тип ресурса managedAppProtection
description: Политика, используемая для настройки расширенных параметров управления для определенного набора приложений.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 97d98a6edea3b03b7d35d68ca1f274e938449990
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833000"
---
# <a name="managedappprotection-resource-type"></a>Тип ресурса managedAppProtection

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

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
|описание|Строка|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|id|Строка|Ключ объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|version|Строка|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|periodOfflineBeforeAccessCheck|Продолжительность|Время до проверки доступа, когда устройство не подключено к Интернету.|
|periodOnlineBeforeAccessCheck|Продолжительность|Время до проверки доступа, когда устройство подключено к Интернету.|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Источники, из которых разрешена передача данных. Возможные значения: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Места, в которые разрешена передача данных. Возможные значения: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Boolean|Указывает, необходимы ли для использования приложения учетные данные организации.|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|Разрешенный уровень совместного использования буфера обмена для приложений на управляемом устройстве. Возможные значения: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolean|Указывает, заблокировано ли резервное копирование данных управляемого приложения.|
|deviceComplianceRequired|Boolean|Указывает, должно ли устройство соответствовать требованиям.|
|managedBrowserToOpenLinksRequired|Boolean|Указывает, следует ли открывать интернет-ссылки в управляемом браузере.|
|saveAsBlocked|Boolean|Указывает, могут ли пользователи сохранять копии защищенных файлов, используя пункт меню "Сохранить как".|
|periodOfflineBeforeWipeIsEnforced|Продолжительность|Время до удаления всех управляемых данных после отключения приложения от Интернета.|
|pinRequired|Boolean|Указывает, требуется ли ПИН-код на уровне приложения.|
|maximumPinRetries|Int32|Максимальное количество неправильный ПИН-код повторных попыток перед блокировке или очистить управляемые приложения.|
|simplePinBlocked|Boolean|Указывает, заблокирован ли простой ПИН-код.|
|minimumPinLength|Int32|Минимальная длина ПИН-кода на уровне приложения, если для параметра PinRequired установлено значение True.|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|Разрешенный набор символов ПИН-кода на уровне приложения, если для параметра PinRequired установлено значение True. Возможные значения: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Продолжительность|Время до сброса универсального ПИН-кода, если для параметра PinRequired установлено значение True.|
|allowedDataStorageLocations|[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) коллекции|Разрешенные места хранения управляемых данных.|
|contactSyncBlocked|Boolean|Указывает, можно ли синхронизировать контакты с устройством пользователя.|
|printBlocked|Boolean|Указывает, разрешена ли печать из управляемых приложений.|
|fingerprintBlocked|Boolean|Указывает, можно ли использовать сканер отпечатков пальцев вместо ПИН-кода, если для параметра PinRequired установлено значение True.|
|disableAppPinIfDevicePinIsSet|Boolean|Указывает, обязательно ли использовать ПИН-код приложения, если установлен ПИН-код устройства.|
|minimumRequiredOsVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании.|
|minimumWarningOsVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение о невозможности получить доступ к данным компании.|
|minimumRequiredAppVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании.|
|minimumWarningAppVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение.|
|minimumWipeOsVersion|Строка|Версии меньше или равно указанную версию будет удаления управляемых приложений и данных связанные компании.|
|minimumWipeAppVersion|Строка|Версии меньше или равно указанную версию будет удаления управляемых приложений и данных связанные компании.|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемых приложений, блокировки или очистки, когда устройства либо корневого или jailbroken, если DeviceComplianceRequired задано значение true. Возможные значения: `block`, `wipe`.|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет поведение управляемых приложений, либо блок или стирание, на основании максимальное количество повторных попыток неправильный ПИН-код. Возможные значения: `block`, `wipe`.|
|pinRequiredInsteadOfBiometricTimeout|Продолжительность|Время ожидания в минутах для закрепления приложения вместо секретный код не биометрия|

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
  "pinRequiredInsteadOfBiometricTimeout": "String (duration)"
}
```





