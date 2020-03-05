---
title: Получение Чатмессажехостедконтент
description: Получение свойств и связей объекта Чатмессажехостедконтент.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d62ffb6fdf88649971992fc42e25ce16be6ae7ab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438297"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="37c3f-103">Получение Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="37c3f-103">Get chatMessageHostedContent</span></span>

<span data-ttu-id="37c3f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="37c3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37c3f-105">Получение свойств и связей объекта [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) .</span><span class="sxs-lookup"><span data-stu-id="37c3f-105">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="37c3f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37c3f-106">Permissions</span></span>

<span data-ttu-id="37c3f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37c3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37c3f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37c3f-109">Permission type</span></span>                        | <span data-ttu-id="37c3f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37c3f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="37c3f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37c3f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="37c3f-112">Для ресурса **user** или **chat**:</span><span class="sxs-lookup"><span data-stu-id="37c3f-112">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="37c3f-113">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37c3f-113">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="37c3f-114">Для ресурса **channel**:</span><span class="sxs-lookup"><span data-stu-id="37c3f-114">For **channel** resource:</span></span><br/><span data-ttu-id="37c3f-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37c3f-115">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="37c3f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37c3f-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37c3f-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="37c3f-117">Not supported</span></span>|
|<span data-ttu-id="37c3f-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="37c3f-118">Application</span></span>| <span data-ttu-id="37c3f-119">Для ресурса **user** или **chat**:</span><span class="sxs-lookup"><span data-stu-id="37c3f-119">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="37c3f-120">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37c3f-120">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="37c3f-121">Для ресурса **channel**:</span><span class="sxs-lookup"><span data-stu-id="37c3f-121">For **channel** resource:</span></span><br/><span data-ttu-id="37c3f-122">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37c3f-122">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="37c3f-123">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="37c3f-123">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="37c3f-124">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="37c3f-124">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="37c3f-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37c3f-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37c3f-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="37c3f-126">Optional query parameters</span></span>

<span data-ttu-id="37c3f-127">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="37c3f-127">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37c3f-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37c3f-128">Request headers</span></span>

| <span data-ttu-id="37c3f-129">Имя</span><span class="sxs-lookup"><span data-stu-id="37c3f-129">Name</span></span>      |<span data-ttu-id="37c3f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="37c3f-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="37c3f-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37c3f-131">Authorization</span></span> | <span data-ttu-id="37c3f-132">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="37c3f-132">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="37c3f-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37c3f-133">Request body</span></span>

<span data-ttu-id="37c3f-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="37c3f-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37c3f-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="37c3f-135">Response</span></span>

<span data-ttu-id="37c3f-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="37c3f-136">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37c3f-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="37c3f-137">Examples</span></span>

### <a name="example-1-get-hosted-content"></a><span data-ttu-id="37c3f-138">Пример 1: получение размещенного контента</span><span class="sxs-lookup"><span data-stu-id="37c3f-138">Example 1: Get hosted content</span></span>

#### <a name="request"></a><span data-ttu-id="37c3f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="37c3f-139">Request</span></span>

<span data-ttu-id="37c3f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37c3f-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37c3f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="37c3f-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="c"></a>[<span data-ttu-id="37c3f-142">C#</span><span class="sxs-lookup"><span data-stu-id="37c3f-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37c3f-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37c3f-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37c3f-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37c3f-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="37c3f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="37c3f-145">Response</span></span>

<span data-ttu-id="37c3f-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="37c3f-146">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="37c3f-147">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="37c3f-147">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="37c3f-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37c3f-148">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="37c3f-149">Пример 2: получение байтов размещенного содержимого для изображения</span><span class="sxs-lookup"><span data-stu-id="37c3f-149">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="37c3f-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="37c3f-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="37c3f-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="37c3f-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}/$value
```
# <a name="c"></a>[<span data-ttu-id="37c3f-152">C#</span><span class="sxs-lookup"><span data-stu-id="37c3f-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37c3f-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37c3f-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37c3f-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37c3f-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="37c3f-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="37c3f-155">Response</span></span>

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
