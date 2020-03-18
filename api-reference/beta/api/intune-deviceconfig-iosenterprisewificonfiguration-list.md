---
title: Список Иосентерприсевификонфигуратионс
description: Список свойств и связей объектов iosEnterpriseWiFiConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e2558a17fbaf8b8c34a33141d31d4b77d182f7f5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42750896"
---
# <a name="list-iosenterprisewificonfigurations"></a><span data-ttu-id="a0e41-103">Список Иосентерприсевификонфигуратионс</span><span class="sxs-lookup"><span data-stu-id="a0e41-103">List iosEnterpriseWiFiConfigurations</span></span>

> <span data-ttu-id="a0e41-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0e41-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0e41-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0e41-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0e41-106">Список свойств и связей объектов [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a0e41-106">List properties and relationships of the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0e41-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a0e41-107">Prerequisites</span></span>
<span data-ttu-id="a0e41-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0e41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0e41-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0e41-110">Permission type</span></span>|<span data-ttu-id="a0e41-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0e41-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0e41-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0e41-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0e41-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0e41-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a0e41-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0e41-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0e41-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0e41-115">Not supported.</span></span>|
|<span data-ttu-id="a0e41-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="a0e41-116">Application</span></span>|<span data-ttu-id="a0e41-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0e41-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0e41-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0e41-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a0e41-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a0e41-119">Request headers</span></span>
|<span data-ttu-id="a0e41-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a0e41-120">Header</span></span>|<span data-ttu-id="a0e41-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a0e41-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0e41-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0e41-122">Authorization</span></span>|<span data-ttu-id="a0e41-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0e41-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0e41-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a0e41-124">Accept</span></span>|<span data-ttu-id="a0e41-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a0e41-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0e41-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0e41-126">Request body</span></span>
<span data-ttu-id="a0e41-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0e41-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0e41-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a0e41-128">Response</span></span>
<span data-ttu-id="a0e41-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a0e41-129">If successful, this method returns a `200 OK` response code and a collection of [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0e41-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a0e41-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0e41-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0e41-131">Request</span></span>
<span data-ttu-id="a0e41-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0e41-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a0e41-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0e41-133">Response</span></span>
<span data-ttu-id="a0e41-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0e41-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2387

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
      "id": "7593f7ba-f7ba-7593-baf7-9375baf79375",
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
      "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
      "usernameFormatString": "Username Format String value",
      "passwordFormatString": "Password Format String value"
    }
  ]
}
```




