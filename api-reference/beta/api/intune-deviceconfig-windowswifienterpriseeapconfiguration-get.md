---
title: Получение windowsWifiEnterpriseEAPConfiguration
description: Чтение свойства и связи объекта windowsWifiEnterpriseEAPConfiguration.
ms.openlocfilehash: 8d4b718bdae430e21386a3fa035fe153340acfa6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078801"
---
# <a name="get-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="12ddb-103">Получение windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="12ddb-103">Get windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="12ddb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="12ddb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12ddb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12ddb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12ddb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="12ddb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12ddb-107">Чтение свойства и связи объекта [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="12ddb-107">Read properties and relationships of the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12ddb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="12ddb-108">Prerequisites</span></span>
<span data-ttu-id="12ddb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12ddb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12ddb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12ddb-111">Permission type</span></span>|<span data-ttu-id="12ddb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12ddb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12ddb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12ddb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12ddb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="12ddb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="12ddb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12ddb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12ddb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12ddb-116">Not supported.</span></span>|
|<span data-ttu-id="12ddb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12ddb-117">Application</span></span>|<span data-ttu-id="12ddb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12ddb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12ddb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12ddb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12ddb-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="12ddb-120">Optional query parameters</span></span>
<span data-ttu-id="12ddb-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="12ddb-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="12ddb-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12ddb-122">Request headers</span></span>
|<span data-ttu-id="12ddb-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12ddb-123">Header</span></span>|<span data-ttu-id="12ddb-124">Значение</span><span class="sxs-lookup"><span data-stu-id="12ddb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12ddb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="12ddb-125">Authorization</span></span>|<span data-ttu-id="12ddb-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="12ddb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12ddb-127">Accept</span><span class="sxs-lookup"><span data-stu-id="12ddb-127">Accept</span></span>|<span data-ttu-id="12ddb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="12ddb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12ddb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12ddb-129">Request body</span></span>
<span data-ttu-id="12ddb-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12ddb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12ddb-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="12ddb-131">Response</span></span>
<span data-ttu-id="12ddb-132">Успешно завершена, этот метод возвращает `200 OK` объект [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="12ddb-132">If successful, this method returns a `200 OK` response code and [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12ddb-133">Пример</span><span class="sxs-lookup"><span data-stu-id="12ddb-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="12ddb-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="12ddb-134">Request</span></span>
<span data-ttu-id="12ddb-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12ddb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="12ddb-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="12ddb-136">Response</span></span>
<span data-ttu-id="12ddb-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="12ddb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1773

{
  "value": {
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
}
```





