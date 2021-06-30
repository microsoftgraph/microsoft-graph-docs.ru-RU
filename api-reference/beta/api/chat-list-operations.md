---
title: Список операций в чате
description: Извлечение операций в чате.
author: jecha
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0c92bfcc920e1839cf90e09126519b2cd343620e
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207958"
---
# <a name="list-operations-on-a-chat"></a><span data-ttu-id="4cd6b-103">Список операций в чате</span><span class="sxs-lookup"><span data-stu-id="4cd6b-103">List operations on a chat</span></span>
<span data-ttu-id="4cd6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cd6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cd6b-105">Список [всех Teams async,](../resources/teamsasyncoperation.md) которые запускались или запускались в указанном [чате.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="4cd6b-105">List all [Teams async operations](../resources/teamsasyncoperation.md) that ran or are running on the specified [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4cd6b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4cd6b-106">Permissions</span></span>
<span data-ttu-id="4cd6b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cd6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4cd6b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cd6b-109">Permission type</span></span>                        | <span data-ttu-id="4cd6b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cd6b-110">Permissions (from least to most privileged)</span></span>|
| :------------------------------------- | :--------------------------------------------------- |
| <span data-ttu-id="4cd6b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cd6b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4cd6b-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4cd6b-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span>|
| <span data-ttu-id="4cd6b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cd6b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cd6b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cd6b-114">Not supported.</span></span> |
| <span data-ttu-id="4cd6b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="4cd6b-115">Application</span></span>                            | <span data-ttu-id="4cd6b-116">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cd6b-116">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |

> <span data-ttu-id="4cd6b-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="4cd6b-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="4cd6b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cd6b-118">HTTP request</span></span>
<!-- { 
    "blockType": "ignored" 
} 
-->
``` http
GET /chats/{chat-id}/operations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4cd6b-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4cd6b-119">Optional query parameters</span></span>

<span data-ttu-id="4cd6b-120">Этот метод поддерживает `$filter` параметры `$select` запросов , и `$top` `$skip` [OData,](/graph/query-parameters) чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="4cd6b-120">This method supports the `$filter`, `$select`, `$top`, and `$skip` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4cd6b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4cd6b-121">Request headers</span></span>

|<span data-ttu-id="4cd6b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4cd6b-122">Name</span></span>|<span data-ttu-id="4cd6b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4cd6b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4cd6b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4cd6b-124">Authorization</span></span>|<span data-ttu-id="4cd6b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cd6b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cd6b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4cd6b-127">Request body</span></span>

<span data-ttu-id="4cd6b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4cd6b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cd6b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cd6b-129">Response</span></span>

<span data-ttu-id="4cd6b-130">В случае успешной работы возвращается код ответа и коллекция объектов `200 OK` [teamsAsyncOperation](../resources/teamsasyncoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4cd6b-130">If successful, this returns a `200 OK` response code and a collection of [teamsAsyncOperation](../resources/teamsasyncoperation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4cd6b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="4cd6b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4cd6b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cd6b-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4cd6b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4cd6b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_chat_operations"
}
-->
``` http
GET https://graph.microsoft.com/beta/chats/19:c253a29b5f694b55a6baad8e83510af7@thread.v2/operations
```
# <a name="c"></a>[<span data-ttu-id="4cd6b-134">C#</span><span class="sxs-lookup"><span data-stu-id="4cd6b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-chat-operations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4cd6b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4cd6b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-chat-operations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4cd6b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4cd6b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-chat-operations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4cd6b-137">Java</span><span class="sxs-lookup"><span data-stu-id="4cd6b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-chat-operations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="4cd6b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cd6b-138">Response</span></span>
><span data-ttu-id="4cd6b-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4cd6b-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAsyncOperation",
  "isCollection": true
}
-->
``` http
HTTP/1.1 202 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ac253a29b5f694b55a6baad8e83510af7%40thread.v2')/operations",
    "@odata.count": 1,
    "value": [
        {
            "id": "2432b57b-0abd-43db-aa7b-16eadd115d34-e88ae9aa-887e-4972-ac3e-bd578e38232e-cf58835e-43f0-4fc1-825e-5de55630e7e4",
            "operationType": "createChat",
            "createdDateTime": "2021-05-27T21:23:41.9085453Z",
            "status": "succeeded",
            "lastActionDateTime": "2021-05-27T21:23:45.1899277Z",
            "attemptsCount": 1,
            "targetResourceId": "19:c253a29b5f694b55a6baad8e83510af7@thread.v2",
            "targetResourceLocation": "/chats('19:c253a29b5f694b55a6baad8e83510af7@thread.v2')",
            "values": "{\"appIds\":[\"1542629c-01b3-4a6d-8f76-1938b779e48d\"]}",
            "error": null
        }
    ]
}
```
