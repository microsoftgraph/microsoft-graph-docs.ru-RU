---
title: Получение Чатмессажехостедконтент
description: Получение свойств и связей объекта Чатмессажехостедконтент.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 81017fbf7dcf3aa2191131e8547cadc0175e60b5
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44287029"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="fc8d1-103">Получение Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="fc8d1-103">Get chatMessageHostedContent</span></span>

<span data-ttu-id="fc8d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc8d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc8d1-105">Получение свойств и связей объекта [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) .</span><span class="sxs-lookup"><span data-stu-id="fc8d1-105">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc8d1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc8d1-106">Permissions</span></span>

<span data-ttu-id="fc8d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc8d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fc8d1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc8d1-109">Permission type</span></span>                        | <span data-ttu-id="fc8d1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc8d1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="fc8d1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc8d1-111">Delegated (work or school account)</span></span>| <span data-ttu-id="fc8d1-112">Для ресурсов " **пользователь** " или " **чат** ": Chat. Read, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc8d1-112">For **user** or **chat** resource: Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="fc8d1-113">Для ресурса **Channel** : Чаннелмессаже. Read. ALL, Group. Read. ALL, Group. Read. вритеалл</span><span class="sxs-lookup"><span data-stu-id="fc8d1-113">For **channel** resource: ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="fc8d1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc8d1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc8d1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc8d1-115">Not supported.</span></span>|
|<span data-ttu-id="fc8d1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc8d1-116">Application</span></span>| <span data-ttu-id="fc8d1-117">Для ресурсов " **пользователь** " или " **чат** ": Chat. Read. ALL, Chat. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fc8d1-117">For **user** or **chat** resource: Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="fc8d1-118">Для ресурса **Channel** : Чаннелмессаже. Read. Group ([RSC](https://aka.ms/teams-rsc)), Чаннелмессаже. Read. ALL, Group. Read. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fc8d1-118">For **channel** resource: ChannelMessage.Read.Group  ([RSC](https://aka.ms/teams-rsc)), ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="fc8d1-119">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="fc8d1-119">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="fc8d1-120">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="fc8d1-120">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="fc8d1-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc8d1-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fc8d1-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fc8d1-122">Optional query parameters</span></span>

<span data-ttu-id="fc8d1-123">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="fc8d1-123">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc8d1-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc8d1-124">Request headers</span></span>

| <span data-ttu-id="fc8d1-125">Имя</span><span class="sxs-lookup"><span data-stu-id="fc8d1-125">Name</span></span>      |<span data-ttu-id="fc8d1-126">Описание</span><span class="sxs-lookup"><span data-stu-id="fc8d1-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fc8d1-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc8d1-127">Authorization</span></span> | <span data-ttu-id="fc8d1-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="fc8d1-128">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc8d1-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc8d1-129">Request body</span></span>

<span data-ttu-id="fc8d1-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fc8d1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc8d1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc8d1-131">Response</span></span>

<span data-ttu-id="fc8d1-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fc8d1-132">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fc8d1-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="fc8d1-133">Examples</span></span>

### <a name="example-1-get-hosted-content"></a><span data-ttu-id="fc8d1-134">Пример 1: получение размещенного контента</span><span class="sxs-lookup"><span data-stu-id="fc8d1-134">Example 1: Get hosted content</span></span>

#### <a name="request"></a><span data-ttu-id="fc8d1-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc8d1-135">Request</span></span>

<span data-ttu-id="fc8d1-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc8d1-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fc8d1-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc8d1-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="c"></a>[<span data-ttu-id="fc8d1-138">C#</span><span class="sxs-lookup"><span data-stu-id="fc8d1-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc8d1-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc8d1-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc8d1-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc8d1-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="fc8d1-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc8d1-141">Response</span></span>

<span data-ttu-id="fc8d1-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc8d1-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="fc8d1-143">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fc8d1-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fc8d1-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc8d1-144">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="fc8d1-145">Пример 2: получение байтов размещенного содержимого для изображения</span><span class="sxs-lookup"><span data-stu-id="fc8d1-145">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="fc8d1-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc8d1-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fc8d1-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc8d1-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}/$value
```
# <a name="c"></a>[<span data-ttu-id="fc8d1-148">C#</span><span class="sxs-lookup"><span data-stu-id="fc8d1-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc8d1-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc8d1-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc8d1-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc8d1-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fc8d1-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc8d1-151">Response</span></span>

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
