---
title: Получить windowsKioskConfiguration
description: Чтение свойств и связей объекта WindowsKioskConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3c2984e881e616d1f404eaf843adf14b29ed845d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132347"
---
# <a name="get-windowskioskconfiguration"></a><span data-ttu-id="6b636-103">Получить windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="6b636-103">Get windowsKioskConfiguration</span></span>

<span data-ttu-id="6b636-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b636-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b636-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b636-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b636-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b636-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b636-107">Чтение свойств и связей [объекта WindowsKioskConfiguration.](../resources/intune-deviceconfig-windowskioskconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b636-107">Read properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b636-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6b636-108">Prerequisites</span></span>
<span data-ttu-id="6b636-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b636-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b636-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b636-111">Permission type</span></span>|<span data-ttu-id="6b636-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b636-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b636-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b636-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b636-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b636-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b636-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b636-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b636-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b636-116">Not supported.</span></span>|
|<span data-ttu-id="6b636-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6b636-117">Application</span></span>|<span data-ttu-id="6b636-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b636-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b636-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b636-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6b636-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6b636-120">Optional query parameters</span></span>
<span data-ttu-id="6b636-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6b636-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b636-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b636-122">Request headers</span></span>
|<span data-ttu-id="6b636-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b636-123">Header</span></span>|<span data-ttu-id="6b636-124">Значение</span><span class="sxs-lookup"><span data-stu-id="6b636-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b636-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b636-125">Authorization</span></span>|<span data-ttu-id="6b636-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b636-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b636-127">Accept</span><span class="sxs-lookup"><span data-stu-id="6b636-127">Accept</span></span>|<span data-ttu-id="6b636-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6b636-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b636-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b636-129">Request body</span></span>
<span data-ttu-id="6b636-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6b636-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b636-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b636-131">Response</span></span>
<span data-ttu-id="6b636-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6b636-132">If successful, this method returns a `200 OK` response code and [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b636-133">Пример</span><span class="sxs-lookup"><span data-stu-id="6b636-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b636-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b636-134">Request</span></span>
<span data-ttu-id="6b636-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b636-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="6b636-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b636-136">Response</span></span>
<span data-ttu-id="6b636-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b636-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3186

{
  "value": {
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
}
```




