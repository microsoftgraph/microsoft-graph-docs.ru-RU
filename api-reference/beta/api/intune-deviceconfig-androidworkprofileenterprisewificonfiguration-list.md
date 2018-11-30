---
title: Список androidWorkProfileEnterpriseWiFiConfigurations
description: Свойства списка и связей объектов androidWorkProfileEnterpriseWiFiConfiguration.
ms.openlocfilehash: 23af237e69f50256406b17491d2fb6297b631ffd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076254"
---
# <a name="list-androidworkprofileenterprisewificonfigurations"></a><span data-ttu-id="6e7de-103">Список androidWorkProfileEnterpriseWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="6e7de-103">List androidWorkProfileEnterpriseWiFiConfigurations</span></span>

> <span data-ttu-id="6e7de-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6e7de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e7de-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e7de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e7de-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6e7de-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6e7de-107">Свойства списка и связей объектов [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6e7de-107">List properties and relationships of the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6e7de-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6e7de-108">Prerequisites</span></span>
<span data-ttu-id="6e7de-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e7de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e7de-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e7de-111">Permission type</span></span>|<span data-ttu-id="6e7de-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e7de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e7de-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e7de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e7de-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e7de-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6e7de-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e7de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e7de-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e7de-116">Not supported.</span></span>|
|<span data-ttu-id="6e7de-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e7de-117">Application</span></span>|<span data-ttu-id="6e7de-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e7de-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e7de-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e7de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6e7de-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e7de-120">Request headers</span></span>
|<span data-ttu-id="6e7de-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e7de-121">Header</span></span>|<span data-ttu-id="6e7de-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6e7de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e7de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e7de-123">Authorization</span></span>|<span data-ttu-id="6e7de-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6e7de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e7de-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6e7de-125">Accept</span></span>|<span data-ttu-id="6e7de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e7de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e7de-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e7de-127">Request body</span></span>
<span data-ttu-id="6e7de-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e7de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e7de-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e7de-129">Response</span></span>
<span data-ttu-id="6e7de-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6e7de-130">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e7de-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6e7de-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6e7de-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e7de-132">Request</span></span>
<span data-ttu-id="6e7de-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e7de-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="6e7de-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e7de-134">Response</span></span>
<span data-ttu-id="6e7de-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6e7de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1065

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
      "id": "c48cd726-d726-c48c-26d7-8cc426d78cc4",
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
      "wiFiSecurityType": "wpaEnterprise",
      "eapType": "eapTtls",
      "authenticationMethod": "usernameAndPassword",
      "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
      "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
      "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
    }
  ]
}
```





