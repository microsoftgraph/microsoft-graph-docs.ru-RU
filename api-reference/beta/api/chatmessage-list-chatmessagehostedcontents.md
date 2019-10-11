---
title: Список Чатмессажехостедконтентс
description: Получение списка объектов Чатмессажехостедконтент из сообщения.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cc43513ea215f9e4a0d037c39fb9e9fe560e0bb3
ms.sourcegitcommit: e4b0211db9b20dfea8be964003661cd99fe064d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2019
ms.locfileid: "37439872"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="48d27-103">Список Хостедконтентс</span><span class="sxs-lookup"><span data-stu-id="48d27-103">List hostedContents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48d27-104">Получение списка объектов [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) из сообщения.</span><span class="sxs-lookup"><span data-stu-id="48d27-104">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span>

## <a name="permissions"></a><span data-ttu-id="48d27-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48d27-105">Permissions</span></span>

<span data-ttu-id="48d27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48d27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48d27-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48d27-108">Permission type</span></span>                        | <span data-ttu-id="48d27-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48d27-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="48d27-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48d27-110">Delegated (work or school account)</span></span>|<span data-ttu-id="48d27-111">Для ресурса **User** или **Chat** :</span><span class="sxs-lookup"><span data-stu-id="48d27-111">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="48d27-112">Чат. Read, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48d27-112">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="48d27-113">Для ресурса **Channel** :</span><span class="sxs-lookup"><span data-stu-id="48d27-113">For **channel** resource:</span></span><br/><span data-ttu-id="48d27-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48d27-114">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="48d27-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48d27-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48d27-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="48d27-116">Not supported</span></span>|
|<span data-ttu-id="48d27-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48d27-117">Application</span></span>| <span data-ttu-id="48d27-118">Для ресурса **User** или **Chat** :</span><span class="sxs-lookup"><span data-stu-id="48d27-118">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="48d27-119">Чат. Read. ALL, Chat. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="48d27-119">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="48d27-120">Для ресурса **Channel** :</span><span class="sxs-lookup"><span data-stu-id="48d27-120">For **channel** resource:</span></span><br/><span data-ttu-id="48d27-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48d27-121">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="48d27-122">Перед вызовом этого API с разрешениями для приложений необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="48d27-122">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="48d27-123">Дополнительные сведения см [в разделе protected API в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="48d27-123">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="48d27-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48d27-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents
GET /users/{id}/chats/{id}/messages/{id}/hostedContents
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="48d27-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="48d27-125">Optional query parameters</span></span>

<span data-ttu-id="48d27-126">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="48d27-126">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48d27-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48d27-127">Request headers</span></span>

| <span data-ttu-id="48d27-128">Имя</span><span class="sxs-lookup"><span data-stu-id="48d27-128">Name</span></span>      |<span data-ttu-id="48d27-129">Описание</span><span class="sxs-lookup"><span data-stu-id="48d27-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="48d27-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48d27-130">Authorization</span></span> | <span data-ttu-id="48d27-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="48d27-131">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="48d27-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48d27-132">Request body</span></span>

<span data-ttu-id="48d27-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48d27-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48d27-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="48d27-134">Response</span></span>

<span data-ttu-id="48d27-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48d27-135">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="48d27-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="48d27-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="48d27-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="48d27-137">Request</span></span>

<span data-ttu-id="48d27-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48d27-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="48d27-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="48d27-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontents"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="48d27-140">C#</span><span class="sxs-lookup"><span data-stu-id="48d27-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48d27-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48d27-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="48d27-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48d27-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="48d27-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="48d27-143">Response</span></span>

<span data-ttu-id="48d27-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="48d27-144">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="48d27-145">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="48d27-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="48d27-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48d27-146">All the properties will be returned from an actual call.</span></span>

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
