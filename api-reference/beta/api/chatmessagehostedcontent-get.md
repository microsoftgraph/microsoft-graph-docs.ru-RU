---
title: Получение Чатмессажехостедконтент
description: Получение свойств и связей объекта Чатмессажехостедконтент.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1cf0aa6bcca49921d90117be71f4cdc5af28372a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261364"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="98eda-103">Получение Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="98eda-103">Get chatMessageHostedContent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98eda-104">Получение свойств и связей объекта [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) .</span><span class="sxs-lookup"><span data-stu-id="98eda-104">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="98eda-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98eda-105">Permissions</span></span>

<span data-ttu-id="98eda-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98eda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="98eda-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98eda-108">Permission type</span></span>                        | <span data-ttu-id="98eda-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98eda-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="98eda-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98eda-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="98eda-111">Чат. Read, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98eda-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="98eda-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98eda-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98eda-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98eda-113">Not supported.</span></span> |
| <span data-ttu-id="98eda-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98eda-114">Application</span></span>                            | <span data-ttu-id="98eda-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98eda-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="98eda-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98eda-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="98eda-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="98eda-117">Optional query parameters</span></span>

<span data-ttu-id="98eda-118">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="98eda-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="98eda-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98eda-119">Request headers</span></span>

| <span data-ttu-id="98eda-120">Имя</span><span class="sxs-lookup"><span data-stu-id="98eda-120">Name</span></span>      |<span data-ttu-id="98eda-121">Описание</span><span class="sxs-lookup"><span data-stu-id="98eda-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="98eda-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="98eda-122">Authorization</span></span> | <span data-ttu-id="98eda-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="98eda-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="98eda-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98eda-124">Request body</span></span>

<span data-ttu-id="98eda-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98eda-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98eda-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="98eda-126">Response</span></span>

<span data-ttu-id="98eda-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="98eda-127">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="98eda-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="98eda-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="98eda-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="98eda-129">Request</span></span>

<span data-ttu-id="98eda-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98eda-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```

### <a name="response"></a><span data-ttu-id="98eda-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="98eda-131">Response</span></span>

<span data-ttu-id="98eda-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="98eda-132">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="98eda-133">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="98eda-133">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="98eda-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98eda-134">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="98eda-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="98eda-135">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="98eda-136">C#</span><span class="sxs-lookup"><span data-stu-id="98eda-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_chatmessagehostedcontent-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="98eda-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="98eda-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_chatmessagehostedcontent-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="98eda-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="98eda-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_chatmessagehostedcontent-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get chatMessageHostedContent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chatmessagehostedcontent-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chatmessagehostedcontent-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/chatmessagehostedcontent-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
}-->
