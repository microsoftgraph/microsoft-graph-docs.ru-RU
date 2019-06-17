---
title: Список Андроидворкпрофилинтерприсевификонфигуратионс
description: Список свойств и связей объектов Андроидворкпрофилинтерприсевификонфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e9c03eb4a944738a47ba594efc33803d4c0233e8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34969444"
---
# <a name="list-androidworkprofileenterprisewificonfigurations"></a><span data-ttu-id="5a1f8-103">Список Андроидворкпрофилинтерприсевификонфигуратионс</span><span class="sxs-lookup"><span data-stu-id="5a1f8-103">List androidWorkProfileEnterpriseWiFiConfigurations</span></span>

> <span data-ttu-id="5a1f8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a1f8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a1f8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a1f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a1f8-106">Список свойств и связей объектов [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5a1f8-106">List properties and relationships of the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a1f8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5a1f8-107">Prerequisites</span></span>
<span data-ttu-id="5a1f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a1f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a1f8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a1f8-110">Permission type</span></span>|<span data-ttu-id="5a1f8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a1f8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a1f8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a1f8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a1f8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a1f8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5a1f8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a1f8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a1f8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a1f8-115">Not supported.</span></span>|
|<span data-ttu-id="5a1f8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a1f8-116">Application</span></span>|<span data-ttu-id="5a1f8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a1f8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a1f8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a1f8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5a1f8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a1f8-119">Request headers</span></span>
|<span data-ttu-id="5a1f8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a1f8-120">Header</span></span>|<span data-ttu-id="5a1f8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5a1f8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a1f8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a1f8-122">Authorization</span></span>|<span data-ttu-id="5a1f8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a1f8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a1f8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5a1f8-124">Accept</span></span>|<span data-ttu-id="5a1f8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5a1f8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a1f8-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5a1f8-126">Request body</span></span>
<span data-ttu-id="5a1f8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5a1f8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a1f8-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a1f8-128">Response</span></span>
<span data-ttu-id="5a1f8-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a1f8-129">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a1f8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5a1f8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a1f8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a1f8-131">Request</span></span>
<span data-ttu-id="5a1f8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a1f8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="5a1f8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a1f8-133">Response</span></span>
<span data-ttu-id="5a1f8-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a1f8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1922

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





