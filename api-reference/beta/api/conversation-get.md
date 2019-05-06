---
title: Получение беседы
description: Получение свойств и связей объекта беседы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 45e8b4e8a3d4397a62d1161a145608447f38d5cf
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591256"
---
# <a name="get-conversation"></a><span data-ttu-id="38541-103">Получение беседы</span><span class="sxs-lookup"><span data-stu-id="38541-103">Get conversation</span></span>

<span data-ttu-id="38541-104">Получение свойств и связей объекта беседы.</span><span class="sxs-lookup"><span data-stu-id="38541-104">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="38541-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="38541-105">Permissions</span></span>
<span data-ttu-id="38541-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38541-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38541-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38541-108">Permission type</span></span>      | <span data-ttu-id="38541-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="38541-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38541-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38541-110">Delegated (work or school account)</span></span> | <span data-ttu-id="38541-111">Group. ReadWrite. ALL, Group. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="38541-111">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="38541-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38541-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38541-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38541-113">Not supported.</span></span>    |
|<span data-ttu-id="38541-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38541-114">Application</span></span> | <span data-ttu-id="38541-115">Group. ReadWrite. ALL, Group. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="38541-115">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38541-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38541-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="38541-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="38541-117">Optional query parameters</span></span>
<span data-ttu-id="38541-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="38541-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="38541-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38541-119">Request headers</span></span>
| <span data-ttu-id="38541-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38541-120">Header</span></span>       | <span data-ttu-id="38541-121">Значение</span><span class="sxs-lookup"><span data-stu-id="38541-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="38541-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38541-122">Authorization</span></span>  | <span data-ttu-id="38541-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38541-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="38541-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38541-125">Request body</span></span>
<span data-ttu-id="38541-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="38541-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38541-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="38541-127">Response</span></span>

<span data-ttu-id="38541-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversation](../resources/conversation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="38541-128">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="38541-129">Пример</span><span class="sxs-lookup"><span data-stu-id="38541-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38541-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="38541-130">Request</span></span>
<span data-ttu-id="38541-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38541-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="38541-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="38541-132">Response</span></span>
<span data-ttu-id="38541-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38541-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="38541-136">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="38541-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="38541-137">Языках</span><span class="sxs-lookup"><span data-stu-id="38541-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_conversation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38541-138">Язык</span><span class="sxs-lookup"><span data-stu-id="38541-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_conversation-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/conversation-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/conversation-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
