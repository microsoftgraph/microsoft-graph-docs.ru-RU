---
title: Перечисление объектов iosDeviceFeaturesConfiguration
description: Список свойств и связей объектов iosDeviceFeaturesConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 70c81605b51eeac6f991232cc7c2abc61560f0fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449049"
---
# <a name="list-iosdevicefeaturesconfigurations"></a><span data-ttu-id="cc713-103">Перечисление объектов iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="cc713-103">List iosDeviceFeaturesConfigurations</span></span>

<span data-ttu-id="cc713-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cc713-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc713-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc713-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc713-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc713-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc713-107">Список свойств и связей объектов [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc713-107">List properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc713-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cc713-108">Prerequisites</span></span>
<span data-ttu-id="cc713-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc713-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc713-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc713-111">Permission type</span></span>|<span data-ttu-id="cc713-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc713-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc713-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc713-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc713-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc713-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cc713-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc713-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc713-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc713-116">Not supported.</span></span>|
|<span data-ttu-id="cc713-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc713-117">Application</span></span>|<span data-ttu-id="cc713-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc713-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc713-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc713-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cc713-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cc713-120">Request headers</span></span>
|<span data-ttu-id="cc713-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc713-121">Header</span></span>|<span data-ttu-id="cc713-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cc713-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc713-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc713-123">Authorization</span></span>|<span data-ttu-id="cc713-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc713-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc713-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cc713-125">Accept</span></span>|<span data-ttu-id="cc713-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cc713-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc713-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc713-127">Request body</span></span>
<span data-ttu-id="cc713-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cc713-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc713-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="cc713-129">Response</span></span>
<span data-ttu-id="cc713-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cc713-130">If successful, this method returns a `200 OK` response code and a collection of [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc713-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cc713-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc713-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc713-132">Request</span></span>
<span data-ttu-id="cc713-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc713-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="cc713-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc713-134">Response</span></span>
<span data-ttu-id="cc713-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc713-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7737

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
  ]
}
```





