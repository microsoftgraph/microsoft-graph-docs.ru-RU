---
title: Список ответов
description: Получение списка объектов chatmessage.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fea842912644c30c7d6b401a4d609d8396f29a94
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863531"
---
# <a name="list-replies"></a><span data-ttu-id="6dc4d-103">Список ответов</span><span class="sxs-lookup"><span data-stu-id="6dc4d-103">List replies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dc4d-104">Получение списка объектов chatmessage.</span><span class="sxs-lookup"><span data-stu-id="6dc4d-104">Retrieve a list of chatmessage objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6dc4d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6dc4d-105">Permissions</span></span>

<span data-ttu-id="6dc4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dc4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6dc4d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6dc4d-108">Permission type</span></span>                        | <span data-ttu-id="6dc4d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6dc4d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6dc4d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6dc4d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6dc4d-111">Чат. Read, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6dc4d-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="6dc4d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6dc4d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dc4d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dc4d-113">Not supported.</span></span> |
| <span data-ttu-id="6dc4d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6dc4d-114">Application</span></span>                            | <span data-ttu-id="6dc4d-115">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6dc4d-115">Chat.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="6dc4d-116">Перед вызовом этого API с разрешениями для приложений необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="6dc4d-116">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="6dc4d-117">Дополнительные сведения см [в разделе protected API в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="6dc4d-117">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="6dc4d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6dc4d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/replies
GET /users/{id}/chats/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6dc4d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6dc4d-119">Optional query parameters</span></span>

<span data-ttu-id="6dc4d-120">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6dc4d-120">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6dc4d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6dc4d-121">Request headers</span></span>

| <span data-ttu-id="6dc4d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6dc4d-122">Name</span></span>      |<span data-ttu-id="6dc4d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6dc4d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6dc4d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6dc4d-124">Authorization</span></span> | <span data-ttu-id="6dc4d-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6dc4d-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6dc4d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6dc4d-126">Request body</span></span>

<span data-ttu-id="6dc4d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6dc4d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dc4d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dc4d-128">Response</span></span>

<span data-ttu-id="6dc4d-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6dc4d-129">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6dc4d-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="6dc4d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6dc4d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6dc4d-131">Request</span></span>

<span data-ttu-id="6dc4d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6dc4d-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6dc4d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6dc4d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_replies"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/replies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6dc4d-134">C#</span><span class="sxs-lookup"><span data-stu-id="6dc4d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-replies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6dc4d-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="6dc4d-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-replies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6dc4d-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6dc4d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-replies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6dc4d-137">Java</span><span class="sxs-lookup"><span data-stu-id="6dc4d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-replies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6dc4d-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="6dc4d-138">Response</span></span>

<span data-ttu-id="6dc4d-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6dc4d-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="6dc4d-140">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6dc4d-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6dc4d-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6dc4d-141">All the properties will be returned from an actual call.</span></span>

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
