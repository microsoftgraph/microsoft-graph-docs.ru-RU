---
title: Получите microsoftTunnelServer
description: Чтение свойств и связей объекта microsoftTunnelServer.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9a7bca5595371f9f45bc725b4c7f7f11bae491e6
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864902"
---
# <a name="get-microsofttunnelserver"></a><span data-ttu-id="7e85e-103">Получите microsoftTunnelServer</span><span class="sxs-lookup"><span data-stu-id="7e85e-103">Get microsoftTunnelServer</span></span>

<span data-ttu-id="7e85e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e85e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e85e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e85e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e85e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e85e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e85e-107">Чтение свойств и связей объекта [microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)</span><span class="sxs-lookup"><span data-stu-id="7e85e-107">Read properties and relationships of the [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e85e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7e85e-108">Prerequisites</span></span>
<span data-ttu-id="7e85e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e85e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e85e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e85e-111">Permission type</span></span>|<span data-ttu-id="7e85e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e85e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e85e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e85e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7e85e-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e85e-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|
|<span data-ttu-id="7e85e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e85e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e85e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e85e-116">Not supported.</span></span>|
|<span data-ttu-id="7e85e-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="7e85e-117">Application</span></span>|<span data-ttu-id="7e85e-118">MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e85e-118">MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e85e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e85e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers/{microsoftTunnelServerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7e85e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7e85e-120">Optional query parameters</span></span>
<span data-ttu-id="7e85e-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7e85e-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e85e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e85e-122">Request headers</span></span>
|<span data-ttu-id="7e85e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e85e-123">Header</span></span>|<span data-ttu-id="7e85e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7e85e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e85e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e85e-125">Authorization</span></span>|<span data-ttu-id="7e85e-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e85e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e85e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7e85e-127">Accept</span></span>|<span data-ttu-id="7e85e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7e85e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e85e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e85e-129">Request body</span></span>
<span data-ttu-id="7e85e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e85e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e85e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e85e-131">Response</span></span>
<span data-ttu-id="7e85e-132">В случае успеха этот метод возвращает код отклика и `200 OK` [объект MicrosoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7e85e-132">If successful, this method returns a `200 OK` response code and [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e85e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7e85e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e85e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e85e-134">Request</span></span>
<span data-ttu-id="7e85e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e85e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers/{microsoftTunnelServerId}
```

### <a name="response"></a><span data-ttu-id="7e85e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e85e-136">Response</span></span>
<span data-ttu-id="7e85e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e85e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 286

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftTunnelServer",
    "id": "b5cf0aee-0aee-b5cf-ee0a-cfb5ee0acfb5",
    "displayName": "Display Name value",
    "tunnelServerHealthStatus": "healthy",
    "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
  }
}
```




