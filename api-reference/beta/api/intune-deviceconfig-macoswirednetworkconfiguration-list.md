---
title: Список macOSWiredNetworkConfigurations
description: Список свойств и связей объектов macOSWiredNetworkConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6dd722d18c80309530c4e513a4b49edc4b48bf6e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155220"
---
# <a name="list-macoswirednetworkconfigurations"></a><span data-ttu-id="1bc0d-103">Список macOSWiredNetworkConfigurations</span><span class="sxs-lookup"><span data-stu-id="1bc0d-103">List macOSWiredNetworkConfigurations</span></span>

<span data-ttu-id="1bc0d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bc0d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bc0d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bc0d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bc0d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1bc0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bc0d-107">Список свойств и связей объектов [macOSWiredNetworkConfiguration.](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1bc0d-107">List properties and relationships of the [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bc0d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1bc0d-108">Prerequisites</span></span>
<span data-ttu-id="1bc0d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bc0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bc0d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bc0d-111">Permission type</span></span>|<span data-ttu-id="1bc0d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bc0d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bc0d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bc0d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1bc0d-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bc0d-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1bc0d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bc0d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bc0d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bc0d-116">Not supported.</span></span>|
|<span data-ttu-id="1bc0d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1bc0d-117">Application</span></span>|<span data-ttu-id="1bc0d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bc0d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bc0d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bc0d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1bc0d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1bc0d-120">Request headers</span></span>
|<span data-ttu-id="1bc0d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1bc0d-121">Header</span></span>|<span data-ttu-id="1bc0d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1bc0d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bc0d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bc0d-123">Authorization</span></span>|<span data-ttu-id="1bc0d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bc0d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bc0d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1bc0d-125">Accept</span></span>|<span data-ttu-id="1bc0d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1bc0d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bc0d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1bc0d-127">Request body</span></span>
<span data-ttu-id="1bc0d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1bc0d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bc0d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bc0d-129">Response</span></span>
<span data-ttu-id="1bc0d-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1bc0d-130">If successful, this method returns a `200 OK` response code and a collection of [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bc0d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1bc0d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bc0d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bc0d-132">Request</span></span>
<span data-ttu-id="1bc0d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bc0d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="1bc0d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bc0d-134">Response</span></span>
<span data-ttu-id="1bc0d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1bc0d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1872

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSWiredNetworkConfiguration",
      "id": "e5a57519-7519-e5a5-1975-a5e51975a5e5",
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
      "networkInterface": "firstActiveEthernet",
      "eapType": "leap",
      "eapFastConfiguration": "useProtectedAccessCredential",
      "trustedServerCertificateNames": [
        "Trusted Server Certificate Names value"
      ],
      "authenticationMethod": "usernameAndPassword",
      "nonEapAuthenticationMethodForEapTtls": "challengeHandshakeAuthenticationProtocol",
      "enableOuterIdentityPrivacy": "Enable Outer Identity Privacy value"
    }
  ]
}
```




