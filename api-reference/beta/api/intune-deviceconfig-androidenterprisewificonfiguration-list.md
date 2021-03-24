---
title: Список androidEnterpriseWiFiConfigurations
description: Список свойств и связей объектов AndroidEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 833118ba2f57664ea6570dda6b80f556b07bd773
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130492"
---
# <a name="list-androidenterprisewificonfigurations"></a><span data-ttu-id="a69a1-103">Список androidEnterpriseWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="a69a1-103">List androidEnterpriseWiFiConfigurations</span></span>

<span data-ttu-id="a69a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a69a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a69a1-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a69a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a69a1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a69a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a69a1-107">Список свойств и связей объектов [AndroidEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a69a1-107">List properties and relationships of the [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a69a1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a69a1-108">Prerequisites</span></span>
<span data-ttu-id="a69a1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a69a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a69a1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a69a1-111">Permission type</span></span>|<span data-ttu-id="a69a1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a69a1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a69a1-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a69a1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a69a1-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a69a1-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a69a1-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a69a1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a69a1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a69a1-116">Not supported.</span></span>|
|<span data-ttu-id="a69a1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a69a1-117">Application</span></span>|<span data-ttu-id="a69a1-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a69a1-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a69a1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a69a1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a69a1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a69a1-120">Request headers</span></span>
|<span data-ttu-id="a69a1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a69a1-121">Header</span></span>|<span data-ttu-id="a69a1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a69a1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a69a1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a69a1-123">Authorization</span></span>|<span data-ttu-id="a69a1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a69a1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a69a1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a69a1-125">Accept</span></span>|<span data-ttu-id="a69a1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a69a1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a69a1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a69a1-127">Request body</span></span>
<span data-ttu-id="a69a1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a69a1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a69a1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a69a1-129">Response</span></span>
<span data-ttu-id="a69a1-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a69a1-130">If successful, this method returns a `200 OK` response code and a collection of [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a69a1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a69a1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a69a1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a69a1-132">Request</span></span>
<span data-ttu-id="a69a1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a69a1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a69a1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a69a1-134">Response</span></span>
<span data-ttu-id="a69a1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a69a1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2084

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
      "id": "972edff4-dff4-972e-f4df-2e97f4df2e97",
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
      "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
      "usernameFormatString": "Username Format String value",
      "passwordFormatString": "Password Format String value",
      "preSharedKey": "Pre Shared Key value"
    }
  ]
}
```




