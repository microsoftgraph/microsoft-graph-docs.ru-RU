---
title: Get chatMessageHostedContent
description: Извлечение свойств и связей объекта chatMessageHostedContent.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 56c96c812c1c5f8e8a6d471224bf8faef2733045
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947783"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="63225-103">Get chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="63225-103">Get chatMessageHostedContent</span></span>

<span data-ttu-id="63225-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63225-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63225-105">Извлечение свойств и связей [объекта chatMessageHostedContent.](../resources/chatmessagehostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="63225-105">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="63225-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63225-106">Permissions</span></span>

<span data-ttu-id="63225-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63225-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="63225-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63225-109">Permission type</span></span>                        | <span data-ttu-id="63225-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63225-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="63225-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63225-111">Delegated (work or school account)</span></span>| <span data-ttu-id="63225-112">Для **пользователя или** ресурса **чата:** Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63225-112">For **user** or **chat** resource: Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="63225-113">Для **ресурса** канала: ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span><span class="sxs-lookup"><span data-stu-id="63225-113">For **channel** resource: ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="63225-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63225-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63225-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63225-115">Not supported.</span></span>|
|<span data-ttu-id="63225-116">Application</span><span class="sxs-lookup"><span data-stu-id="63225-116">Application</span></span>| <span data-ttu-id="63225-117">Для **пользователя** или **ресурса чата:** Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63225-117">For **user** or **chat** resource: Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="63225-118">Для **ресурса** канала: ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63225-118">For **channel** resource: ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="63225-119">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="63225-119">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="63225-120">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="63225-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="63225-121">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="63225-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="63225-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63225-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="63225-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="63225-123">Optional query parameters</span></span>

<span data-ttu-id="63225-124">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="63225-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63225-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63225-125">Request headers</span></span>

| <span data-ttu-id="63225-126">Имя</span><span class="sxs-lookup"><span data-stu-id="63225-126">Name</span></span>      |<span data-ttu-id="63225-127">Описание</span><span class="sxs-lookup"><span data-stu-id="63225-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="63225-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63225-128">Authorization</span></span> | <span data-ttu-id="63225-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="63225-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="63225-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63225-130">Request body</span></span>

<span data-ttu-id="63225-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="63225-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63225-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="63225-132">Response</span></span>

<span data-ttu-id="63225-133">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="63225-133">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63225-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="63225-134">Examples</span></span>

### <a name="example-1-get-hosted-content"></a><span data-ttu-id="63225-135">Пример 1. Получить хостинг контента</span><span class="sxs-lookup"><span data-stu-id="63225-135">Example 1: Get hosted content</span></span>

#### <a name="request"></a><span data-ttu-id="63225-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="63225-136">Request</span></span>

<span data-ttu-id="63225-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63225-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="63225-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="63225-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="c"></a>[<span data-ttu-id="63225-139">C#</span><span class="sxs-lookup"><span data-stu-id="63225-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63225-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63225-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63225-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63225-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63225-142">Java</span><span class="sxs-lookup"><span data-stu-id="63225-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chatmessagehostedcontent-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="63225-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="63225-143">Response</span></span>

<span data-ttu-id="63225-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="63225-144">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="63225-145">Объект отклика, показанный здесь, может быть сокращен для чтения.</span><span class="sxs-lookup"><span data-stu-id="63225-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="63225-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="63225-146">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="63225-147">Пример 2. Получить у себя bytes контента для изображения</span><span class="sxs-lookup"><span data-stu-id="63225-147">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="63225-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="63225-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="63225-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="63225-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}/$value
```
# <a name="c"></a>[<span data-ttu-id="63225-150">C#</span><span class="sxs-lookup"><span data-stu-id="63225-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63225-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63225-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63225-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63225-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63225-153">Java</span><span class="sxs-lookup"><span data-stu-id="63225-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chatmessagehostedcontent-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="63225-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="63225-154">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->

```http
HTTP/1.1 200 OK
Content-type: image/jpeg
Content-length: 201
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get chatMessageHostedContent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


