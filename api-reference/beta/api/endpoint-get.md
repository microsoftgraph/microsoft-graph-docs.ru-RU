---
title: Получение конечной точки
description: Получение свойств и связей определенного объекта конечной точки.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 4bea857418cf4dc911021da58a465cfc53cc30fc
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289646"
---
# <a name="get-endpoint"></a><span data-ttu-id="d6c06-103">Получение конечной точки</span><span class="sxs-lookup"><span data-stu-id="d6c06-103">Get endpoint</span></span>

<span data-ttu-id="d6c06-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6c06-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6c06-105">Получение свойств и связей определенного объекта [конечной точки](../resources/endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="d6c06-105">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6c06-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6c06-106">Permissions</span></span>
<span data-ttu-id="d6c06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6c06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d6c06-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6c06-109">Permission type</span></span>      | <span data-ttu-id="d6c06-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6c06-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6c06-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6c06-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d6c06-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6c06-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d6c06-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6c06-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6c06-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6c06-114">Not supported.</span></span>    |
|<span data-ttu-id="d6c06-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6c06-115">Application</span></span> | <span data-ttu-id="d6c06-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6c06-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6c06-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6c06-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d6c06-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d6c06-118">Optional query parameters</span></span>
<span data-ttu-id="d6c06-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d6c06-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6c06-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6c06-120">Request headers</span></span>
| <span data-ttu-id="d6c06-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d6c06-121">Name</span></span>      |<span data-ttu-id="d6c06-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d6c06-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d6c06-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6c06-123">Authorization</span></span>  | <span data-ttu-id="d6c06-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6c06-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6c06-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d6c06-126">Request body</span></span>
<span data-ttu-id="d6c06-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d6c06-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6c06-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6c06-128">Response</span></span>

<span data-ttu-id="d6c06-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [конечной точки](../resources/endpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6c06-129">If successful, this method returns a `200 OK` response code and an [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d6c06-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d6c06-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="d6c06-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6c06-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d6c06-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6c06-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
# <a name="c"></a>[<span data-ttu-id="d6c06-133">C#</span><span class="sxs-lookup"><span data-stu-id="d6c06-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6c06-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6c06-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6c06-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6c06-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d6c06-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6c06-136">Response</span></span>
<span data-ttu-id="d6c06-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d6c06-137">Here is an example of the response.</span></span>
><span data-ttu-id="d6c06-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6c06-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.endpoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 208

{
  "capability": "Conversations",
  "providerId": "{Yammer GUID}",
  "providerName": "Yammer",
  "uri": "uri-value",
  "providerResourceId": "Yammer.FeedURL",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Endpoint",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
