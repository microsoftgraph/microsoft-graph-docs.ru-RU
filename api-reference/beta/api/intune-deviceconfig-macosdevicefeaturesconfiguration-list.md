---
title: Перечисление объектов macOSDeviceFeaturesConfiguration
description: Список свойств и связей объектов macOSDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9ec23fdd99ca0bc7585121ac5b15e42237098b8e
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177914"
---
# <a name="list-macosdevicefeaturesconfigurations"></a><span data-ttu-id="3e926-103">Перечисление объектов macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e926-103">List macOSDeviceFeaturesConfigurations</span></span>

<span data-ttu-id="3e926-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e926-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e926-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e926-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e926-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e926-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e926-107">Список свойств и связей объектов [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e926-107">List properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e926-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3e926-108">Prerequisites</span></span>
<span data-ttu-id="3e926-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e926-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e926-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e926-111">Permission type</span></span>|<span data-ttu-id="3e926-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e926-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e926-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e926-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e926-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e926-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3e926-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e926-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e926-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e926-116">Not supported.</span></span>|
|<span data-ttu-id="3e926-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e926-117">Application</span></span>|<span data-ttu-id="3e926-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e926-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e926-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e926-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3e926-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3e926-120">Request headers</span></span>
|<span data-ttu-id="3e926-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e926-121">Header</span></span>|<span data-ttu-id="3e926-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3e926-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e926-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e926-123">Authorization</span></span>|<span data-ttu-id="3e926-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e926-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e926-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3e926-125">Accept</span></span>|<span data-ttu-id="3e926-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e926-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e926-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e926-127">Request body</span></span>
<span data-ttu-id="3e926-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3e926-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e926-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e926-129">Response</span></span>
<span data-ttu-id="3e926-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3e926-130">If successful, this method returns a `200 OK` response code and a collection of [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e926-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3e926-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e926-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e926-132">Request</span></span>
<span data-ttu-id="3e926-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e926-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="3e926-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e926-134">Response</span></span>
<span data-ttu-id="3e926-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e926-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4556

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
      "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
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
      "autoLaunchItems": [
        {
          "@odata.type": "microsoft.graph.macOSLaunchItem",
          "path": "Path value",
          "hide": true
        }
      ],
      "adminShowHostInfo": true,
      "loginWindowText": "Login Window Text value",
      "authorizedUsersListHidden": true,
      "authorizedUsersListHideLocalUsers": true,
      "authorizedUsersListHideMobileAccounts": true,
      "authorizedUsersListIncludeNetworkUsers": true,
      "authorizedUsersListHideAdminUsers": true,
      "authorizedUsersListShowOtherManagedUsers": true,
      "shutDownDisabled": true,
      "restartDisabled": true,
      "sleepDisabled": true,
      "consoleAccessDisabled": true,
      "shutDownDisabledWhileLoggedIn": true,
      "restartDisabledWhileLoggedIn": true,
      "powerOffDisabledWhileLoggedIn": true,
      "logOutDisabledWhileLoggedIn": true,
      "screenLockDisableImmediate": true,
      "associatedDomains": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "singleSignOnExtension": {
        "@odata.type": "microsoft.graph.credentialSingleSignOnExtension",
        "extensionIdentifier": "Extension Identifier value",
        "teamIdentifier": "Team Identifier value",
        "domains": [
          "Domains value"
        ],
        "realm": "Realm value",
        "configurations": [
          {
            "@odata.type": "microsoft.graph.keyStringValuePair",
            "key": "Key value",
            "value": "Value value"
          }
        ]
      },
      "macOSSingleSignOnExtension": {
        "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension",
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



