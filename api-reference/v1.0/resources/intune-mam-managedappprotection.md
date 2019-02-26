---
title: Тип ресурса managedAppProtection
description: Политика, используемая для настройки расширенных параметров управления для определенного набора приложений.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b97b4b1453253ecd6fc5b5d77515b8b28586b19f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254130"
---
# <a name="managedappprotection-resource-type"></a>Тип ресурса managedAppProtection

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|String|Ключ объекта. Унаследовано от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|Строка|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|periodOfflineBeforeAccessCheck|Длительность|Время до проверки доступа, когда устройство не подключено к Интернету.|
|periodOnlineBeforeAccessCheck|Длительность|Время до проверки доступа, когда устройство подключено к Интернету.|
|allowedInboundDataTransferSources|[Манажедаппдататрансферлевел](../resources/intune-mam-managedappdatatransferlevel.md)|Источники, из которых разрешена передача данных. Возможные значения: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|[Манажедаппдататрансферлевел](../resources/intune-mam-managedappdatatransferlevel.md)|Места, в которые разрешена передача данных. Возможные значения: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Логический|Указывает, необходимы ли для использования приложения учетные данные организации.|
|allowedOutboundClipboardSharingLevel|[Манажедаппклипбоардшаринглевел](../resources/intune-mam-managedappclipboardsharinglevel.md)|Разрешенный уровень совместного использования буфера обмена для приложений на управляемом устройстве. Возможные значения: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Логический|Указывает, заблокировано ли резервное копирование данных управляемого приложения.|
|deviceComplianceRequired|Логический|Указывает, должно ли устройство соответствовать требованиям.|
|managedBrowserToOpenLinksRequired|Логический|Указывает, следует ли открывать интернет-ссылки в управляемом браузере.|
|saveAsBlocked|Boolean|Указывает, могут ли пользователи сохранять копии защищенных файлов, используя пункт меню "Сохранить как".|
|periodOfflineBeforeWipeIsEnforced|Продолжительность|Время до удаления всех управляемых данных после отключения приложения от Интернета.|
|pinRequired|Логический|Указывает, требуется ли ПИН-код на уровне приложения.|
|maximumPinRetries|Int32|Максимальное количество неудачных попыток ввода ПИН-кода перед блокированием или очисткой управляемого приложения.|
|simplePinBlocked|Boolean|Указывает, заблокирован ли простой ПИН-код.|
|minimumPinLength|Int32|Минимальная длина ПИН-кода на уровне приложения, если для параметра PinRequired установлено значение True.|
|pinCharacterSet|[Манажедапппинчарактерсет](../resources/intune-mam-managedapppincharacterset.md)|Разрешенный набор символов ПИН-кода на уровне приложения, если для параметра PinRequired установлено значение True. Возможные значения: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Продолжительность|Время до сброса универсального ПИН-кода, если для параметра PinRequired установлено значение True.|
|allowedDataStorageLocations|Коллекция [манажедаппдатасторажелокатион](../resources/intune-mam-managedappdatastoragelocation.md)|Разрешенные места хранения управляемых данных.|
|contactSyncBlocked|Логический|Указывает, можно ли синхронизировать контакты с устройством пользователя.|
|printBlocked|Логический|Указывает, разрешена ли печать из управляемых приложений.|
|fingerprintBlocked|Логический|Указывает, можно ли использовать сканер отпечатков пальцев вместо ПИН-кода, если для параметра PinRequired установлено значение True.|
|disableAppPinIfDevicePinIsSet|Boolean|Указывает, обязательно ли использовать ПИН-код приложения, если установлен ПИН-код устройства.|
|minimumRequiredOsVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании.|
|minimumWarningOsVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение о невозможности получить доступ к данным компании.|
|minimumRequiredAppVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании.|
|minimumWarningAppVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение.|

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
  "minimumWarningAppVersion": "String"
}
```


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-managedappprotection.md/microsoft.graph.managedAppProtection/allowedDataStorageLocations:
    Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->

