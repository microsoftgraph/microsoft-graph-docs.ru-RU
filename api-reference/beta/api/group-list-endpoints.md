---
title: Перечисление конечных точек
description: Извлечение списка конечных объектов.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: be99b570d16193aa461fa8cc2d8cc3646d0e55a1
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681624"
---
# <a name="list-endpoints"></a><span data-ttu-id="c44df-103">Перечисление конечных точек</span><span class="sxs-lookup"><span data-stu-id="c44df-103">List endpoints</span></span>

<span data-ttu-id="c44df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c44df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c44df-105">Извлечение списка [конечных объектов.](../resources/endpoint.md)</span><span class="sxs-lookup"><span data-stu-id="c44df-105">Retrieve a list of [endpoint](../resources/endpoint.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c44df-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c44df-106">Permissions</span></span>
<span data-ttu-id="c44df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c44df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c44df-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c44df-109">Permission type</span></span>      | <span data-ttu-id="c44df-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c44df-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c44df-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c44df-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c44df-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c44df-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c44df-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c44df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c44df-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c44df-114">Not supported.</span></span>    |
|<span data-ttu-id="c44df-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c44df-115">Application</span></span> | <span data-ttu-id="c44df-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c44df-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c44df-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c44df-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c44df-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c44df-118">Optional query parameters</span></span>
<span data-ttu-id="c44df-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c44df-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c44df-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c44df-120">Request headers</span></span>
| <span data-ttu-id="c44df-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c44df-121">Name</span></span>      |<span data-ttu-id="c44df-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c44df-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c44df-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c44df-123">Authorization</span></span>  | <span data-ttu-id="c44df-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c44df-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="c44df-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c44df-126">Content-Type</span></span>   | <span data-ttu-id="c44df-127">Application/Json</span><span class="sxs-lookup"><span data-stu-id="c44df-127">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c44df-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c44df-128">Request body</span></span>
<span data-ttu-id="c44df-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c44df-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c44df-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c44df-130">Response</span></span>

<span data-ttu-id="c44df-131">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [endpoint](../resources/endpoint.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c44df-131">If successful, this method returns a `200 OK` response code and a collection of [Endpoint](../resources/endpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c44df-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c44df-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="c44df-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c44df-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c44df-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c44df-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints
```
# <a name="c"></a>[<span data-ttu-id="c44df-135">C#</span><span class="sxs-lookup"><span data-stu-id="c44df-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c44df-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c44df-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c44df-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c44df-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c44df-138">Java</span><span class="sxs-lookup"><span data-stu-id="c44df-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-endpoints-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c44df-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c44df-139">Response</span></span>
<span data-ttu-id="c44df-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c44df-140">Here is an example of the response.</span></span>
><span data-ttu-id="c44df-141">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c44df-141">Note: The response object shown here might be shortened for readability.</span></span>
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
