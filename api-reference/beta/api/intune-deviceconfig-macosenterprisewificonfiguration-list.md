---
title: Список macOSEnterpriseWiFiConfigurations
description: Список свойств и связей объектов macOSEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a9e7019f55e689be377f9ec1e4a89db0cbcca08b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131283"
---
# <a name="list-macosenterprisewificonfigurations"></a><span data-ttu-id="1c763-103">Список macOSEnterpriseWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="1c763-103">List macOSEnterpriseWiFiConfigurations</span></span>

<span data-ttu-id="1c763-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c763-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c763-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c763-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c763-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c763-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c763-107">Список свойств и связей объектов [macOSEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c763-107">List properties and relationships of the [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c763-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1c763-108">Prerequisites</span></span>
<span data-ttu-id="1c763-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c763-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c763-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c763-111">Permission type</span></span>|<span data-ttu-id="1c763-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c763-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c763-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c763-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c763-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c763-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1c763-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c763-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c763-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c763-116">Not supported.</span></span>|
|<span data-ttu-id="1c763-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1c763-117">Application</span></span>|<span data-ttu-id="1c763-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c763-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c763-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c763-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1c763-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1c763-120">Request headers</span></span>
|<span data-ttu-id="1c763-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c763-121">Header</span></span>|<span data-ttu-id="1c763-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1c763-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c763-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c763-123">Authorization</span></span>|<span data-ttu-id="1c763-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c763-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c763-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1c763-125">Accept</span></span>|<span data-ttu-id="1c763-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1c763-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c763-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c763-127">Request body</span></span>
<span data-ttu-id="1c763-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c763-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c763-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c763-129">Response</span></span>
<span data-ttu-id="1c763-130">В случае успеха этот метод возвращает код ответа и коллекцию объектов `200 OK` [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1c763-130">If successful, this method returns a `200 OK` response code and a collection of [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c763-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1c763-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c763-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c763-132">Request</span></span>
<span data-ttu-id="1c763-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c763-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="1c763-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c763-134">Response</span></span>
<span data-ttu-id="1c763-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c763-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2263

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
      "id": "7a6f9a2e-9a2e-7a6f-2e9a-6f7a2e9a6f7a",
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
      "networkName": "Network Name value",
      "ssid": "Ssid value",
      "connectAutomatically": true,
      "connectWhenNetworkNameIsHidden": true,
      "wiFiSecurityType": "wpaPersonal",
      "proxySettings": "manual",
      "proxyManualAddress": "Proxy Manual Address value",
      "proxyManualPort": 15,
      "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
      "preSharedKey": "Pre Shared Key value",
      "eapType": "leap",
      "eapFastConfiguration": "useProtectedAccessCredential",
      "trustedServerCertificateNames": [
        "Trusted Server Certificate Names value"
      ],
      "authenticationMethod": "usernameAndPassword",
      "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
      "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
    }
  ]
}
```




