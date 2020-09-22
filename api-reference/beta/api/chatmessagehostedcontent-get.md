---
title: Получение Чатмессажехостедконтент
description: Получение свойств и связей объекта Чатмессажехостедконтент.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: eb5c56eb1a67e8fac936e9a80600f8291cd595d4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982591"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="49c06-103">Получение Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="49c06-103">Get chatMessageHostedContent</span></span>

<span data-ttu-id="49c06-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49c06-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49c06-105">Получение свойств и связей объекта [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) .</span><span class="sxs-lookup"><span data-stu-id="49c06-105">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="49c06-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49c06-106">Permissions</span></span>

<span data-ttu-id="49c06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49c06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49c06-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49c06-109">Permission type</span></span>                        | <span data-ttu-id="49c06-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49c06-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="49c06-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49c06-111">Delegated (work or school account)</span></span>| <span data-ttu-id="49c06-112">Для ресурсов " **пользователь** " или " **чат** ": Chat. Read, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49c06-112">For **user** or **chat** resource: Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="49c06-113">Для ресурса **Channel** : Чаннелмессаже. Read. ALL, Group. Read. ALL, Group. Read. вритеалл</span><span class="sxs-lookup"><span data-stu-id="49c06-113">For **channel** resource: ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="49c06-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49c06-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49c06-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49c06-115">Not supported.</span></span>|
|<span data-ttu-id="49c06-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49c06-116">Application</span></span>| <span data-ttu-id="49c06-117">Для ресурсов " **пользователь** " или " **чат** ": Chat. Read. ALL, Chat. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="49c06-117">For **user** or **chat** resource: Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="49c06-118">Для ресурса **Channel** : Чаннелмессаже. Read. Group \*, Чаннелмессаже. Read. ALL, Group. Read. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="49c06-118">For **channel** resource: ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="49c06-119">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="49c06-119">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="49c06-120">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="49c06-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="49c06-121">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="49c06-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="49c06-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49c06-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="49c06-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="49c06-123">Optional query parameters</span></span>

<span data-ttu-id="49c06-124">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="49c06-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49c06-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49c06-125">Request headers</span></span>

| <span data-ttu-id="49c06-126">Имя</span><span class="sxs-lookup"><span data-stu-id="49c06-126">Name</span></span>      |<span data-ttu-id="49c06-127">Описание</span><span class="sxs-lookup"><span data-stu-id="49c06-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="49c06-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49c06-128">Authorization</span></span> | <span data-ttu-id="49c06-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="49c06-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="49c06-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49c06-130">Request body</span></span>

<span data-ttu-id="49c06-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49c06-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49c06-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="49c06-132">Response</span></span>

<span data-ttu-id="49c06-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49c06-133">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49c06-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="49c06-134">Examples</span></span>

### <a name="example-1-get-hosted-content"></a><span data-ttu-id="49c06-135">Пример 1: получение размещенного контента</span><span class="sxs-lookup"><span data-stu-id="49c06-135">Example 1: Get hosted content</span></span>

#### <a name="request"></a><span data-ttu-id="49c06-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="49c06-136">Request</span></span>

<span data-ttu-id="49c06-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49c06-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49c06-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="49c06-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="c"></a>[<span data-ttu-id="49c06-139">C#</span><span class="sxs-lookup"><span data-stu-id="49c06-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49c06-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49c06-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49c06-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49c06-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="49c06-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="49c06-142">Response</span></span>

<span data-ttu-id="49c06-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="49c06-143">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="49c06-144">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="49c06-144">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="49c06-145">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49c06-145">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="49c06-146">Пример 2: получение байтов размещенного содержимого для изображения</span><span class="sxs-lookup"><span data-stu-id="49c06-146">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="49c06-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="49c06-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="49c06-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="49c06-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}/$value
```
# <a name="c"></a>[<span data-ttu-id="49c06-149">C#</span><span class="sxs-lookup"><span data-stu-id="49c06-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49c06-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49c06-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49c06-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49c06-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="49c06-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="49c06-152">Response</span></span>

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


