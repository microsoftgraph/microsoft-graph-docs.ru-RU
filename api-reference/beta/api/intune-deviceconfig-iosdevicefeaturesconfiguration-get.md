---
title: Get iosDeviceFeaturesConfiguration
description: Чтение свойств и связей объекта iosDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 14f8d9c8fa6283bb22e6b2264c32423222868081
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132676"
---
# <a name="get-iosdevicefeaturesconfiguration"></a><span data-ttu-id="ae7de-103">Get iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae7de-103">Get iosDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="ae7de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae7de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae7de-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae7de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae7de-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae7de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae7de-107">Чтение свойств и связей объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7de-107">Read properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae7de-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ae7de-108">Prerequisites</span></span>
<span data-ttu-id="ae7de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae7de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae7de-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae7de-111">Permission type</span></span>|<span data-ttu-id="ae7de-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae7de-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae7de-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae7de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae7de-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae7de-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae7de-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae7de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae7de-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae7de-116">Not supported.</span></span>|
|<span data-ttu-id="ae7de-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ae7de-117">Application</span></span>|<span data-ttu-id="ae7de-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae7de-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae7de-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae7de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae7de-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ae7de-120">Optional query parameters</span></span>
<span data-ttu-id="ae7de-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ae7de-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae7de-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae7de-122">Request headers</span></span>
|<span data-ttu-id="ae7de-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae7de-123">Header</span></span>|<span data-ttu-id="ae7de-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ae7de-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae7de-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae7de-125">Authorization</span></span>|<span data-ttu-id="ae7de-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae7de-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae7de-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ae7de-127">Accept</span></span>|<span data-ttu-id="ae7de-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ae7de-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae7de-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae7de-129">Request body</span></span>
<span data-ttu-id="ae7de-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ae7de-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae7de-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae7de-131">Response</span></span>
<span data-ttu-id="ae7de-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ae7de-132">If successful, this method returns a `200 OK` response code and [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae7de-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ae7de-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae7de-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae7de-134">Request</span></span>
<span data-ttu-id="ae7de-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae7de-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="ae7de-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae7de-136">Response</span></span>
<span data-ttu-id="ae7de-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae7de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7435

{
  "value": {
    "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
    "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
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
                "bundleID": "Bundle ID value",
                "isWebClip": true
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
                    "bundleID": "Bundle ID value",
                    "isWebClip": true
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
        "soundsEnabled": true,
        "previewVisibility": "alwaysShow"
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
    },
    "singleSignOnExtension": {
      "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension",
      "realm": "Realm value",
      "domains": [
        "Domains value"
      ],
      "blockAutomaticLogin": true,
      "cacheName": "Cache Name value",
      "credentialBundleIdAccessControlList": [
        "Credential Bundle Id Access Control List value"
      ],
      "domainRealms": [
        "Domain Realms value"
      ],
      "isDefaultRealm": true,
      "passwordBlockModification": true,
      "passwordExpirationDays": 6,
      "passwordExpirationNotificationDays": 2,
      "userPrincipalName": "User Principal Name value",
      "passwordRequireActiveDirectoryComplexity": true,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordMinimumLength": 5,
      "passwordMinimumAgeDays": 6,
      "passwordRequirementsDescription": "Password Requirements Description value",
      "requireUserPresence": true,
      "activeDirectorySiteCode": "Active Directory Site Code value",
      "passwordEnableLocalSync": true,
      "blockActiveDirectorySiteAutoDiscovery": true,
      "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
    },
    "iosSingleSignOnExtension": {
      "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension",
      "realm": "Realm value",
      "domains": [
        "Domains value"
      ],
      "blockAutomaticLogin": true,
      "cacheName": "Cache Name value",
      "credentialBundleIdAccessControlList": [
        "Credential Bundle Id Access Control List value"
      ],
      "domainRealms": [
        "Domain Realms value"
      ],
      "isDefaultRealm": true,
      "passwordBlockModification": true,
      "passwordExpirationDays": 6,
      "passwordExpirationNotificationDays": 2,
      "userPrincipalName": "User Principal Name value",
      "passwordRequireActiveDirectoryComplexity": true,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordMinimumLength": 5,
      "passwordMinimumAgeDays": 6,
      "passwordRequirementsDescription": "Password Requirements Description value",
      "requireUserPresence": true,
      "activeDirectorySiteCode": "Active Directory Site Code value",
      "passwordEnableLocalSync": true,
      "blockActiveDirectorySiteAutoDiscovery": true,
      "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
    }
  }
}
```




