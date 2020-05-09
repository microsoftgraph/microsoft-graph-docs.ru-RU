---
title: Получение объекта macOSDeviceFeaturesConfiguration
description: Чтение свойств и связей объекта macOSDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a5594efadfa5f8c77774ad808d05d378f0e5a2c0
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177921"
---
# <a name="get-macosdevicefeaturesconfiguration"></a><span data-ttu-id="beb76-103">Получение объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="beb76-103">Get macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="beb76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="beb76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="beb76-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beb76-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="beb76-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="beb76-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="beb76-107">Чтение свойств и связей объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="beb76-107">Read properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="beb76-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="beb76-108">Prerequisites</span></span>
<span data-ttu-id="beb76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="beb76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="beb76-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="beb76-111">Permission type</span></span>|<span data-ttu-id="beb76-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="beb76-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="beb76-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="beb76-113">Delegated (work or school account)</span></span>|<span data-ttu-id="beb76-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="beb76-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="beb76-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="beb76-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="beb76-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beb76-116">Not supported.</span></span>|
|<span data-ttu-id="beb76-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="beb76-117">Application</span></span>|<span data-ttu-id="beb76-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="beb76-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="beb76-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="beb76-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="beb76-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="beb76-120">Optional query parameters</span></span>
<span data-ttu-id="beb76-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="beb76-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="beb76-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="beb76-122">Request headers</span></span>
|<span data-ttu-id="beb76-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="beb76-123">Header</span></span>|<span data-ttu-id="beb76-124">Значение</span><span class="sxs-lookup"><span data-stu-id="beb76-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="beb76-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="beb76-125">Authorization</span></span>|<span data-ttu-id="beb76-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="beb76-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="beb76-127">Accept</span><span class="sxs-lookup"><span data-stu-id="beb76-127">Accept</span></span>|<span data-ttu-id="beb76-128">application/json</span><span class="sxs-lookup"><span data-stu-id="beb76-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="beb76-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="beb76-129">Request body</span></span>
<span data-ttu-id="beb76-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="beb76-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="beb76-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="beb76-131">Response</span></span>
<span data-ttu-id="beb76-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="beb76-132">If successful, this method returns a `200 OK` response code and [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="beb76-133">Пример</span><span class="sxs-lookup"><span data-stu-id="beb76-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="beb76-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="beb76-134">Request</span></span>
<span data-ttu-id="beb76-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="beb76-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="beb76-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="beb76-136">Response</span></span>
<span data-ttu-id="beb76-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="beb76-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4306

{
  "value": {
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
}
```



