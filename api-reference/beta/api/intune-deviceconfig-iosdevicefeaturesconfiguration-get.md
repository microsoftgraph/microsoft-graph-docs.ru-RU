---
title: Get iosDeviceFeaturesConfiguration
description: Чтение свойств и связей объекта iosDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 34fcfddce904e10e48f70ea8635b49fd6546d620
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817327"
---
# <a name="get-iosdevicefeaturesconfiguration"></a><span data-ttu-id="5c67f-103">Get iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="5c67f-103">Get iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="5c67f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5c67f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c67f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c67f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c67f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5c67f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c67f-107">Чтение свойств и связей объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c67f-107">Read properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c67f-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5c67f-108">Prerequisites</span></span>
<span data-ttu-id="5c67f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c67f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c67f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c67f-111">Permission type</span></span>|<span data-ttu-id="5c67f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c67f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c67f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c67f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c67f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c67f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5c67f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c67f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c67f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c67f-116">Not supported.</span></span>|
|<span data-ttu-id="5c67f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c67f-117">Application</span></span>|<span data-ttu-id="5c67f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c67f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c67f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c67f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c67f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5c67f-120">Optional query parameters</span></span>
<span data-ttu-id="5c67f-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5c67f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5c67f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c67f-122">Request headers</span></span>
|<span data-ttu-id="5c67f-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c67f-123">Header</span></span>|<span data-ttu-id="5c67f-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5c67f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c67f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c67f-125">Authorization</span></span>|<span data-ttu-id="5c67f-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5c67f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c67f-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5c67f-127">Accept</span></span>|<span data-ttu-id="5c67f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5c67f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c67f-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c67f-129">Request body</span></span>
<span data-ttu-id="5c67f-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c67f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c67f-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c67f-131">Response</span></span>
<span data-ttu-id="5c67f-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5c67f-132">If successful, this method returns a `200 OK` response code and [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c67f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5c67f-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c67f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c67f-134">Request</span></span>
<span data-ttu-id="5c67f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c67f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5c67f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c67f-136">Response</span></span>
<span data-ttu-id="5c67f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5c67f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3904

{
  "value": {
    "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
    "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "airPrintDestinations": [
      {
        "@odata.type": "microsoft.graph.airPrintDestination",
        "ipAddress": "Ip Address value",
        "resourcePath": "Resource Path value",
        "port": 4,
        "forceTls": true
      }
    ],
    "assetTagTemplate": "Asset Tag Template value",
    "contentFilterSettings": {
      "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
      "specificWebsitesOnly": [
        {
          "@odata.type": "microsoft.graph.iosBookmark",
          "url": "Url value",
          "bookmarkFolder": "Bookmark Folder value",
          "displayName": "Display Name value"
        }
      ],
      "websiteList": [
        {
          "@odata.type": "microsoft.graph.iosBookmark",
          "url": "Url value",
          "bookmarkFolder": "Bookmark Folder value",
          "displayName": "Display Name value"
        }
      ]
    },
    "lockScreenFootnote": "Lock Screen Footnote value",
    "homeScreenDockIcons": [
      {
        "@odata.type": "microsoft.graph.iosHomeScreenFolder",
        "displayName": "Display Name value",
        "pages": [
          {
            "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
            "displayName": "Display Name value",
            "apps": [
              {
                "@odata.type": "microsoft.graph.iosHomeScreenApp",
                "displayName": "Display Name value",
                "bundleID": "Bundle ID value"
              }
            ]
          }
        ]
      }
    ],
    "homeScreenPages": [
      {
        "@odata.type": "microsoft.graph.iosHomeScreenPage",
        "displayName": "Display Name value",
        "icons": [
          {
            "@odata.type": "microsoft.graph.iosHomeScreenFolder",
            "displayName": "Display Name value",
            "pages": [
              {
                "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
                "displayName": "Display Name value",
                "apps": [
                  {
                    "@odata.type": "microsoft.graph.iosHomeScreenApp",
                    "displayName": "Display Name value",
                    "bundleID": "Bundle ID value"
                  }
                ]
              }
            ]
          }
        ]
      }
    ],
    "notificationSettings": [
      {
        "@odata.type": "microsoft.graph.iosNotificationSettings",
        "bundleID": "Bundle ID value",
        "appName": "App Name value",
        "publisher": "Publisher value",
        "enabled": true,
        "showInNotificationCenter": true,
        "showOnLockScreen": true,
        "alertType": "banner",
        "badgesEnabled": true,
        "soundsEnabled": true
      }
    ],
    "singleSignOnSettings": {
      "@odata.type": "microsoft.graph.iosSingleSignOnSettings",
      "allowedAppsList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "allowedUrls": [
        "Allowed Urls value"
      ],
      "displayName": "Display Name value",
      "kerberosPrincipalName": "Kerberos Principal Name value",
      "kerberosRealm": "Kerberos Realm value"
    }
  }
}
```





