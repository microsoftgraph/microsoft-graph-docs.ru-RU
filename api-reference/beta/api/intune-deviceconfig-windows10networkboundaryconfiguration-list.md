---
title: Список windows10NetworkBoundaryConfigurations
description: Список свойств и связей объектов windows10NetworkBoundaryConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b6ee82581f75da8285f006c6885cbde28d2ec30e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49205050"
---
# <a name="list-windows10networkboundaryconfigurations"></a><span data-ttu-id="52aa2-103">Список windows10NetworkBoundaryConfigurations</span><span class="sxs-lookup"><span data-stu-id="52aa2-103">List windows10NetworkBoundaryConfigurations</span></span>

<span data-ttu-id="52aa2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52aa2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52aa2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52aa2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52aa2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52aa2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52aa2-107">Список свойств и связей объектов [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="52aa2-107">List properties and relationships of the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52aa2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="52aa2-108">Prerequisites</span></span>
<span data-ttu-id="52aa2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52aa2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52aa2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52aa2-111">Permission type</span></span>|<span data-ttu-id="52aa2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="52aa2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52aa2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52aa2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52aa2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="52aa2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="52aa2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52aa2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52aa2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52aa2-116">Not supported.</span></span>|
|<span data-ttu-id="52aa2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="52aa2-117">Application</span></span>|<span data-ttu-id="52aa2-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="52aa2-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52aa2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52aa2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="52aa2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="52aa2-120">Request headers</span></span>
|<span data-ttu-id="52aa2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52aa2-121">Header</span></span>|<span data-ttu-id="52aa2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="52aa2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52aa2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52aa2-123">Authorization</span></span>|<span data-ttu-id="52aa2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52aa2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52aa2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="52aa2-125">Accept</span></span>|<span data-ttu-id="52aa2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52aa2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52aa2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52aa2-127">Request body</span></span>
<span data-ttu-id="52aa2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52aa2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52aa2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="52aa2-129">Response</span></span>
<span data-ttu-id="52aa2-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="52aa2-130">If successful, this method returns a `200 OK` response code and a collection of [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52aa2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="52aa2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="52aa2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="52aa2-132">Request</span></span>
<span data-ttu-id="52aa2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52aa2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="52aa2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="52aa2-134">Response</span></span>
<span data-ttu-id="52aa2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52aa2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2368

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
      "id": "afbc9e01-9e01-afbc-019e-bcaf019ebcaf",
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
      "windowsNetworkIsolationPolicy": {
        "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy",
        "enterpriseNetworkDomainNames": [
          "Enterprise Network Domain Names value"
        ],
        "enterpriseCloudResources": [
          {
            "@odata.type": "microsoft.graph.proxiedDomain",
            "ipAddressOrFQDN": "Ip Address Or FQDN value",
            "proxy": "Proxy value"
          }
        ],
        "enterpriseIPRanges": [
          {
            "@odata.type": "microsoft.graph.ipRange"
          }
        ],
        "enterpriseInternalProxyServers": [
          "Enterprise Internal Proxy Servers value"
        ],
        "enterpriseIPRangesAreAuthoritative": true,
        "enterpriseProxyServers": [
          "Enterprise Proxy Servers value"
        ],
        "enterpriseProxyServersAreAuthoritative": true,
        "neutralDomainResources": [
          "Neutral Domain Resources value"
        ]
      }
    }
  ]
}
```




