---
title: Список windowsKioskConfigurations
description: Список свойств и связей объектов WindowsKioskConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fffc65824cc6772711b29f926ac7c503e0545bda
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132375"
---
# <a name="list-windowskioskconfigurations"></a>Список windowsKioskConfigurations

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей объектов [WindowsKioskConfiguration.](../resources/intune-deviceconfig-windowskioskconfiguration.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3366

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
      "id": "146a990b-990b-146a-0b99-6a140b996a14",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "deviceManagementApplicabilityRuleOsEdition": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
        "osEditionTypes": [
          "windows10EnterpriseN"
        ],
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleOsVersion": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
        "minOSVersion": "Min OSVersion value",
        "maxOSVersion": "Max OSVersion value",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleDeviceMode": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
        "deviceMode": "sModeConfiguration",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "kioskProfiles": [
        {
          "@odata.type": "microsoft.graph.windowsKioskProfile",
          "profileId": "Profile Id value",
          "profileName": "Profile Name value",
          "appConfiguration": {
            "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
            "apps": [
              {
                "@odata.type": "microsoft.graph.windowsKioskUWPApp",
                "startLayoutTileSize": "small",
                "name": "Name value",
                "appType": "store",
                "autoLaunch": true,
                "appUserModelId": "App User Model Id value",
                "appId": "App Id value",
                "containedAppId": "Contained App Id value"
              }
            ],
            "showTaskBar": true,
            "allowAccessToDownloadsFolder": true,
            "disallowDesktopApps": true,
            "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
          },
          "userAccountsConfiguration": [
            {
              "@odata.type": "microsoft.graph.windowsKioskVisitor"
            }
          ]
        }
      ],
      "kioskBrowserDefaultUrl": "https://example.com/kioskBrowserDefaultUrl/",
      "kioskBrowserEnableHomeButton": true,
      "kioskBrowserEnableNavigationButtons": true,
      "kioskBrowserEnableEndSessionButton": true,
      "kioskBrowserRestartOnIdleTimeInMinutes": 6,
      "kioskBrowserBlockedURLs": [
        "Kiosk Browser Blocked URLs value"
      ],
      "kioskBrowserBlockedUrlExceptions": [
        "Kiosk Browser Blocked Url Exceptions value"
      ],
      "edgeKioskEnablePublicBrowsing": true,
      "windowsKioskForceUpdateSchedule": {
        "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule",
        "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
        "recurrence": "daily",
        "dayofWeek": "monday",
        "dayofMonth": 10,
        "runImmediatelyIfAfterStartDateTime": true
      }
    }
  ]
}
```




