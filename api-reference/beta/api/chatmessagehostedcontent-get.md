---
title: Получение Чатмессажехостедконтент
description: Получение свойств и связей объекта Чатмессажехостедконтент.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e15f8aa932e2534b80fbee0c7d00d759191bc42d
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333222"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="3c5bb-103">Получение Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="3c5bb-103">Get chatMessageHostedContent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c5bb-104">Получение свойств и связей объекта [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) .</span><span class="sxs-lookup"><span data-stu-id="3c5bb-104">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c5bb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c5bb-105">Permissions</span></span>

<span data-ttu-id="3c5bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c5bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3c5bb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c5bb-108">Permission type</span></span>                        | <span data-ttu-id="3c5bb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c5bb-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="3c5bb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c5bb-110">Delegated (work or school account)</span></span>|<span data-ttu-id="3c5bb-111">Для ресурса **User** или **Chat** :</span><span class="sxs-lookup"><span data-stu-id="3c5bb-111">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="3c5bb-112">Чат. Read, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c5bb-112">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="3c5bb-113">Для ресурса **Channel** :</span><span class="sxs-lookup"><span data-stu-id="3c5bb-113">For **channel** resource:</span></span><br/><span data-ttu-id="3c5bb-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c5bb-114">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="3c5bb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c5bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c5bb-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3c5bb-116">Not supported</span></span>|
|<span data-ttu-id="3c5bb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c5bb-117">Application</span></span>| <span data-ttu-id="3c5bb-118">Для ресурса **User** или **Chat** :</span><span class="sxs-lookup"><span data-stu-id="3c5bb-118">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="3c5bb-119">Чат. Read. ALL, Chat. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3c5bb-119">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="3c5bb-120">Для ресурса **Channel** :</span><span class="sxs-lookup"><span data-stu-id="3c5bb-120">For **channel** resource:</span></span><br/><span data-ttu-id="3c5bb-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c5bb-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c5bb-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c5bb-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c5bb-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3c5bb-123">Optional query parameters</span></span>

<span data-ttu-id="3c5bb-124">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3c5bb-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c5bb-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c5bb-125">Request headers</span></span>

| <span data-ttu-id="3c5bb-126">Имя</span><span class="sxs-lookup"><span data-stu-id="3c5bb-126">Name</span></span>      |<span data-ttu-id="3c5bb-127">Описание</span><span class="sxs-lookup"><span data-stu-id="3c5bb-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3c5bb-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c5bb-128">Authorization</span></span> | <span data-ttu-id="3c5bb-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3c5bb-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c5bb-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c5bb-130">Request body</span></span>

<span data-ttu-id="3c5bb-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c5bb-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c5bb-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c5bb-132">Response</span></span>

<span data-ttu-id="3c5bb-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3c5bb-133">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3c5bb-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="3c5bb-134">Examples</span></span>

### <a name="example-1-get-hosted-content"></a><span data-ttu-id="3c5bb-135">Пример 1: получение размещенного контента</span><span class="sxs-lookup"><span data-stu-id="3c5bb-135">Example 1: Get hosted content</span></span>

#### <a name="request"></a><span data-ttu-id="3c5bb-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c5bb-136">Request</span></span>

<span data-ttu-id="3c5bb-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c5bb-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3c5bb-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c5bb-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3c5bb-139">C#</span><span class="sxs-lookup"><span data-stu-id="3c5bb-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c5bb-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c5bb-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3c5bb-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c5bb-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3c5bb-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c5bb-142">Response</span></span>

<span data-ttu-id="3c5bb-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3c5bb-143">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="3c5bb-144">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3c5bb-144">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3c5bb-145">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c5bb-145">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="3c5bb-146">Пример 2: получение байтов размещенного содержимого для изображения</span><span class="sxs-lookup"><span data-stu-id="3c5bb-146">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="3c5bb-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c5bb-147">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->
```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}/$value
```

#### <a name="response"></a><span data-ttu-id="3c5bb-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c5bb-148">Response</span></span>

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
