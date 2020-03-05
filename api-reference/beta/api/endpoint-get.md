---
title: Получение конечной точки
description: Получение свойств и связей определенного объекта конечной точки.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 15ccf9b6a250cf75d613826899a30a0c8e20b420
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42423492"
---
# <a name="get-endpoint"></a><span data-ttu-id="34e6e-103">Получение конечной точки</span><span class="sxs-lookup"><span data-stu-id="34e6e-103">Get endpoint</span></span>

<span data-ttu-id="34e6e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="34e6e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34e6e-105">Получение свойств и связей определенного объекта [конечной точки](../resources/endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="34e6e-105">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="34e6e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34e6e-106">Permissions</span></span>
<span data-ttu-id="34e6e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34e6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="34e6e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34e6e-109">Permission type</span></span>      | <span data-ttu-id="34e6e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34e6e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34e6e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34e6e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="34e6e-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34e6e-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="34e6e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34e6e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34e6e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34e6e-114">Not supported.</span></span>    |
|<span data-ttu-id="34e6e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34e6e-115">Application</span></span> | <span data-ttu-id="34e6e-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34e6e-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="34e6e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34e6e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="34e6e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="34e6e-118">Optional query parameters</span></span>
<span data-ttu-id="34e6e-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="34e6e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34e6e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34e6e-120">Request headers</span></span>
| <span data-ttu-id="34e6e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="34e6e-121">Name</span></span>      |<span data-ttu-id="34e6e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="34e6e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="34e6e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34e6e-123">Authorization</span></span>  | <span data-ttu-id="34e6e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34e6e-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="34e6e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="34e6e-126">Content-Type</span></span>   | <span data-ttu-id="34e6e-127">Приложение/JSON</span><span class="sxs-lookup"><span data-stu-id="34e6e-127">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="34e6e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34e6e-128">Request body</span></span>
<span data-ttu-id="34e6e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="34e6e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34e6e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="34e6e-130">Response</span></span>

<span data-ttu-id="34e6e-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [конечной точки](../resources/endpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="34e6e-131">If successful, this method returns a `200 OK` response code and [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="34e6e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="34e6e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34e6e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="34e6e-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="34e6e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="34e6e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
# <a name="c"></a>[<span data-ttu-id="34e6e-135">C#</span><span class="sxs-lookup"><span data-stu-id="34e6e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="34e6e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34e6e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="34e6e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34e6e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="34e6e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="34e6e-138">Response</span></span>
<span data-ttu-id="34e6e-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="34e6e-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
