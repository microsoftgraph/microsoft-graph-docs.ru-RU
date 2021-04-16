---
title: Список microsoftTunnelConfigurations
description: Список свойств и связей объектов microsoftTunnelConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f8306e73e96c555e0f88a134bf854a19be5180c7
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863887"
---
# <a name="list-microsofttunnelconfigurations"></a><span data-ttu-id="6d8f7-103">Список microsoftTunnelConfigurations</span><span class="sxs-lookup"><span data-stu-id="6d8f7-103">List microsoftTunnelConfigurations</span></span>

<span data-ttu-id="6d8f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d8f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d8f7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d8f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d8f7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d8f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d8f7-107">Список свойств и связей объектов [microsoftTunnelConfiguration.](../resources/intune-mstunnel-microsofttunnelconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d8f7-107">List properties and relationships of the [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d8f7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6d8f7-108">Prerequisites</span></span>
<span data-ttu-id="6d8f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d8f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d8f7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d8f7-111">Permission type</span></span>|<span data-ttu-id="6d8f7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d8f7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d8f7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d8f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6d8f7-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d8f7-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|
|<span data-ttu-id="6d8f7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d8f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d8f7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d8f7-116">Not supported.</span></span>|
|<span data-ttu-id="6d8f7-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="6d8f7-117">Application</span></span>|<span data-ttu-id="6d8f7-118">MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d8f7-118">MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d8f7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d8f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/microsoftTunnelConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6d8f7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6d8f7-120">Request headers</span></span>
|<span data-ttu-id="6d8f7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d8f7-121">Header</span></span>|<span data-ttu-id="6d8f7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6d8f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d8f7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d8f7-123">Authorization</span></span>|<span data-ttu-id="6d8f7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d8f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d8f7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6d8f7-125">Accept</span></span>|<span data-ttu-id="6d8f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d8f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d8f7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d8f7-127">Request body</span></span>
<span data-ttu-id="6d8f7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6d8f7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d8f7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d8f7-129">Response</span></span>
<span data-ttu-id="6d8f7-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6d8f7-130">If successful, this method returns a `200 OK` response code and a collection of [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d8f7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6d8f7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d8f7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d8f7-132">Request</span></span>
<span data-ttu-id="6d8f7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d8f7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelConfigurations
```

### <a name="response"></a><span data-ttu-id="6d8f7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d8f7-134">Response</span></span>
<span data-ttu-id="6d8f7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d8f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 950

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
      "id": "b8bdb469-b469-b8bd-69b4-bdb869b4bdb8",
      "displayName": "Display Name value",
      "description": "Description value",
      "network": "Network value",
      "dnsServers": [
        "Dns Servers value"
      ],
      "defaultDomainSuffix": "Default Domain Suffix value",
      "routesInclude": [
        "Routes Include value"
      ],
      "routesExclude": [
        "Routes Exclude value"
      ],
      "splitDNS": [
        "Split DNS value"
      ],
      "listenPort": 10,
      "advancedSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




