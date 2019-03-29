---
title: Список Виндовсвифиентерприсиапконфигуратионс
description: Список свойств и связей объектов Виндовсвифиентерприсиапконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 42ce39ab3dc42b2fb775f1cad60af502890176fe
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966063"
---
# <a name="list-windowswifienterpriseeapconfigurations"></a><span data-ttu-id="b0485-103">Список Виндовсвифиентерприсиапконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="b0485-103">List windowsWifiEnterpriseEAPConfigurations</span></span>

> <span data-ttu-id="b0485-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0485-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0485-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0485-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0485-106">Список свойств и связей объектов [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b0485-106">List properties and relationships of the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0485-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b0485-107">Prerequisites</span></span>
<span data-ttu-id="b0485-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0485-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0485-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0485-110">Permission type</span></span>|<span data-ttu-id="b0485-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0485-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0485-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0485-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b0485-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0485-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b0485-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0485-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0485-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0485-115">Not supported.</span></span>|
|<span data-ttu-id="b0485-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0485-116">Application</span></span>|<span data-ttu-id="b0485-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0485-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0485-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0485-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b0485-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0485-119">Request headers</span></span>
|<span data-ttu-id="b0485-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0485-120">Header</span></span>|<span data-ttu-id="b0485-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b0485-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0485-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0485-122">Authorization</span></span>|<span data-ttu-id="b0485-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0485-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0485-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b0485-124">Accept</span></span>|<span data-ttu-id="b0485-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b0485-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0485-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0485-126">Request body</span></span>
<span data-ttu-id="b0485-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0485-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0485-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0485-128">Response</span></span>
<span data-ttu-id="b0485-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0485-129">If successful, this method returns a `200 OK` response code and a collection of [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0485-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b0485-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0485-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0485-131">Request</span></span>
<span data-ttu-id="b0485-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0485-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="b0485-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0485-133">Response</span></span>
<span data-ttu-id="b0485-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0485-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




