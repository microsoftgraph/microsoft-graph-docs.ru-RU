---
title: Получение Чатмессажехостедконтент
description: Получение свойств и связей объекта Чатмессажехостедконтент.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bdeeb14eff0adf31fefe757cee646d61727f12dd
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535627"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="00a2b-103">Получение Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="00a2b-103">Get chatMessageHostedContent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00a2b-104">Получение свойств и связей объекта [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) .</span><span class="sxs-lookup"><span data-stu-id="00a2b-104">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="00a2b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00a2b-105">Permissions</span></span>

<span data-ttu-id="00a2b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00a2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="00a2b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00a2b-108">Permission type</span></span>                        | <span data-ttu-id="00a2b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00a2b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="00a2b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00a2b-110">Delegated (work or school account)</span></span>|<span data-ttu-id="00a2b-111">Для ресурса **user** или **chat**:</span><span class="sxs-lookup"><span data-stu-id="00a2b-111">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="00a2b-112">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00a2b-112">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="00a2b-113">Для ресурса **channel**:</span><span class="sxs-lookup"><span data-stu-id="00a2b-113">For **channel** resource:</span></span><br/><span data-ttu-id="00a2b-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a2b-114">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="00a2b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00a2b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00a2b-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="00a2b-116">Not supported</span></span>|
|<span data-ttu-id="00a2b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="00a2b-117">Application</span></span>| <span data-ttu-id="00a2b-118">Для ресурса **user** или **chat**:</span><span class="sxs-lookup"><span data-stu-id="00a2b-118">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="00a2b-119">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a2b-119">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="00a2b-120">Для ресурса **channel**:</span><span class="sxs-lookup"><span data-stu-id="00a2b-120">For **channel** resource:</span></span><br/><span data-ttu-id="00a2b-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a2b-121">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="00a2b-122">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="00a2b-122">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="00a2b-123">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="00a2b-123">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="00a2b-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00a2b-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00a2b-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="00a2b-125">Optional query parameters</span></span>

<span data-ttu-id="00a2b-126">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="00a2b-126">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="00a2b-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00a2b-127">Request headers</span></span>

| <span data-ttu-id="00a2b-128">Имя</span><span class="sxs-lookup"><span data-stu-id="00a2b-128">Name</span></span>      |<span data-ttu-id="00a2b-129">Описание</span><span class="sxs-lookup"><span data-stu-id="00a2b-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="00a2b-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00a2b-130">Authorization</span></span> | <span data-ttu-id="00a2b-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="00a2b-131">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="00a2b-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00a2b-132">Request body</span></span>

<span data-ttu-id="00a2b-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00a2b-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00a2b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="00a2b-134">Response</span></span>

<span data-ttu-id="00a2b-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="00a2b-135">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="00a2b-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="00a2b-136">Examples</span></span>

### <a name="example-1-get-hosted-content"></a><span data-ttu-id="00a2b-137">Пример 1: получение размещенного контента</span><span class="sxs-lookup"><span data-stu-id="00a2b-137">Example 1: Get hosted content</span></span>

#### <a name="request"></a><span data-ttu-id="00a2b-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="00a2b-138">Request</span></span>

<span data-ttu-id="00a2b-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00a2b-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="00a2b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="00a2b-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="00a2b-141">C#</span><span class="sxs-lookup"><span data-stu-id="00a2b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00a2b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00a2b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="00a2b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00a2b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="00a2b-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="00a2b-144">Response</span></span>

<span data-ttu-id="00a2b-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="00a2b-145">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="00a2b-146">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="00a2b-146">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="00a2b-147">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00a2b-147">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="00a2b-148">Пример 2: получение байтов размещенного содержимого для изображения</span><span class="sxs-lookup"><span data-stu-id="00a2b-148">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="00a2b-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="00a2b-149">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="00a2b-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="00a2b-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}/$value
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="00a2b-151">C#</span><span class="sxs-lookup"><span data-stu-id="00a2b-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00a2b-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00a2b-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="00a2b-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00a2b-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="00a2b-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="00a2b-154">Response</span></span>

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
