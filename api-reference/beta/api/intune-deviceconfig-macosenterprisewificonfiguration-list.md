---
title: Список macOSEnterpriseWiFiConfigurations
description: Свойства списка и связей объектов macOSEnterpriseWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 092ff0ec37482981f487bb9c76d7ec486064fe08
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816872"
---
# <a name="list-macosenterprisewificonfigurations"></a><span data-ttu-id="0a405-103">Список macOSEnterpriseWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="0a405-103">List macOSEnterpriseWiFiConfigurations</span></span>

> <span data-ttu-id="0a405-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0a405-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a405-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a405-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a405-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0a405-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a405-107">Свойства списка и связей объектов [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0a405-107">List properties and relationships of the [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0a405-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0a405-108">Prerequisites</span></span>
<span data-ttu-id="0a405-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a405-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a405-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a405-111">Permission type</span></span>|<span data-ttu-id="0a405-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a405-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a405-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a405-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a405-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a405-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0a405-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a405-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a405-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a405-116">Not supported.</span></span>|
|<span data-ttu-id="0a405-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a405-117">Application</span></span>|<span data-ttu-id="0a405-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a405-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a405-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a405-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0a405-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a405-120">Request headers</span></span>
|<span data-ttu-id="0a405-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a405-121">Header</span></span>|<span data-ttu-id="0a405-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0a405-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a405-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a405-123">Authorization</span></span>|<span data-ttu-id="0a405-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0a405-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a405-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0a405-125">Accept</span></span>|<span data-ttu-id="0a405-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a405-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a405-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0a405-127">Request body</span></span>
<span data-ttu-id="0a405-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0a405-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a405-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a405-129">Response</span></span>
<span data-ttu-id="0a405-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0a405-130">If successful, this method returns a `200 OK` response code and a collection of [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a405-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0a405-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0a405-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a405-132">Request</span></span>
<span data-ttu-id="0a405-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a405-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="0a405-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a405-134">Response</span></span>
<span data-ttu-id="0a405-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0a405-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1406

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





