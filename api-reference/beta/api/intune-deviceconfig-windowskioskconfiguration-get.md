---
title: Получение windowsKioskConfiguration
description: Чтение свойства и связи объекта windowsKioskConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4860924b415ef71913792a2f96c7a4ac934c25cd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851725"
---
# <a name="get-windowskioskconfiguration"></a><span data-ttu-id="ceb8e-103">Получение windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="ceb8e-103">Get windowsKioskConfiguration</span></span>

> <span data-ttu-id="ceb8e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ceb8e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ceb8e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ceb8e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ceb8e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ceb8e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ceb8e-107">Чтение свойства и связи объекта [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ceb8e-107">Read properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ceb8e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ceb8e-108">Prerequisites</span></span>
<span data-ttu-id="ceb8e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ceb8e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ceb8e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ceb8e-111">Permission type</span></span>|<span data-ttu-id="ceb8e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ceb8e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ceb8e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ceb8e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ceb8e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ceb8e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ceb8e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ceb8e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ceb8e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ceb8e-116">Not supported.</span></span>|
|<span data-ttu-id="ceb8e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ceb8e-117">Application</span></span>|<span data-ttu-id="ceb8e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ceb8e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ceb8e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ceb8e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ceb8e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ceb8e-120">Optional query parameters</span></span>
<span data-ttu-id="ceb8e-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ceb8e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ceb8e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ceb8e-122">Request headers</span></span>
|<span data-ttu-id="ceb8e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ceb8e-123">Header</span></span>|<span data-ttu-id="ceb8e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ceb8e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ceb8e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ceb8e-125">Authorization</span></span>|<span data-ttu-id="ceb8e-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ceb8e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ceb8e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ceb8e-127">Accept</span></span>|<span data-ttu-id="ceb8e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ceb8e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ceb8e-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ceb8e-129">Request body</span></span>
<span data-ttu-id="ceb8e-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ceb8e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ceb8e-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ceb8e-131">Response</span></span>
<span data-ttu-id="ceb8e-132">Успешно завершена, этот метод возвращает `200 OK` объект [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ceb8e-132">If successful, this method returns a `200 OK` response code and [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ceb8e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ceb8e-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ceb8e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ceb8e-134">Request</span></span>
<span data-ttu-id="ceb8e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ceb8e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="ceb8e-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="ceb8e-136">Response</span></span>
<span data-ttu-id="ceb8e-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ceb8e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1889

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
    "id": "146a990b-990b-146a-0b99-6a140b996a14",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
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
              "appUserModelId": "App User Model Id value",
              "appId": "App Id value",
              "containedAppId": "Contained App Id value"
            }
          ],
          "showTaskBar": true,
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
    ]
  }
}
```





