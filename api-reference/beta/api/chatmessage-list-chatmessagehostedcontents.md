---
title: Список Чатмессажехостедконтентс
description: Получение списка объектов Чатмессажехостедконтент из сообщения.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7e235a902421e7f969e9d9e63400e08e7ebfb253
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982642"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="7c56e-103">Список Хостедконтентс</span><span class="sxs-lookup"><span data-stu-id="7c56e-103">List hostedContents</span></span>

<span data-ttu-id="7c56e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c56e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c56e-105">Получение списка объектов [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) из сообщения.</span><span class="sxs-lookup"><span data-stu-id="7c56e-105">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c56e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c56e-106">Permissions</span></span>

<span data-ttu-id="7c56e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c56e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7c56e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c56e-109">Permission type</span></span>                        | <span data-ttu-id="7c56e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c56e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="7c56e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c56e-111">Delegated (work or school account)</span></span>| <span data-ttu-id="7c56e-112">Для ресурсов " **пользователь** " или " **чат** ": Chat. Read, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c56e-112">For **user** or **chat** resource: Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="7c56e-113">Для ресурса **Channel** : Чаннелмессаже. Read. ALL, Group. Read. ALL, Group. Read. вритеалл</span><span class="sxs-lookup"><span data-stu-id="7c56e-113">For **channel** resource: ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="7c56e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c56e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c56e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c56e-115">Not supported.</span></span>|
|<span data-ttu-id="7c56e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c56e-116">Application</span></span>| <span data-ttu-id="7c56e-117">Для ресурсов " **пользователь** " или " **чат** ": Chat. Read. ALL, Chat. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7c56e-117">For **user** or **chat** resource: Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="7c56e-118">Для ресурса **Channel** : Чаннелмессаже. Read. Group \*, Чаннелмессаже. Read. ALL, Group. Read. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7c56e-118">For **channel** resource: ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="7c56e-119">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="7c56e-119">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="7c56e-120">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="7c56e-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="7c56e-121">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="7c56e-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="7c56e-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c56e-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents
GET /users/{id}/chats/{id}/messages/{id}/hostedContents
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7c56e-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7c56e-123">Optional query parameters</span></span>

<span data-ttu-id="7c56e-124">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7c56e-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c56e-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c56e-125">Request headers</span></span>

| <span data-ttu-id="7c56e-126">Имя</span><span class="sxs-lookup"><span data-stu-id="7c56e-126">Name</span></span>      |<span data-ttu-id="7c56e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="7c56e-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7c56e-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c56e-128">Authorization</span></span> | <span data-ttu-id="7c56e-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7c56e-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c56e-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c56e-130">Request body</span></span>

<span data-ttu-id="7c56e-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7c56e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c56e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c56e-132">Response</span></span>

<span data-ttu-id="7c56e-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c56e-133">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7c56e-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="7c56e-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7c56e-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c56e-135">Request</span></span>

<span data-ttu-id="7c56e-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c56e-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7c56e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c56e-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontents"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents
```
# <a name="c"></a>[<span data-ttu-id="7c56e-138">C#</span><span class="sxs-lookup"><span data-stu-id="7c56e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c56e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c56e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c56e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c56e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7c56e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c56e-141">Response</span></span>

<span data-ttu-id="7c56e-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7c56e-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="7c56e-143">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7c56e-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7c56e-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c56e-144">All the properties will be returned from an actual call.</span></span>

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


