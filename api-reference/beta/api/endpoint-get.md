---
title: Получение конечной точки
description: Получение свойств и связей определенного объекта конечной точки.
localization_priority: Normal
ms.openlocfilehash: 9c43c965fe5210df035f1b7a6bb6b553c4f40540
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587215"
---
# <a name="get-endpoint"></a><span data-ttu-id="0dfa1-103">Получение конечной точки</span><span class="sxs-lookup"><span data-stu-id="0dfa1-103">Get endpoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0dfa1-104">Получение свойств и связей определенного объекта [конечной точки](../resources/endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="0dfa1-104">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0dfa1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0dfa1-105">Permissions</span></span>
<span data-ttu-id="0dfa1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0dfa1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0dfa1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0dfa1-108">Permission type</span></span>      | <span data-ttu-id="0dfa1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0dfa1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0dfa1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0dfa1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0dfa1-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dfa1-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0dfa1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0dfa1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0dfa1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0dfa1-113">Not supported.</span></span>    |
|<span data-ttu-id="0dfa1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0dfa1-114">Application</span></span> | <span data-ttu-id="0dfa1-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dfa1-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0dfa1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0dfa1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0dfa1-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0dfa1-117">Optional query parameters</span></span>
<span data-ttu-id="0dfa1-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0dfa1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0dfa1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0dfa1-119">Request headers</span></span>
| <span data-ttu-id="0dfa1-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0dfa1-120">Name</span></span>      |<span data-ttu-id="0dfa1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0dfa1-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0dfa1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0dfa1-122">Authorization</span></span>  | <span data-ttu-id="0dfa1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0dfa1-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="0dfa1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0dfa1-125">Content-Type</span></span>   | <span data-ttu-id="0dfa1-126">Приложение/JSON</span><span class="sxs-lookup"><span data-stu-id="0dfa1-126">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0dfa1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0dfa1-127">Request body</span></span>
<span data-ttu-id="0dfa1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0dfa1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0dfa1-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="0dfa1-129">Response</span></span>

<span data-ttu-id="0dfa1-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [конечной точки](../resources/endpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0dfa1-130">If successful, this method returns a `200 OK` response code and [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0dfa1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0dfa1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0dfa1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0dfa1-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
##### <a name="response"></a><span data-ttu-id="0dfa1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0dfa1-133">Response</span></span>
<span data-ttu-id="0dfa1-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0dfa1-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0dfa1-136">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="0dfa1-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0dfa1-137">Языках</span><span class="sxs-lookup"><span data-stu-id="0dfa1-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_endpoint-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0dfa1-138">Язык</span><span class="sxs-lookup"><span data-stu-id="0dfa1-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_endpoint-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/endpoint-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/endpoint-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
