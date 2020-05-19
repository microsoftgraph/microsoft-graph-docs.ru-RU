---
title: Список ответов
description: Получение списка объектов chatmessage.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d82d2fe3268cb95af19b39b6be192fe44f747a20
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44287106"
---
# <a name="list-replies"></a><span data-ttu-id="c032a-103">Список ответов</span><span class="sxs-lookup"><span data-stu-id="c032a-103">List replies</span></span>

<span data-ttu-id="c032a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c032a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c032a-105">Получение списка объектов chatmessage.</span><span class="sxs-lookup"><span data-stu-id="c032a-105">Retrieve a list of chatmessage objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c032a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c032a-106">Permissions</span></span>

<span data-ttu-id="c032a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c032a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c032a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c032a-109">Permission type</span></span>                        | <span data-ttu-id="c032a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c032a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c032a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c032a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c032a-112">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c032a-112">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="c032a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c032a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c032a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c032a-114">Not supported.</span></span> |
| <span data-ttu-id="c032a-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="c032a-115">Application</span></span>                            | <span data-ttu-id="c032a-116">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c032a-116">Chat.Read.All, Chat.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="c032a-117">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="c032a-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="c032a-118">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="c032a-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="c032a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c032a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c032a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c032a-120">Optional query parameters</span></span>

<span data-ttu-id="c032a-121">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c032a-121">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c032a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c032a-122">Request headers</span></span>

| <span data-ttu-id="c032a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c032a-123">Name</span></span>      |<span data-ttu-id="c032a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c032a-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c032a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c032a-125">Authorization</span></span> | <span data-ttu-id="c032a-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c032a-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c032a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c032a-127">Request body</span></span>

<span data-ttu-id="c032a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c032a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c032a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c032a-129">Response</span></span>

<span data-ttu-id="c032a-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c032a-130">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c032a-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="c032a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c032a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c032a-132">Request</span></span>

<span data-ttu-id="c032a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c032a-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c032a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c032a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_replies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/replies
```
# <a name="c"></a>[<span data-ttu-id="c032a-135">C#</span><span class="sxs-lookup"><span data-stu-id="c032a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-replies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c032a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c032a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-replies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c032a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c032a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-replies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c032a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c032a-138">Response</span></span>

<span data-ttu-id="c032a-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c032a-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="c032a-140">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c032a-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c032a-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c032a-141">All the properties will be returned from an actual call.</span></span>

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
