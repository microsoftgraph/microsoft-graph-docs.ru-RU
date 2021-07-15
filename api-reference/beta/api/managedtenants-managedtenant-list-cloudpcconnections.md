---
title: Список cloudPcConnections
description: Получите список объектов cloudPcConnection и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: e0b8ab55319ed04d64318d422b36a57550dc29a0
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441594"
---
# <a name="list-cloudpcconnections"></a><span data-ttu-id="81019-103">Список cloudPcConnections</span><span class="sxs-lookup"><span data-stu-id="81019-103">List cloudPcConnections</span></span>
<span data-ttu-id="81019-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="81019-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81019-105">Получите список объектов [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="81019-105">Get a list of the [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="81019-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81019-106">Permissions</span></span>
<span data-ttu-id="81019-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81019-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81019-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81019-109">Permission type</span></span>|<span data-ttu-id="81019-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81019-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81019-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81019-111">Delegated (work or school account)</span></span>|<span data-ttu-id="81019-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81019-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="81019-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81019-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81019-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81019-114">Not supported.</span></span>|
|<span data-ttu-id="81019-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81019-115">Application</span></span>|<span data-ttu-id="81019-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81019-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81019-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81019-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcConnections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81019-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="81019-118">Optional query parameters</span></span>
<span data-ttu-id="81019-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="81019-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81019-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81019-120">Request headers</span></span>
|<span data-ttu-id="81019-121">Имя</span><span class="sxs-lookup"><span data-stu-id="81019-121">Name</span></span>|<span data-ttu-id="81019-122">Описание</span><span class="sxs-lookup"><span data-stu-id="81019-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="81019-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81019-123">Authorization</span></span>|<span data-ttu-id="81019-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81019-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81019-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81019-126">Request body</span></span>
<span data-ttu-id="81019-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="81019-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81019-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="81019-128">Response</span></span>

<span data-ttu-id="81019-129">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="81019-129">If successful, this method returns a `200 OK` response code and a collection of [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81019-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="81019-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="81019-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="81019-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="81019-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="81019-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcconnection"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcConnections
```
# <a name="c"></a>[<span data-ttu-id="81019-133">C#</span><span class="sxs-lookup"><span data-stu-id="81019-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcconnection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81019-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81019-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcconnection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81019-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81019-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcconnection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81019-136">Java</span><span class="sxs-lookup"><span data-stu-id="81019-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcconnection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="81019-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="81019-137">Response</span></span>
><span data-ttu-id="81019-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="81019-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.cloudPcConnection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/cloudPcConnections",
  "value": [
    {
      "id": "021bd3a9-59c6-4503-b408-c326a98f238f",
      "lastUpdated": "2021-07-11T18:02:16.6450704Z",
      "displayName": "RunnerPlus-Az-Connection",
      "organizationId": "0b9701e1-f1ae-4f15-bd67-f4f591595454",
      "organizationDisplayName": "Terra Firm",
      "healthCheckStatus": "Passed",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee",
      "lastRefreshedDateTime": "2021-07-11T18:02:16.6450704Z"
    }
  ]
}
```
