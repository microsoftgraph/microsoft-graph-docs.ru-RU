---
title: Список ответов
description: Получение списка объектов chatmessage.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 44d90dd085a09639467c054dbc2af516d270eb3b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437749"
---
# <a name="list-replies"></a><span data-ttu-id="5de14-103">Список ответов</span><span class="sxs-lookup"><span data-stu-id="5de14-103">List replies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5de14-104">Получение списка объектов chatmessage.</span><span class="sxs-lookup"><span data-stu-id="5de14-104">Retrieve a list of chatmessage objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="5de14-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5de14-105">Permissions</span></span>

<span data-ttu-id="5de14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5de14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5de14-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5de14-108">Permission type</span></span>                        | <span data-ttu-id="5de14-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5de14-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5de14-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5de14-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5de14-111">Чат. Read, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5de14-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="5de14-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5de14-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5de14-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5de14-113">Not supported.</span></span> |
| <span data-ttu-id="5de14-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5de14-114">Application</span></span>                            | <span data-ttu-id="5de14-115">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="5de14-115">Chat.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5de14-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5de14-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/replies
GET /users/{id}/chats/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5de14-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5de14-117">Optional query parameters</span></span>

<span data-ttu-id="5de14-118">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5de14-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5de14-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5de14-119">Request headers</span></span>

| <span data-ttu-id="5de14-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5de14-120">Name</span></span>      |<span data-ttu-id="5de14-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5de14-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5de14-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5de14-122">Authorization</span></span> | <span data-ttu-id="5de14-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5de14-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5de14-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5de14-124">Request body</span></span>

<span data-ttu-id="5de14-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5de14-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5de14-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="5de14-126">Response</span></span>

<span data-ttu-id="5de14-127">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5de14-127">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5de14-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="5de14-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5de14-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5de14-129">Request</span></span>

<span data-ttu-id="5de14-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5de14-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5de14-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5de14-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_replies"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/replies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5de14-132">C#</span><span class="sxs-lookup"><span data-stu-id="5de14-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-replies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5de14-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="5de14-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-replies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5de14-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5de14-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-replies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5de14-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="5de14-135">Response</span></span>

<span data-ttu-id="5de14-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5de14-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="5de14-137">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5de14-137">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5de14-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5de14-138">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "replyToId": "replyToId-value",
      "from": {
        "application": {
          "id": "id-value",
          "displayName": "displayName-value"
        },
        "device": {
          "id": "id-value",
          "displayName": "displayName-value"
        },
        "user": {
          "id": "id-value",
          "displayName": "displayName-value"
        }
      },
      "etag": "etag-value",
      "messageType": "messageType-value",
      "createdDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
