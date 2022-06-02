---
title: Тип ресурса windowsManagedAppProtection
description: Политика, используемая для настройки подробных параметров управления, предназначенных для определенных групп безопасности и для указанного набора приложений на Windows устройстве
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2d3116545d5d9bf8480f8c35dcd7ed7703739304
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858775"
---
# <a name="windowsmanagedappprotection-resource-type"></a>Тип ресурса windowsManagedAppProtection

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политика, используемая для настройки подробных параметров управления, предназначенных для определенных групп безопасности и для указанного набора приложений на Windows устройстве


Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов windowsManagedAppProtection](../api/intune-mam-windowsmanagedappprotection-list.md)|[Коллекция windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md)|Список свойств и связей объектов [windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) .|
|[Получение объекта windowsManagedAppProtection](../api/intune-mam-windowsmanagedappprotection-get.md)|[windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md)|Чтение свойств и связей объекта [windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) .|
|[Создание объекта windowsManagedAppProtection](../api/intune-mam-windowsmanagedappprotection-create.md)|[windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md)|Создайте объект [windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) .|
|[Удаление объекта windowsManagedAppProtection](../api/intune-mam-windowsmanagedappprotection-delete.md)|Нет|Удаляет объект [windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md).|
|[Обновление windowsManagedAppProtection](../api/intune-mam-windowsmanagedappprotection-update.md)|[windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md)|Обновление свойств объекта [windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) .|
|[Действие targetApps](../api/intune-mam-windowsmanagedappprotection-targetapps.md)|Нет|Н/Д|
|[Действие assign](../api/intune-mam-windowsmanagedappprotection-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|description|Строка|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|Идентификаторы roleScopeTagId|Коллекция строк|Список тегов области для этого экземпляра сущности. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|id|String|Ключ объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|version|String|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|isAssigned|Boolean|Значение TRUE указывает, что политика развернута в некоторых группах включения. Значение FALSE указывает, что политика не развернута ни в каких группах включения. Значение по умолчанию — FALSE.|
|deployedAppCount|Int32|Указывает общее количество приложений, для которых развернута текущая политика.|
|printBlocked|Boolean|Значение TRUE указывает, что печать заблокирована в управляемых приложениях. Значение FALSE указывает, что печать разрешена из управляемых приложений. Значение по умолчанию — FALSE.|
|allowedInboundDataTransferSources|[windowsManagedAppDataTransferLevel](../resources/intune-mam-windowsmanagedappdatatransferlevel.md)|Указывает источники, из которых разрешено передавать данные. Некоторые возможные значения— allApps или none. Возможные значения: `allApps`, `none`.|
|allowedOutboundClipboardSharingLevel|[windowsManagedAppClipboardSharingLevel](../resources/intune-mam-windowsmanagedappclipboardsharinglevel.md)|Указывает уровень, на который буфер обмена может быть совместно использоваться & ресурсами, не входя в организацию. Некоторые возможные значения: anyDestinationAnySource или none. Возможные значения: `anyDestinationAnySource`, `none`.|
|allowedOutboundDataTransferDestinations|[windowsManagedAppDataTransferLevel](../resources/intune-mam-windowsmanagedappdatatransferlevel.md)|Указывает назначения, в которые разрешено передавать данные. Некоторые возможные значения— allApps или none. Возможные значения: `allApps`, `none`.|
|appActionIfUnableToAuthenticateUser|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Если задано, будет указано, какое действие следует выполнить в случае, если пользователь не может выполнить проверку подлинности, так как его маркер проверки подлинности недопустим. Это происходит при удалении или отключении пользователя в AAD. Некоторые возможные значения— блочные или очистки. Если это свойство не задано, никаких действий выполняться не будет. Возможные значения: `block`, `wipe`, `warn`.|
|maximumAllowedDeviceThreatLevel|[managedAppDeviceThreatLevel](../resources/intune-mam-managedappdevicethreatlevel.md)|Максимальный допустимый уровень угроз устройства, о чем сообщает приложение Mobile Threat Defense. Возможные значения: `notConfigured`, `secured`, `low`, `medium`, `high`.|
|mobileThreatDefenseRemediationAction|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Определяет, какие действия следует выполнить, если пороговое значение угрозы защиты мобильных устройств от угроз не соблюдены. Некоторые возможные значения— блочные или очистки. Предупреждение не является поддерживаемым значением для этого свойства. Возможные значения: `block`, `wipe`, `warn`.|
|minimumRequiredSdkVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании. Например, "8.1.0" или "13.1.1".|
|minimumWipeSdkVersion|Строка|Версии, которые меньше указанной версии, очищают управляемое приложение и связанные с ним данные компании. Например, "8.1.0" или "13.1.1".|
|minimumRequiredOsVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании. Например, "8.1.0" или "13.1.1".|
|minimumWarningOsVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение о невозможности получить доступ к данным компании. Например, "8.1.0" или "13.1.1".|
|minimumWipeOsVersion|String|Версии, которые меньше указанной версии, очищают управляемое приложение и связанные с ним данные компании. Например, "8.1.0" или "13.1.1".|
|minimumRequiredAppVersion|String|В более старых версиях управляемое приложение не сможет получить доступ к данным компании. Например, "8.1.0" или "13.1.1".|
|minimumWarningAppVersion|String|В более старых версиях в управляемом приложении будет отображаться предупреждающее сообщение о невозможности получить доступ к данным компании. Например, "8.1.0" или "13.1.1".|
|minimumWipeAppVersion|Строка|Версии, которые меньше указанной версии, очищают управляемое приложение и связанные с ним данные компании. Например, "8.1.0" или "13.1.1".|
|maximumRequiredOsVersion|Строка|Версии, которые больше указанной версии, блокируют доступ управляемого приложения к данным компании. Например, "8.1.0" или "13.1.1".|
|maximumWarningOsVersion|Строка|Версии, которые больше указанной версии, выдают управляемому приложению предупреждение о доступе к данным компании. Например, "8.1.0" или "13.1.1".|
|maximumWipeOsVersion|Строка|Версии, размер которых превышает указанную версию, очищают управляемое приложение и связанные с ним данные компании. Например, "8.1.0" или "13.1.1".|
|periodOfflineBeforeWipeIsEnforced|Duration|Время до удаления всех управляемых данных после отключения приложения от Интернета. Например, P5D указывает, что интервал составляет 5 дней. Значение интервала времени PT0S указывает, что управляемые данные никогда не будут очищаться, если устройство не подключено к Интернету.|
|periodOfflineBeforeAccessCheck|Duration|Время до проверки доступа, когда устройство не подключено к Интернету. Например, PT5M указывает, что интервал составляет 5 минут. Значение интервала времени PT0S указывает, что доступ будет заблокирован немедленно, когда устройство не подключено к Интернету.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|Список групп включения и исключения, к которым применяется политика.|
|apps|Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Список приложений, к которым применена политика.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagedAppProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String",
  "isAssigned": true,
  "deployedAppCount": 1024,
  "printBlocked": true,
  "allowedInboundDataTransferSources": "String",
  "allowedOutboundClipboardSharingLevel": "String",
  "allowedOutboundDataTransferDestinations": "String",
  "appActionIfUnableToAuthenticateUser": "String",
  "maximumAllowedDeviceThreatLevel": "String",
  "mobileThreatDefenseRemediationAction": "String",
  "minimumRequiredSdkVersion": "String",
  "minimumWipeSdkVersion": "String",
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumWipeOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String",
  "minimumWipeAppVersion": "String",
  "maximumRequiredOsVersion": "String",
  "maximumWarningOsVersion": "String",
  "maximumWipeOsVersion": "String",
  "periodOfflineBeforeWipeIsEnforced": "String (duration)",
  "periodOfflineBeforeAccessCheck": "String (duration)"
}
```




