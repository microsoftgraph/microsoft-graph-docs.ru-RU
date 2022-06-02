---
title: Обновление windowsManagedAppProtection
description: Обновление свойств объекта windowsManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ec1fbab7605a65a27139761fb8f14443186d4f3
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858902"
---
# <a name="update-windowsmanagedappprotection"></a>Обновление windowsManagedAppProtection

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagedAppProtections/{windowsManagedAppProtectionId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [windowsManagedAppProtection в формате](../resources/intune-mam-windowsmanagedappprotection.md) JSON.

В следующей таблице показаны свойства, необходимые при создании [объекта windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|description|Строка|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|Идентификаторы roleScopeTagId|Коллекция String|Список тегов области для этого экземпляра сущности. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
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



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код `200 OK` отклика и обновленный объект [windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagedAppProtections/{windowsManagedAppProtectionId}
Content-type: application/json
Content-length: 1453

{
  "@odata.type": "#microsoft.graph.windowsManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "version": "Version value",
  "isAssigned": true,
  "deployedAppCount": 0,
  "printBlocked": true,
  "allowedInboundDataTransferSources": "none",
  "allowedOutboundClipboardSharingLevel": "none",
  "allowedOutboundDataTransferDestinations": "none",
  "appActionIfUnableToAuthenticateUser": "wipe",
  "maximumAllowedDeviceThreatLevel": "secured",
  "mobileThreatDefenseRemediationAction": "wipe",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "maximumRequiredOsVersion": "Maximum Required Os Version value",
  "maximumWarningOsVersion": "Maximum Warning Os Version value",
  "maximumWipeOsVersion": "Maximum Wipe Os Version value",
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1625

{
  "@odata.type": "#microsoft.graph.windowsManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "c7894cd1-4cd1-c789-d14c-89c7d14c89c7",
  "version": "Version value",
  "isAssigned": true,
  "deployedAppCount": 0,
  "printBlocked": true,
  "allowedInboundDataTransferSources": "none",
  "allowedOutboundClipboardSharingLevel": "none",
  "allowedOutboundDataTransferDestinations": "none",
  "appActionIfUnableToAuthenticateUser": "wipe",
  "maximumAllowedDeviceThreatLevel": "secured",
  "mobileThreatDefenseRemediationAction": "wipe",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "maximumRequiredOsVersion": "Maximum Required Os Version value",
  "maximumWarningOsVersion": "Maximum Warning Os Version value",
  "maximumWipeOsVersion": "Maximum Wipe Os Version value",
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S"
}
```




