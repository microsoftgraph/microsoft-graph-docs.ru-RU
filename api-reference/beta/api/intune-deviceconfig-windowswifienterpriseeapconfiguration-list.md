---
title: Список windowsWifiEnterpriseEAPConfigurations
description: Свойства списка и связей объектов windowsWifiEnterpriseEAPConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3724a7b5facd634c1457ccbd218ddfdb6505ce68
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978090"
---
# <a name="list-windowswifienterpriseeapconfigurations"></a><span data-ttu-id="9fccf-103">Список windowsWifiEnterpriseEAPConfigurations</span><span class="sxs-lookup"><span data-stu-id="9fccf-103">List windowsWifiEnterpriseEAPConfigurations</span></span>

> <span data-ttu-id="9fccf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9fccf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9fccf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fccf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9fccf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9fccf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9fccf-107">Свойства списка и связей объектов [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9fccf-107">List properties and relationships of the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9fccf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9fccf-108">Prerequisites</span></span>
<span data-ttu-id="9fccf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fccf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fccf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9fccf-111">Permission type</span></span>|<span data-ttu-id="9fccf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9fccf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fccf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fccf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9fccf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fccf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9fccf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fccf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fccf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fccf-116">Not supported.</span></span>|
|<span data-ttu-id="9fccf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9fccf-117">Application</span></span>|<span data-ttu-id="9fccf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fccf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fccf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fccf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9fccf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9fccf-120">Request headers</span></span>
|<span data-ttu-id="9fccf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9fccf-121">Header</span></span>|<span data-ttu-id="9fccf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9fccf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fccf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fccf-123">Authorization</span></span>|<span data-ttu-id="9fccf-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9fccf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fccf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9fccf-125">Accept</span></span>|<span data-ttu-id="9fccf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9fccf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fccf-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9fccf-127">Request body</span></span>
<span data-ttu-id="9fccf-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9fccf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fccf-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="9fccf-129">Response</span></span>
<span data-ttu-id="9fccf-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9fccf-130">If successful, this method returns a `200 OK` response code and a collection of [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fccf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9fccf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9fccf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fccf-132">Request</span></span>
<span data-ttu-id="9fccf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fccf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="9fccf-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="9fccf-134">Response</span></span>
<span data-ttu-id="9fccf-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9fccf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1865

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
      "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "preSharedKey": "Pre Shared Key value",
      "wifiSecurityType": "wpaPersonal",
      "meteredConnectionLimit": "fixed",
      "ssid": "Ssid value",
      "networkName": "Network Name value",
      "connectAutomatically": true,
      "connectToPreferredNetwork": true,
      "connectWhenNetworkNameIsHidden": true,
      "proxySetting": "manual",
      "proxyManualAddress": "Proxy Manual Address value",
      "proxyManualPort": 15,
      "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
      "forceFIPSCompliance": true,
      "networkSingleSignOn": "prelogon",
      "maximumAuthenticationTimeoutInSeconds": 5,
      "promptForAdditionalAuthenticationCredentials": true,
      "enablePairwiseMasterKeyCaching": true,
      "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
      "maximumNumberOfPairwiseMasterKeysInCache": 8,
      "enablePreAuthentication": true,
      "maximumPreAuthenticationAttempts": 0,
      "eapType": "leap",
      "trustedServerCertificateNames": [
        "Trusted Server Certificate Names value"
      ],
      "authenticationMethod": "usernameAndPassword",
      "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
      "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
    }
  ]
}
```





