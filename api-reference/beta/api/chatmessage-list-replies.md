---
title: Ответы списка
description: Извлечение списка объектов chatmessage.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 025607cb1b2b9bb33820b8877cbde1d6a1fac844
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947819"
---
# <a name="list-replies"></a><span data-ttu-id="c8744-103">Ответы списка</span><span class="sxs-lookup"><span data-stu-id="c8744-103">List replies</span></span>

<span data-ttu-id="c8744-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8744-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8744-105">Извлечение списка объектов chatmessage.</span><span class="sxs-lookup"><span data-stu-id="c8744-105">Retrieve a list of chatmessage objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8744-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8744-106">Permissions</span></span>

<span data-ttu-id="c8744-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8744-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8744-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8744-109">Permission type</span></span>                        | <span data-ttu-id="c8744-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8744-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c8744-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8744-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8744-112">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8744-112">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="c8744-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8744-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8744-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8744-114">Not supported.</span></span> |
| <span data-ttu-id="c8744-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="c8744-115">Application</span></span>                            | <span data-ttu-id="c8744-116">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8744-116">Chat.Read.All, Chat.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="c8744-117">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="c8744-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="c8744-118">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="c8744-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="c8744-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8744-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8744-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c8744-120">Optional query parameters</span></span>

<span data-ttu-id="c8744-121">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c8744-121">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8744-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8744-122">Request headers</span></span>

| <span data-ttu-id="c8744-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c8744-123">Name</span></span>      |<span data-ttu-id="c8744-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c8744-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c8744-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8744-125">Authorization</span></span> | <span data-ttu-id="c8744-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c8744-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8744-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8744-127">Request body</span></span>

<span data-ttu-id="c8744-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8744-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8744-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8744-129">Response</span></span>

<span data-ttu-id="c8744-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c8744-130">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c8744-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="c8744-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c8744-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8744-132">Request</span></span>

<span data-ttu-id="c8744-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8744-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c8744-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8744-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_replies_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/replies
```
# <a name="c"></a>[<span data-ttu-id="c8744-135">C#</span><span class="sxs-lookup"><span data-stu-id="c8744-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-replies-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8744-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8744-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-replies-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8744-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8744-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-replies-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c8744-138">Java</span><span class="sxs-lookup"><span data-stu-id="c8744-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-replies-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c8744-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8744-139">Response</span></span>

<span data-ttu-id="c8744-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c8744-140">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="c8744-141">Объект отклика, показанный здесь, может быть сокращен для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8744-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c8744-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8744-142">All the properties will be returned from an actual call.</span></span>

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


