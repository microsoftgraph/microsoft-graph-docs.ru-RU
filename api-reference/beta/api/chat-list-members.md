---
title: Список участников
description: Получение списка объектов Конверсатионмембер.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bf4d178301be74410a894f05732679e482c64583
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261490"
---
# <a name="list-members"></a><span data-ttu-id="ff9d6-103">Список элементов</span><span class="sxs-lookup"><span data-stu-id="ff9d6-103">List members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff9d6-104">Получение списка объектов [конверсатионмембер](../resources/conversationmember.md) .</span><span class="sxs-lookup"><span data-stu-id="ff9d6-104">Retrieve a list of [conversationMember](../resources/conversationmember.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff9d6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff9d6-105">Permissions</span></span>

<span data-ttu-id="ff9d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff9d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ff9d6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff9d6-108">Permission type</span></span>                        | <span data-ttu-id="ff9d6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff9d6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ff9d6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff9d6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ff9d6-111">Чат. Read, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff9d6-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="ff9d6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff9d6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff9d6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff9d6-113">Not supported.</span></span> |
| <span data-ttu-id="ff9d6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff9d6-114">Application</span></span>                            | <span data-ttu-id="ff9d6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff9d6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff9d6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff9d6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/members
GET /users/{id}/chats/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff9d6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ff9d6-117">Optional query parameters</span></span>

<span data-ttu-id="ff9d6-118">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ff9d6-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff9d6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff9d6-119">Request headers</span></span>

| <span data-ttu-id="ff9d6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ff9d6-120">Name</span></span>      |<span data-ttu-id="ff9d6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ff9d6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ff9d6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff9d6-122">Authorization</span></span> | <span data-ttu-id="ff9d6-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ff9d6-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff9d6-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff9d6-124">Request body</span></span>

<span data-ttu-id="ff9d6-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ff9d6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff9d6-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff9d6-126">Response</span></span>

<span data-ttu-id="ff9d6-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [конверсатионмембер](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ff9d6-127">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff9d6-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="ff9d6-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ff9d6-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff9d6-129">Request</span></span>

<span data-ttu-id="ff9d6-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff9d6-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/members
```

### <a name="response"></a><span data-ttu-id="ff9d6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff9d6-131">Response</span></span>

<span data-ttu-id="ff9d6-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ff9d6-132">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="ff9d6-133">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ff9d6-133">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ff9d6-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff9d6-134">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "roles": [
        "roles-value"
      ],
      "displayName": "displayName-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ff9d6-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="ff9d6-135">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="ff9d6-136">C#</span><span class="sxs-lookup"><span data-stu-id="ff9d6-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_members-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff9d6-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="ff9d6-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_members-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ff9d6-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ff9d6-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_members-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chat-list-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chat-list-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/chat-list-members.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
}-->
