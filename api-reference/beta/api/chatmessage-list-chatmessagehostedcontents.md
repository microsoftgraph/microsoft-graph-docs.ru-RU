---
title: Список Чатмессажехостедконтентс
description: Получение списка объектов Чатмессажехостедконтент из сообщения.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0be0b5668b4e583b855ae4e4e85fdb7bc4169705
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438374"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="bd3c4-103">Список Хостедконтентс</span><span class="sxs-lookup"><span data-stu-id="bd3c4-103">List hostedContents</span></span>

<span data-ttu-id="bd3c4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bd3c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd3c4-105">Получение списка объектов [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) из сообщения.</span><span class="sxs-lookup"><span data-stu-id="bd3c4-105">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd3c4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd3c4-106">Permissions</span></span>

<span data-ttu-id="bd3c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd3c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd3c4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd3c4-109">Permission type</span></span>                        | <span data-ttu-id="bd3c4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd3c4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="bd3c4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd3c4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bd3c4-112">Для ресурса **user** или **chat**:</span><span class="sxs-lookup"><span data-stu-id="bd3c4-112">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="bd3c4-113">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd3c4-113">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="bd3c4-114">Для ресурса **channel**:</span><span class="sxs-lookup"><span data-stu-id="bd3c4-114">For **channel** resource:</span></span><br/><span data-ttu-id="bd3c4-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd3c4-115">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="bd3c4-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd3c4-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd3c4-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="bd3c4-117">Not supported</span></span>|
|<span data-ttu-id="bd3c4-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="bd3c4-118">Application</span></span>| <span data-ttu-id="bd3c4-119">Для ресурса **user** или **chat**:</span><span class="sxs-lookup"><span data-stu-id="bd3c4-119">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="bd3c4-120">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd3c4-120">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="bd3c4-121">Для ресурса **channel**:</span><span class="sxs-lookup"><span data-stu-id="bd3c4-121">For **channel** resource:</span></span><br/><span data-ttu-id="bd3c4-122">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd3c4-122">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="bd3c4-123">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="bd3c4-123">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="bd3c4-124">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="bd3c4-124">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="bd3c4-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd3c4-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents
GET /users/{id}/chats/{id}/messages/{id}/hostedContents
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd3c4-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bd3c4-126">Optional query parameters</span></span>

<span data-ttu-id="bd3c4-127">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="bd3c4-127">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd3c4-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd3c4-128">Request headers</span></span>

| <span data-ttu-id="bd3c4-129">Имя</span><span class="sxs-lookup"><span data-stu-id="bd3c4-129">Name</span></span>      |<span data-ttu-id="bd3c4-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bd3c4-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bd3c4-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd3c4-131">Authorization</span></span> | <span data-ttu-id="bd3c4-132">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bd3c4-132">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd3c4-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd3c4-133">Request body</span></span>

<span data-ttu-id="bd3c4-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bd3c4-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd3c4-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="bd3c4-135">Response</span></span>

<span data-ttu-id="bd3c4-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bd3c4-136">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd3c4-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="bd3c4-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd3c4-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd3c4-138">Request</span></span>

<span data-ttu-id="bd3c4-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd3c4-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bd3c4-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd3c4-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontents"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents
```
# <a name="c"></a>[<span data-ttu-id="bd3c4-141">C#</span><span class="sxs-lookup"><span data-stu-id="bd3c4-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd3c4-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd3c4-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd3c4-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd3c4-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bd3c4-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd3c4-144">Response</span></span>

<span data-ttu-id="bd3c4-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bd3c4-145">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="bd3c4-146">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bd3c4-146">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bd3c4-147">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd3c4-147">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List hostedContents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
