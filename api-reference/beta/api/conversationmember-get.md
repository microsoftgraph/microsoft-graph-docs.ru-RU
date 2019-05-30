---
title: Получение conversationMember
description: Получение участника чата.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 58087819631a9d86464d17307755d6add0af4d73
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536108"
---
# <a name="get-conversationmember"></a><span data-ttu-id="9bebf-103">Получение conversationMember</span><span class="sxs-lookup"><span data-stu-id="9bebf-103">Get conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bebf-104">Получение объекта [conversationMember](../resources/conversationmember.md) из [чата](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="9bebf-104">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9bebf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9bebf-105">Permissions</span></span>

<span data-ttu-id="9bebf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bebf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bebf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9bebf-108">Permission Type</span></span>|<span data-ttu-id="9bebf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9bebf-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="9bebf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9bebf-110">Delegated (work or school account)</span></span>|<span data-ttu-id="9bebf-111">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9bebf-111">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="9bebf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9bebf-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bebf-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9bebf-113">Not supported</span></span>|
|<span data-ttu-id="9bebf-114">Для приложения</span><span class="sxs-lookup"><span data-stu-id="9bebf-114">Application</span></span> |<span data-ttu-id="9bebf-115">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bebf-115">Chat.Read.All, Chat.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9bebf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9bebf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9bebf-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9bebf-117">Optional query parameters</span></span>

<span data-ttu-id="9bebf-118">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="9bebf-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9bebf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9bebf-119">Request headers</span></span>

| <span data-ttu-id="9bebf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9bebf-120">Header</span></span>       | <span data-ttu-id="9bebf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9bebf-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9bebf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9bebf-122">Authorization</span></span>  | <span data-ttu-id="9bebf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9bebf-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9bebf-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9bebf-125">Request body</span></span>

<span data-ttu-id="9bebf-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9bebf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bebf-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bebf-127">Response</span></span>

<span data-ttu-id="9bebf-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9bebf-128">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bebf-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9bebf-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9bebf-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bebf-130">Request</span></span>

<span data-ttu-id="9bebf-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bebf-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="9bebf-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bebf-132">Response</span></span>

<span data-ttu-id="9bebf-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9bebf-133">Here is an example of the response.</span></span> 

><span data-ttu-id="9bebf-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9bebf-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "display-name-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9bebf-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="9bebf-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9bebf-137">C#</span><span class="sxs-lookup"><span data-stu-id="9bebf-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_conversation_member-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9bebf-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bebf-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_conversation_member-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation: member get",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/conversationmember-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/conversationmember-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->