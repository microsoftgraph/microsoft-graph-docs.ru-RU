---
title: Get cloudPcConnection
description: Ознакомьтесь с свойствами и отношениями объекта cloudPcConnection.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: eab1d8d41a8c79f011de369fd9e4d2f31d5a7ed6
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402490"
---
# <a name="get-cloudpcconnection"></a><span data-ttu-id="596cc-103">Get cloudPcConnection</span><span class="sxs-lookup"><span data-stu-id="596cc-103">Get cloudPcConnection</span></span>
<span data-ttu-id="596cc-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="596cc-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="596cc-105">Ознакомьтесь с свойствами и отношениями объекта [cloudPcConnection.](../resources/managedtenants-cloudpcconnection.md)</span><span class="sxs-lookup"><span data-stu-id="596cc-105">Read the properties and relationships of a [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="596cc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="596cc-106">Permissions</span></span>
<span data-ttu-id="596cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="596cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="596cc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="596cc-109">Permission type</span></span>|<span data-ttu-id="596cc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="596cc-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="596cc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="596cc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="596cc-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="596cc-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="596cc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="596cc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="596cc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="596cc-114">Not supported.</span></span>|
|<span data-ttu-id="596cc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="596cc-115">Application</span></span>|<span data-ttu-id="596cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="596cc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="596cc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="596cc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcConnections/{cloudPcConnectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="596cc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="596cc-118">Optional query parameters</span></span>
<span data-ttu-id="596cc-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="596cc-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="596cc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="596cc-120">Request headers</span></span>
|<span data-ttu-id="596cc-121">Имя</span><span class="sxs-lookup"><span data-stu-id="596cc-121">Name</span></span>|<span data-ttu-id="596cc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="596cc-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="596cc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="596cc-123">Authorization</span></span>|<span data-ttu-id="596cc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="596cc-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="596cc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="596cc-126">Request body</span></span>
<span data-ttu-id="596cc-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="596cc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="596cc-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="596cc-128">Response</span></span>

<span data-ttu-id="596cc-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="596cc-129">If successful, this method returns a `200 OK` response code and a [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="596cc-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="596cc-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="596cc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="596cc-131">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["86789ee0-e31d-4bee-98e6-6f310bd327bb"],
  "name": "get_cloudpcconnection"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcConnections/86789ee0-e31d-4bee-98e6-6f310bd327bb
```


### <a name="response"></a><span data-ttu-id="596cc-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="596cc-132">Response</span></span>
><span data-ttu-id="596cc-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="596cc-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.cloudPcConnection"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.cloudPcConnection",
  "id": "86789ee0-e31d-4bee-98e6-6f310bd327bb",
  "lastUpdated": "2021-07-11T15:46:28.1243279Z",
  "displayName": "Az-Connection-93ac6d62-7d78-4477-bd43-db5e2013864d",
  "healthCheckStatus": "Failed",
  "tenantId": "aa060093-1e81-45b4-bebc-652713194ef7",
  "tenantDisplayName": "Lucerne Publishing",
  "lastRefreshedDateTime": "2021-07-11T15:46:28.1243279Z"
}
```
