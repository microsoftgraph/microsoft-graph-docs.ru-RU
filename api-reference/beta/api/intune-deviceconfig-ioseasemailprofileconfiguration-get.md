---
title: Получение iosEasEmailProfileConfiguration
description: Чтение свойств и связей объекта iosEasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 90b1e99d84491a70be66a3ad302af16b4a55ba7a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37174524"
---
# <a name="get-ioseasemailprofileconfiguration"></a><span data-ttu-id="50b17-103">Получение iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="50b17-103">Get iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="50b17-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50b17-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50b17-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50b17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50b17-106">Чтение свойств и связей объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="50b17-106">Read properties and relationships of the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50b17-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="50b17-107">Prerequisites</span></span>
<span data-ttu-id="50b17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50b17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50b17-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50b17-110">Permission type</span></span>|<span data-ttu-id="50b17-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="50b17-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50b17-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50b17-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50b17-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50b17-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="50b17-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50b17-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50b17-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50b17-115">Not supported.</span></span>|
|<span data-ttu-id="50b17-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50b17-116">Application</span></span>|<span data-ttu-id="50b17-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50b17-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50b17-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50b17-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50b17-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="50b17-119">Optional query parameters</span></span>
<span data-ttu-id="50b17-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="50b17-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50b17-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50b17-121">Request headers</span></span>
|<span data-ttu-id="50b17-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50b17-122">Header</span></span>|<span data-ttu-id="50b17-123">Значение</span><span class="sxs-lookup"><span data-stu-id="50b17-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50b17-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50b17-124">Authorization</span></span>|<span data-ttu-id="50b17-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50b17-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50b17-126">Accept</span><span class="sxs-lookup"><span data-stu-id="50b17-126">Accept</span></span>|<span data-ttu-id="50b17-127">application/json</span><span class="sxs-lookup"><span data-stu-id="50b17-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50b17-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="50b17-128">Request body</span></span>
<span data-ttu-id="50b17-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="50b17-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50b17-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="50b17-130">Response</span></span>
<span data-ttu-id="50b17-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="50b17-131">If successful, this method returns a `200 OK` response code and [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50b17-132">Пример</span><span class="sxs-lookup"><span data-stu-id="50b17-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="50b17-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="50b17-133">Request</span></span>
<span data-ttu-id="50b17-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50b17-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="50b17-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="50b17-135">Response</span></span>
<span data-ttu-id="50b17-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50b17-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2360

{
  "value": {
    "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
    "id": "e03086da-86da-e030-da86-30e0da8630e0",
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
    "usernameSource": "primarySmtpAddress",
    "usernameAADSource": "primarySmtpAddress",
    "userDomainNameSource": "netBiosDomainName",
    "customDomainName": "Custom Domain Name value",
    "accountName": "Account Name value",
    "authenticationMethod": "certificate",
    "blockMovingMessagesToOtherEmailAccounts": true,
    "blockSendingEmailFromThirdPartyApps": true,
    "blockSyncingRecentlyUsedEmailAddresses": true,
    "durationOfEmailToSync": "oneDay",
    "emailAddressSource": "primarySmtpAddress",
    "hostName": "Host Name value",
    "requireSmime": true,
    "smimeEnablePerMessageSwitch": true,
    "smimeEncryptByDefaultEnabled": true,
    "smimeSigningEnabled": true,
    "smimeSigningUserOverrideEnabled": true,
    "smimeEncryptByDefaultUserOverrideEnabled": true,
    "smimeSigningCertificateUserOverrideEnabled": true,
    "smimeEncryptionCertificateUserOverrideEnabled": true,
    "requireSsl": true,
    "useOAuth": true,
    "signingCertificateType": "certificate",
    "encryptionCertificateType": "certificate"
  }
}
```




