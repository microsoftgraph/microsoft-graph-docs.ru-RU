---
title: Получение конечной точки
description: Получение свойств и связей определенного объекта конечной точки.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: yyuank
ms.openlocfilehash: 703565dd656b5d4b6c3963da9896ef4d0dac5831
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973257"
---
# <a name="get-endpoint"></a><span data-ttu-id="16403-103">Получение конечной точки</span><span class="sxs-lookup"><span data-stu-id="16403-103">Get endpoint</span></span>

<span data-ttu-id="16403-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16403-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16403-105">Получение свойств и связей определенного объекта [конечной точки](../resources/endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="16403-105">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="16403-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16403-106">Permissions</span></span>
<span data-ttu-id="16403-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16403-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="16403-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16403-109">Permission type</span></span>      | <span data-ttu-id="16403-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16403-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16403-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16403-111">Delegated (work or school account)</span></span> | <span data-ttu-id="16403-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16403-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="16403-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16403-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16403-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16403-114">Not supported.</span></span>    |
|<span data-ttu-id="16403-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16403-115">Application</span></span> | <span data-ttu-id="16403-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16403-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16403-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16403-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="16403-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="16403-118">Optional query parameters</span></span>
<span data-ttu-id="16403-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="16403-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16403-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16403-120">Request headers</span></span>
| <span data-ttu-id="16403-121">Имя</span><span class="sxs-lookup"><span data-stu-id="16403-121">Name</span></span>      |<span data-ttu-id="16403-122">Описание</span><span class="sxs-lookup"><span data-stu-id="16403-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="16403-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16403-123">Authorization</span></span>  | <span data-ttu-id="16403-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16403-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16403-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16403-126">Request body</span></span>
<span data-ttu-id="16403-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16403-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16403-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="16403-128">Response</span></span>

<span data-ttu-id="16403-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [конечной точки](../resources/endpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16403-129">If successful, this method returns a `200 OK` response code and an [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="16403-130">Пример</span><span class="sxs-lookup"><span data-stu-id="16403-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="16403-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="16403-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="16403-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="16403-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
# <a name="c"></a>[<span data-ttu-id="16403-133">C#</span><span class="sxs-lookup"><span data-stu-id="16403-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16403-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16403-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16403-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16403-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16403-136">Java</span><span class="sxs-lookup"><span data-stu-id="16403-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-endpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="16403-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="16403-137">Response</span></span>
<span data-ttu-id="16403-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="16403-138">Here is an example of the response.</span></span>
><span data-ttu-id="16403-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16403-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
