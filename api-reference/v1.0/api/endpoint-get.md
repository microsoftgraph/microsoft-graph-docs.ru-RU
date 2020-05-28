---
title: Получение конечной точки
description: Получение свойств и связей определенного объекта конечной точки.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: yyuank
ms.openlocfilehash: 6c84649a5607684d1841b9ca57611f717141b930
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383618"
---
# <a name="get-endpoint"></a><span data-ttu-id="d800c-103">Получение конечной точки</span><span class="sxs-lookup"><span data-stu-id="d800c-103">Get endpoint</span></span>

<span data-ttu-id="d800c-104">Получение свойств и связей определенного объекта [конечной точки](../resources/endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="d800c-104">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d800c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d800c-105">Permissions</span></span>
<span data-ttu-id="d800c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d800c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d800c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d800c-108">Permission type</span></span>      | <span data-ttu-id="d800c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d800c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d800c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d800c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d800c-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d800c-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d800c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d800c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d800c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d800c-113">Not supported.</span></span>    |
|<span data-ttu-id="d800c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d800c-114">Application</span></span> | <span data-ttu-id="d800c-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d800c-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d800c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d800c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d800c-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d800c-117">Optional query parameters</span></span>
<span data-ttu-id="d800c-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d800c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d800c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d800c-119">Request headers</span></span>
| <span data-ttu-id="d800c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d800c-120">Name</span></span>      |<span data-ttu-id="d800c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d800c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d800c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d800c-122">Authorization</span></span>  | <span data-ttu-id="d800c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d800c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d800c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d800c-125">Request body</span></span>
<span data-ttu-id="d800c-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d800c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d800c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d800c-127">Response</span></span>

<span data-ttu-id="d800c-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [конечной точки](../resources/endpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d800c-128">If successful, this method returns a `200 OK` response code and an [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d800c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d800c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d800c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d800c-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d800c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="d800c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
# <a name="c"></a>[<span data-ttu-id="d800c-132">C#</span><span class="sxs-lookup"><span data-stu-id="d800c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d800c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d800c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d800c-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d800c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d800c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d800c-135">Response</span></span>
<span data-ttu-id="d800c-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d800c-136">Here is an example of the response.</span></span>
><span data-ttu-id="d800c-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d800c-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
