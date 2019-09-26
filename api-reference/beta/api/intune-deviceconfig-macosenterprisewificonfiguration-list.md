---
title: Список Макосентерприсевификонфигуратионс
description: Список свойств и связей объектов macOSEnterpriseWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3f424fb12483c58ff37534245939039cd56a7df8
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37178587"
---
# <a name="list-macosenterprisewificonfigurations"></a><span data-ttu-id="3ab1f-103">Список Макосентерприсевификонфигуратионс</span><span class="sxs-lookup"><span data-stu-id="3ab1f-103">List macOSEnterpriseWiFiConfigurations</span></span>

> <span data-ttu-id="3ab1f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ab1f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ab1f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ab1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ab1f-106">Список свойств и связей объектов [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3ab1f-106">List properties and relationships of the [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ab1f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3ab1f-107">Prerequisites</span></span>
<span data-ttu-id="3ab1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ab1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ab1f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ab1f-110">Permission type</span></span>|<span data-ttu-id="3ab1f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ab1f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ab1f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ab1f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3ab1f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ab1f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3ab1f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ab1f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ab1f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ab1f-115">Not supported.</span></span>|
|<span data-ttu-id="3ab1f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ab1f-116">Application</span></span>|<span data-ttu-id="3ab1f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ab1f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ab1f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ab1f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3ab1f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ab1f-119">Request headers</span></span>
|<span data-ttu-id="3ab1f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ab1f-120">Header</span></span>|<span data-ttu-id="3ab1f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3ab1f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ab1f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ab1f-122">Authorization</span></span>|<span data-ttu-id="3ab1f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ab1f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ab1f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3ab1f-124">Accept</span></span>|<span data-ttu-id="3ab1f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3ab1f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ab1f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3ab1f-126">Request body</span></span>
<span data-ttu-id="3ab1f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ab1f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ab1f-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ab1f-128">Response</span></span>
<span data-ttu-id="3ab1f-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3ab1f-129">If successful, this method returns a `200 OK` response code and a collection of [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ab1f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3ab1f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ab1f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ab1f-131">Request</span></span>
<span data-ttu-id="3ab1f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ab1f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="3ab1f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ab1f-133">Response</span></span>
<span data-ttu-id="3ab1f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ab1f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




