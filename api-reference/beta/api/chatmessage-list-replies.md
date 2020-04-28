---
title: Список ответов
description: Получение списка объектов chatmessage.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d8e3332a7ed50dd7c1ba383b247cd5016af5a768
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438360"
---
# <a name="list-replies"></a><span data-ttu-id="970fd-103">Список ответов</span><span class="sxs-lookup"><span data-stu-id="970fd-103">List replies</span></span>

<span data-ttu-id="970fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="970fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="970fd-105">Получение списка объектов chatmessage.</span><span class="sxs-lookup"><span data-stu-id="970fd-105">Retrieve a list of chatmessage objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="970fd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="970fd-106">Permissions</span></span>

<span data-ttu-id="970fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="970fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="970fd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="970fd-109">Permission type</span></span>                        | <span data-ttu-id="970fd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="970fd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="970fd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="970fd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="970fd-112">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="970fd-112">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="970fd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="970fd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="970fd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="970fd-114">Not supported.</span></span> |
| <span data-ttu-id="970fd-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="970fd-115">Application</span></span>                            | <span data-ttu-id="970fd-116">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="970fd-116">Chat.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="970fd-117">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="970fd-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="970fd-118">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="970fd-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="970fd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="970fd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="970fd-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="970fd-120">Optional query parameters</span></span>

<span data-ttu-id="970fd-121">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="970fd-121">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="970fd-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="970fd-122">Request headers</span></span>

| <span data-ttu-id="970fd-123">Имя</span><span class="sxs-lookup"><span data-stu-id="970fd-123">Name</span></span>      |<span data-ttu-id="970fd-124">Описание</span><span class="sxs-lookup"><span data-stu-id="970fd-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="970fd-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="970fd-125">Authorization</span></span> | <span data-ttu-id="970fd-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="970fd-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="970fd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="970fd-127">Request body</span></span>

<span data-ttu-id="970fd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="970fd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="970fd-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="970fd-129">Response</span></span>

<span data-ttu-id="970fd-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="970fd-130">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="970fd-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="970fd-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="970fd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="970fd-132">Request</span></span>

<span data-ttu-id="970fd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="970fd-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="970fd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="970fd-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_replies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/replies
```
# <a name="c"></a>[<span data-ttu-id="970fd-135">C#</span><span class="sxs-lookup"><span data-stu-id="970fd-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-replies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="970fd-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="970fd-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-replies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="970fd-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="970fd-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-replies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="970fd-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="970fd-138">Response</span></span>

<span data-ttu-id="970fd-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="970fd-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="970fd-140">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="970fd-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="970fd-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="970fd-141">All the properties will be returned from an actual call.</span></span>

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
