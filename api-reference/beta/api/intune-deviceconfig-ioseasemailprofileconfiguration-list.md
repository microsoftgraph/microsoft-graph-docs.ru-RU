---
title: Список iosEasEmailProfileConfigurations
description: Список свойств и связей объектов iosEasEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 020bd876e8b3f60455ba5da783e7119cdb7b5fc1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129988"
---
# <a name="list-ioseasemailprofileconfigurations"></a><span data-ttu-id="8743b-103">Список iosEasEmailProfileConfigurations</span><span class="sxs-lookup"><span data-stu-id="8743b-103">List iosEasEmailProfileConfigurations</span></span>

<span data-ttu-id="8743b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8743b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8743b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8743b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8743b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8743b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8743b-107">Список свойств и связей объектов [iosEasEmailProfileConfiguration.](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8743b-107">List properties and relationships of the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8743b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8743b-108">Prerequisites</span></span>
<span data-ttu-id="8743b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8743b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8743b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8743b-111">Permission type</span></span>|<span data-ttu-id="8743b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8743b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8743b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8743b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8743b-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8743b-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8743b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8743b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8743b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8743b-116">Not supported.</span></span>|
|<span data-ttu-id="8743b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8743b-117">Application</span></span>|<span data-ttu-id="8743b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8743b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8743b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8743b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8743b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8743b-120">Request headers</span></span>
|<span data-ttu-id="8743b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8743b-121">Header</span></span>|<span data-ttu-id="8743b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8743b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8743b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8743b-123">Authorization</span></span>|<span data-ttu-id="8743b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8743b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8743b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8743b-125">Accept</span></span>|<span data-ttu-id="8743b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8743b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8743b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8743b-127">Request body</span></span>
<span data-ttu-id="8743b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8743b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8743b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8743b-129">Response</span></span>
<span data-ttu-id="8743b-130">В случае успеха этот метод возвращает код ответа и коллекцию объектов `200 OK` [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8743b-130">If successful, this method returns a `200 OK` response code and a collection of [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8743b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8743b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8743b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8743b-132">Request</span></span>
<span data-ttu-id="8743b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8743b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="8743b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8743b-134">Response</span></span>
<span data-ttu-id="8743b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8743b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2628

{
  "value": [
    {
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
      "easServices": "calendars",
      "easServicesUserOverrideEnabled": true,
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
      "encryptionCertificateType": "certificate",
      "perAppVPNProfileId": "Per App VPNProfile Id value"
    }
  ]
}
```




