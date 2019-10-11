---
title: Получение Чатмессажехостедконтент
description: Получение свойств и связей объекта Чатмессажехостедконтент.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e911091bb4e1b5cd3179f781dd0d2f326f121a3d
ms.sourcegitcommit: e4b0211db9b20dfea8be964003661cd99fe064d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2019
ms.locfileid: "37439865"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="68503-103">Получение Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="68503-103">Get chatMessageHostedContent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68503-104">Получение свойств и связей объекта [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) .</span><span class="sxs-lookup"><span data-stu-id="68503-104">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="68503-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68503-105">Permissions</span></span>

<span data-ttu-id="68503-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68503-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="68503-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68503-108">Permission type</span></span>                        | <span data-ttu-id="68503-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68503-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="68503-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68503-110">Delegated (work or school account)</span></span>|<span data-ttu-id="68503-111">Для ресурса **User** или **Chat** :</span><span class="sxs-lookup"><span data-stu-id="68503-111">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="68503-112">Чат. Read, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68503-112">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="68503-113">Для ресурса **Channel** :</span><span class="sxs-lookup"><span data-stu-id="68503-113">For **channel** resource:</span></span><br/><span data-ttu-id="68503-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68503-114">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="68503-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68503-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68503-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="68503-116">Not supported</span></span>|
|<span data-ttu-id="68503-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68503-117">Application</span></span>| <span data-ttu-id="68503-118">Для ресурса **User** или **Chat** :</span><span class="sxs-lookup"><span data-stu-id="68503-118">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="68503-119">Чат. Read. ALL, Chat. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="68503-119">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="68503-120">Для ресурса **Channel** :</span><span class="sxs-lookup"><span data-stu-id="68503-120">For **channel** resource:</span></span><br/><span data-ttu-id="68503-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68503-121">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="68503-122">Перед вызовом этого API с разрешениями для приложений необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="68503-122">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="68503-123">Дополнительные сведения см [в разделе protected API в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="68503-123">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="68503-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68503-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68503-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="68503-125">Optional query parameters</span></span>

<span data-ttu-id="68503-126">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="68503-126">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="68503-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68503-127">Request headers</span></span>

| <span data-ttu-id="68503-128">Имя</span><span class="sxs-lookup"><span data-stu-id="68503-128">Name</span></span>      |<span data-ttu-id="68503-129">Описание</span><span class="sxs-lookup"><span data-stu-id="68503-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="68503-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68503-130">Authorization</span></span> | <span data-ttu-id="68503-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="68503-131">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="68503-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68503-132">Request body</span></span>

<span data-ttu-id="68503-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68503-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68503-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="68503-134">Response</span></span>

<span data-ttu-id="68503-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="68503-135">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="68503-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="68503-136">Examples</span></span>

### <a name="example-1-get-hosted-content"></a><span data-ttu-id="68503-137">Пример 1: получение размещенного контента</span><span class="sxs-lookup"><span data-stu-id="68503-137">Example 1: Get hosted content</span></span>

#### <a name="request"></a><span data-ttu-id="68503-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="68503-138">Request</span></span>

<span data-ttu-id="68503-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68503-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="68503-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="68503-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="68503-141">C#</span><span class="sxs-lookup"><span data-stu-id="68503-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="68503-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68503-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="68503-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68503-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="68503-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="68503-144">Response</span></span>

<span data-ttu-id="68503-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="68503-145">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="68503-146">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="68503-146">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="68503-147">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68503-147">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="68503-148">Пример 2: получение байтов размещенного содержимого для изображения</span><span class="sxs-lookup"><span data-stu-id="68503-148">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="68503-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="68503-149">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="68503-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="68503-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->
```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}/$value
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="68503-151">C#</span><span class="sxs-lookup"><span data-stu-id="68503-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="68503-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68503-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="68503-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68503-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="68503-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="68503-154">Response</span></span>

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
