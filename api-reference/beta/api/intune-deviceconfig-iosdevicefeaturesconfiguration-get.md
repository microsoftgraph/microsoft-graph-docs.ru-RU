---
title: Get iosDeviceFeaturesConfiguration
description: Чтение свойств и связей объекта iosDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f6ca86f5b01932061a6be5eefb1eb2ad939be584
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161420"
---
# <a name="get-iosdevicefeaturesconfiguration"></a><span data-ttu-id="4b743-103">Get iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b743-103">Get iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="4b743-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b743-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b743-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b743-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b743-106">Чтение свойств и связей объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b743-106">Read properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b743-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4b743-107">Prerequisites</span></span>
<span data-ttu-id="4b743-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4b743-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4b743-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b743-110">Permission type</span></span>|<span data-ttu-id="4b743-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b743-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b743-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b743-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b743-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b743-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4b743-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b743-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b743-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b743-115">Not supported.</span></span>|
|<span data-ttu-id="4b743-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b743-116">Application</span></span>|<span data-ttu-id="4b743-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b743-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b743-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b743-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4b743-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4b743-119">Optional query parameters</span></span>
<span data-ttu-id="4b743-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4b743-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b743-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b743-121">Request headers</span></span>
|<span data-ttu-id="4b743-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b743-122">Header</span></span>|<span data-ttu-id="4b743-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4b743-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b743-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b743-124">Authorization</span></span>|<span data-ttu-id="4b743-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4b743-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b743-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4b743-126">Accept</span></span>|<span data-ttu-id="4b743-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4b743-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b743-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b743-128">Request body</span></span>
<span data-ttu-id="4b743-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4b743-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b743-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b743-130">Response</span></span>
<span data-ttu-id="4b743-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4b743-131">If successful, this method returns a `200 OK` response code and [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b743-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4b743-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b743-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b743-133">Request</span></span>
<span data-ttu-id="4b743-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b743-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="4b743-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b743-135">Response</span></span>
<span data-ttu-id="4b743-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b743-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4093

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
    },
    "wallpaperDisplayLocation": "lockScreen",
    "wallpaperImage": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    }
  }
}
```




