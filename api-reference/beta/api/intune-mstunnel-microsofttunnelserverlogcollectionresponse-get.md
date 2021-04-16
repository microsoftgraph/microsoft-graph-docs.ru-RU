---
title: Получите microsoftTunnelServerLogCollectionResponse
description: Чтение свойств и связей объекта microsoftTunnelServerLogCollectionResponse.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3bc5f9222da502b19ccbb677fb57ba2f31e6ee28
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864825"
---
# <a name="get-microsofttunnelserverlogcollectionresponse"></a><span data-ttu-id="1036a-103">Получите microsoftTunnelServerLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="1036a-103">Get microsoftTunnelServerLogCollectionResponse</span></span>

<span data-ttu-id="1036a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1036a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1036a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1036a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1036a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1036a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1036a-107">Чтение свойств и связей объекта [microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)</span><span class="sxs-lookup"><span data-stu-id="1036a-107">Read properties and relationships of the [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1036a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1036a-108">Prerequisites</span></span>
<span data-ttu-id="1036a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1036a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1036a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1036a-111">Permission type</span></span>|<span data-ttu-id="1036a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1036a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1036a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1036a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1036a-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1036a-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|
|<span data-ttu-id="1036a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1036a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1036a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1036a-116">Not supported.</span></span>|
|<span data-ttu-id="1036a-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="1036a-117">Application</span></span>|<span data-ttu-id="1036a-118">MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1036a-118">MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1036a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1036a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/microsoftTunnelServerLogCollectionResponses/{microsoftTunnelServerLogCollectionResponseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1036a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1036a-120">Optional query parameters</span></span>
<span data-ttu-id="1036a-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1036a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1036a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1036a-122">Request headers</span></span>
|<span data-ttu-id="1036a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1036a-123">Header</span></span>|<span data-ttu-id="1036a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="1036a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1036a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1036a-125">Authorization</span></span>|<span data-ttu-id="1036a-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1036a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1036a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1036a-127">Accept</span></span>|<span data-ttu-id="1036a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1036a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1036a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1036a-129">Request body</span></span>
<span data-ttu-id="1036a-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1036a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1036a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1036a-131">Response</span></span>
<span data-ttu-id="1036a-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1036a-132">If successful, this method returns a `200 OK` response code and [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1036a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1036a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1036a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1036a-134">Request</span></span>
<span data-ttu-id="1036a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1036a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelServerLogCollectionResponses/{microsoftTunnelServerLogCollectionResponseId}
```

### <a name="response"></a><span data-ttu-id="1036a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1036a-136">Response</span></span>
<span data-ttu-id="1036a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1036a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftTunnelServerLogCollectionResponse",
    "id": "05dcc2e9-c2e9-05dc-e9c2-dc05e9c2dc05",
    "status": "completed",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
    "sizeInBytes": 11
  }
}
```




