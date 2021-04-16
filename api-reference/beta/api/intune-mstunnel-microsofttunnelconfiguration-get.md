---
title: Получите microsoftTunnelConfiguration
description: Чтение свойств и связей объекта microsoftTunnelConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b9df82d2db35a54842a76ccc3478e3fe6e1ddb96
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867555"
---
# <a name="get-microsofttunnelconfiguration"></a><span data-ttu-id="b2bad-103">Получите microsoftTunnelConfiguration</span><span class="sxs-lookup"><span data-stu-id="b2bad-103">Get microsoftTunnelConfiguration</span></span>

<span data-ttu-id="b2bad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2bad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2bad-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2bad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2bad-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2bad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2bad-107">Чтение свойств и связей объекта [microsoftTunnelConfiguration.](../resources/intune-mstunnel-microsofttunnelconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2bad-107">Read properties and relationships of the [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2bad-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b2bad-108">Prerequisites</span></span>
<span data-ttu-id="b2bad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2bad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2bad-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2bad-111">Permission type</span></span>|<span data-ttu-id="b2bad-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2bad-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2bad-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2bad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2bad-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2bad-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|
|<span data-ttu-id="b2bad-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2bad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2bad-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2bad-116">Not supported.</span></span>|
|<span data-ttu-id="b2bad-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="b2bad-117">Application</span></span>|<span data-ttu-id="b2bad-118">MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2bad-118">MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2bad-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2bad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
GET /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b2bad-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b2bad-120">Optional query parameters</span></span>
<span data-ttu-id="b2bad-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b2bad-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b2bad-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2bad-122">Request headers</span></span>
|<span data-ttu-id="b2bad-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2bad-123">Header</span></span>|<span data-ttu-id="b2bad-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b2bad-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2bad-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2bad-125">Authorization</span></span>|<span data-ttu-id="b2bad-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2bad-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2bad-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b2bad-127">Accept</span></span>|<span data-ttu-id="b2bad-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b2bad-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2bad-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2bad-129">Request body</span></span>
<span data-ttu-id="b2bad-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2bad-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2bad-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2bad-131">Response</span></span>
<span data-ttu-id="b2bad-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b2bad-132">If successful, this method returns a `200 OK` response code and [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2bad-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b2bad-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2bad-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2bad-134">Request</span></span>
<span data-ttu-id="b2bad-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2bad-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b2bad-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2bad-136">Response</span></span>
<span data-ttu-id="b2bad-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2bad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 876

{
  "value": {
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
}
```




