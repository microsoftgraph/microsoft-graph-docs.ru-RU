---
title: Перечисление объектов iosDeviceFeaturesConfiguration
description: Список свойств и связей объектов iosDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d070ec281f6d87c2aa72d9f03387e800f3795597
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790223"
---
# <a name="list-iosdevicefeaturesconfigurations"></a><span data-ttu-id="4547b-103">Перечисление объектов iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="4547b-103">List iosDeviceFeaturesConfigurations</span></span>

> <span data-ttu-id="4547b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4547b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4547b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4547b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4547b-106">Список свойств и связей объектов [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4547b-106">List properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4547b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4547b-107">Prerequisites</span></span>
<span data-ttu-id="4547b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4547b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4547b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4547b-110">Permission type</span></span>|<span data-ttu-id="4547b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4547b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4547b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4547b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4547b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4547b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4547b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4547b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4547b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4547b-115">Not supported.</span></span>|
|<span data-ttu-id="4547b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4547b-116">Application</span></span>|<span data-ttu-id="4547b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4547b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4547b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4547b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4547b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4547b-119">Request headers</span></span>
|<span data-ttu-id="4547b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4547b-120">Header</span></span>|<span data-ttu-id="4547b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4547b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4547b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4547b-122">Authorization</span></span>|<span data-ttu-id="4547b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4547b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4547b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4547b-124">Accept</span></span>|<span data-ttu-id="4547b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4547b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4547b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4547b-126">Request body</span></span>
<span data-ttu-id="4547b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4547b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4547b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4547b-128">Response</span></span>
<span data-ttu-id="4547b-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4547b-129">If successful, this method returns a `200 OK` response code and a collection of [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4547b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4547b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4547b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4547b-131">Request</span></span>
<span data-ttu-id="4547b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4547b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="4547b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4547b-133">Response</span></span>
<span data-ttu-id="4547b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4547b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4353

{
  "value": [
    {
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
  ]
}
```





