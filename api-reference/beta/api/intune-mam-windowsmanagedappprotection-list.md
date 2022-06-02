---
title: Перечисление объектов windowsManagedAppProtection
description: Список свойств и связей объектов windowsManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 59f36fee770c87292795091f199396e2bd51655c
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858727"
---
# <a name="list-windowsmanagedappprotections"></a>Перечисление объектов windowsManagedAppProtection

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей объектов [windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagedAppProtections
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код `200 OK` отклика и коллекцию объектов [windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagedAppProtections
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1786

{
  "value": [
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
  ]
}
```




