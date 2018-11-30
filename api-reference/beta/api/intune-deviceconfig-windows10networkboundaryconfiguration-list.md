---
title: Список windows10NetworkBoundaryConfigurations
description: Свойства списка и связей объектов windows10NetworkBoundaryConfiguration.
ms.openlocfilehash: a9b16a37915ddbea536b0378c521a447852e7ef7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079156"
---
# <a name="list-windows10networkboundaryconfigurations"></a><span data-ttu-id="e3cbe-103">Список windows10NetworkBoundaryConfigurations</span><span class="sxs-lookup"><span data-stu-id="e3cbe-103">List windows10NetworkBoundaryConfigurations</span></span>

> <span data-ttu-id="e3cbe-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e3cbe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3cbe-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3cbe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3cbe-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e3cbe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3cbe-107">Свойства списка и связей объектов [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e3cbe-107">List properties and relationships of the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3cbe-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e3cbe-108">Prerequisites</span></span>
<span data-ttu-id="e3cbe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3cbe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3cbe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3cbe-111">Permission type</span></span>|<span data-ttu-id="e3cbe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3cbe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3cbe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3cbe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3cbe-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3cbe-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e3cbe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3cbe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3cbe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3cbe-116">Not supported.</span></span>|
|<span data-ttu-id="e3cbe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3cbe-117">Application</span></span>|<span data-ttu-id="e3cbe-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3cbe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3cbe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3cbe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e3cbe-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3cbe-120">Request headers</span></span>
|<span data-ttu-id="e3cbe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3cbe-121">Header</span></span>|<span data-ttu-id="e3cbe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e3cbe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3cbe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3cbe-123">Authorization</span></span>|<span data-ttu-id="e3cbe-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e3cbe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3cbe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e3cbe-125">Accept</span></span>|<span data-ttu-id="e3cbe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3cbe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3cbe-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3cbe-127">Request body</span></span>
<span data-ttu-id="e3cbe-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3cbe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3cbe-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3cbe-129">Response</span></span>
<span data-ttu-id="e3cbe-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e3cbe-130">If successful, this method returns a `200 OK` response code and a collection of [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3cbe-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e3cbe-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3cbe-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3cbe-132">Request</span></span>
<span data-ttu-id="e3cbe-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3cbe-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="e3cbe-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3cbe-134">Response</span></span>
<span data-ttu-id="e3cbe-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e3cbe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1617

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
            "@odata.type": "microsoft.graph.iPv6Range",
            "lowerAddress": "Lower Address value",
            "upperAddress": "Upper Address value"
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





