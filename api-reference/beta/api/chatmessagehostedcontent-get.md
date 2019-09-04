---
title: Получение Чатмессажехостедконтент
description: Получение свойств и связей объекта Чатмессажехостедконтент.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 899a2c7e2f829f296cd55f420dddbb9079d53890
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719803"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="082da-103">Получение Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="082da-103">Get chatMessageHostedContent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="082da-104">Получение свойств и связей объекта [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) .</span><span class="sxs-lookup"><span data-stu-id="082da-104">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="082da-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="082da-105">Permissions</span></span>

<span data-ttu-id="082da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="082da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="082da-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="082da-108">Permission type</span></span>                        | <span data-ttu-id="082da-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="082da-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="082da-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="082da-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="082da-111">Чат. Read, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="082da-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="082da-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="082da-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="082da-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="082da-113">Not supported.</span></span> |
| <span data-ttu-id="082da-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="082da-114">Application</span></span>                            | <span data-ttu-id="082da-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="082da-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="082da-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="082da-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="082da-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="082da-117">Optional query parameters</span></span>

<span data-ttu-id="082da-118">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="082da-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="082da-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="082da-119">Request headers</span></span>

| <span data-ttu-id="082da-120">Имя</span><span class="sxs-lookup"><span data-stu-id="082da-120">Name</span></span>      |<span data-ttu-id="082da-121">Описание</span><span class="sxs-lookup"><span data-stu-id="082da-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="082da-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="082da-122">Authorization</span></span> | <span data-ttu-id="082da-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="082da-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="082da-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="082da-124">Request body</span></span>

<span data-ttu-id="082da-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="082da-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="082da-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="082da-126">Response</span></span>

<span data-ttu-id="082da-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="082da-127">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="082da-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="082da-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="082da-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="082da-129">Request</span></span>

<span data-ttu-id="082da-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="082da-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="082da-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="082da-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="082da-132">C#</span><span class="sxs-lookup"><span data-stu-id="082da-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="082da-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="082da-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="082da-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="082da-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="082da-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="082da-135">Response</span></span>

<span data-ttu-id="082da-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="082da-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="082da-137">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="082da-137">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="082da-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="082da-138">All the properties will be returned from an actual call.</span></span>

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
