---
title: Список Чатмессажехостедконтентс
description: Получение списка объектов Чатмессажехостедконтент из сообщения.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 077b3305ce2b342a32f52371d8382b49bd25a55d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958191"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="d4315-103">Список Хостедконтентс</span><span class="sxs-lookup"><span data-stu-id="d4315-103">List hostedContents</span></span>

<span data-ttu-id="d4315-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4315-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4315-105">Получение списка объектов [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) из сообщения.</span><span class="sxs-lookup"><span data-stu-id="d4315-105">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4315-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4315-106">Permissions</span></span>

<span data-ttu-id="d4315-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4315-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4315-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4315-109">Permission type</span></span>                        | <span data-ttu-id="d4315-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4315-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="d4315-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4315-111">Delegated (work or school account)</span></span>| <span data-ttu-id="d4315-112">Для ресурсов " **пользователь** " или " **чат** ": Chat. Read, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4315-112">For **user** or **chat** resource: Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="d4315-113">Для ресурса **Channel** : Чаннелмессаже. Read. ALL, Group. Read. ALL, Group. Read. вритеалл</span><span class="sxs-lookup"><span data-stu-id="d4315-113">For **channel** resource: ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="d4315-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4315-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4315-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4315-115">Not supported.</span></span>|
|<span data-ttu-id="d4315-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4315-116">Application</span></span>| <span data-ttu-id="d4315-117">Для ресурсов " **пользователь** " или " **чат** ": Chat. Read. ALL, Chat. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d4315-117">For **user** or **chat** resource: Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="d4315-118">Для ресурса **Channel** : Чаннелмессаже. Read. Group \*, Чаннелмессаже. Read. ALL, Group. Read. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d4315-118">For **channel** resource: ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="d4315-119">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="d4315-119">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="d4315-120">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="d4315-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="d4315-121">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="d4315-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="d4315-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4315-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents
GET /users/{id}/chats/{id}/messages/{id}/hostedContents
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4315-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d4315-123">Optional query parameters</span></span>

<span data-ttu-id="d4315-124">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d4315-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4315-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4315-125">Request headers</span></span>

| <span data-ttu-id="d4315-126">Имя</span><span class="sxs-lookup"><span data-stu-id="d4315-126">Name</span></span>      |<span data-ttu-id="d4315-127">Описание</span><span class="sxs-lookup"><span data-stu-id="d4315-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d4315-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4315-128">Authorization</span></span> | <span data-ttu-id="d4315-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d4315-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4315-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4315-130">Request body</span></span>

<span data-ttu-id="d4315-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d4315-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4315-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4315-132">Response</span></span>

<span data-ttu-id="d4315-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4315-133">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4315-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="d4315-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4315-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4315-135">Request</span></span>

<span data-ttu-id="d4315-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4315-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d4315-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4315-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontents"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents
```
# <a name="c"></a>[<span data-ttu-id="d4315-138">C#</span><span class="sxs-lookup"><span data-stu-id="d4315-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4315-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4315-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4315-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4315-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4315-141">Java</span><span class="sxs-lookup"><span data-stu-id="d4315-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hostedcontents-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d4315-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4315-142">Response</span></span>

<span data-ttu-id="d4315-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d4315-143">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="d4315-144">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d4315-144">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d4315-145">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4315-145">All the properties will be returned from an actual call.</span></span>

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


