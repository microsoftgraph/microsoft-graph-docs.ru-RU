---
title: Перечисление конечных точек
description: Получение списка объектов конечной точки.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8bf4d52ebe1e59efeb2b47afcf33f028c91567be
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43397019"
---
# <a name="list-endpoints"></a><span data-ttu-id="0db29-103">Перечисление конечных точек</span><span class="sxs-lookup"><span data-stu-id="0db29-103">List endpoints</span></span>

<span data-ttu-id="0db29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0db29-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0db29-105">Получение списка объектов [конечной точки](../resources/endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="0db29-105">Retrieve a list of [endpoint](../resources/endpoint.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0db29-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0db29-106">Permissions</span></span>
<span data-ttu-id="0db29-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0db29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0db29-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0db29-109">Permission type</span></span>      | <span data-ttu-id="0db29-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0db29-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0db29-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0db29-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0db29-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0db29-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0db29-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0db29-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0db29-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0db29-114">Not supported.</span></span>    |
|<span data-ttu-id="0db29-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0db29-115">Application</span></span> | <span data-ttu-id="0db29-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0db29-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0db29-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0db29-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0db29-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0db29-118">Optional query parameters</span></span>
<span data-ttu-id="0db29-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0db29-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0db29-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0db29-120">Request headers</span></span>
| <span data-ttu-id="0db29-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0db29-121">Name</span></span>      |<span data-ttu-id="0db29-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0db29-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0db29-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0db29-123">Authorization</span></span>  | <span data-ttu-id="0db29-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0db29-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="0db29-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0db29-126">Content-Type</span></span>   | <span data-ttu-id="0db29-127">Приложение/JSON</span><span class="sxs-lookup"><span data-stu-id="0db29-127">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0db29-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0db29-128">Request body</span></span>
<span data-ttu-id="0db29-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0db29-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0db29-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="0db29-130">Response</span></span>

<span data-ttu-id="0db29-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Endpoint](../resources/endpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0db29-131">If successful, this method returns a `200 OK` response code and collection of [Endpoint](../resources/endpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0db29-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0db29-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0db29-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0db29-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0db29-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0db29-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints
```
# <a name="c"></a>[<span data-ttu-id="0db29-135">C#</span><span class="sxs-lookup"><span data-stu-id="0db29-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0db29-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0db29-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0db29-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0db29-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0db29-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0db29-138">Response</span></span>
<span data-ttu-id="0db29-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0db29-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.endpoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 261

{
  "value": [
    {
      "capability": "Conversations",
      "providerId": "{Yammer GUID}",
      "providerName": "Yammer",
      "uri": "uri-value",
      "providerResourceId": "Yammer.FeedURL",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List endpoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
