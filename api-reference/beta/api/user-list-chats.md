---
title: Список чатов
description: Получение списка объектов Chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3e8ea297fe707c1076543f925610e30686627a7f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270170"
---
# <a name="list-chats"></a><span data-ttu-id="170b0-103">Список чатов</span><span class="sxs-lookup"><span data-stu-id="170b0-103">List chats</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="170b0-104">Получение списка объектов Chat.</span><span class="sxs-lookup"><span data-stu-id="170b0-104">Retrieve a list of chat objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="170b0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="170b0-105">Permissions</span></span>

<span data-ttu-id="170b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="170b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="170b0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="170b0-108">Permission type</span></span>                        | <span data-ttu-id="170b0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="170b0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="170b0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="170b0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="170b0-111">Чат. Read, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="170b0-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="170b0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="170b0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="170b0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="170b0-113">Not supported.</span></span> |
| <span data-ttu-id="170b0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="170b0-114">Application</span></span>                            | <span data-ttu-id="170b0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="170b0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="170b0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="170b0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="170b0-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="170b0-117">Optional query parameters</span></span>

<span data-ttu-id="170b0-118">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="170b0-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="170b0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="170b0-119">Request headers</span></span>

| <span data-ttu-id="170b0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="170b0-120">Name</span></span>      |<span data-ttu-id="170b0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="170b0-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="170b0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="170b0-122">Authorization</span></span> | <span data-ttu-id="170b0-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="170b0-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="170b0-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="170b0-124">Request body</span></span>

<span data-ttu-id="170b0-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="170b0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="170b0-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="170b0-126">Response</span></span>

<span data-ttu-id="170b0-127">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [chat](../resources/chat.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="170b0-127">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="170b0-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="170b0-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="170b0-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="170b0-129">Request</span></span>

<span data-ttu-id="170b0-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="170b0-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->

```http
GET https://graph.microsoft.com/beta/users/{id}/chats
```

### <a name="response"></a><span data-ttu-id="170b0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="170b0-131">Response</span></span>

<span data-ttu-id="170b0-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="170b0-132">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="170b0-133">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="170b0-133">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="170b0-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="170b0-134">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "topic": "topic-value",
      "createdDateTime": "datetime-value",
      "lastUpdatedDateTime": "datetime-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="170b0-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="170b0-135">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="170b0-136">C#</span><span class="sxs-lookup"><span data-stu-id="170b0-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_chats-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="170b0-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="170b0-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_chats-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="170b0-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="170b0-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_chats-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List chats",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-chats.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-list-chats.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-list-chats.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
}-->
