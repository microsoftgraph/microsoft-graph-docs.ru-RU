---
title: Список Чатмессажехостедконтентс
description: Получение списка объектов Чатмессажехостедконтент из сообщения.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 51311dccc3ba5068d2d6485763c157dbbc8c3a35
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491296"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="5e442-103">Список Хостедконтентс</span><span class="sxs-lookup"><span data-stu-id="5e442-103">List hostedContents</span></span>

<span data-ttu-id="5e442-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e442-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e442-105">Получение списка объектов [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) из сообщения.</span><span class="sxs-lookup"><span data-stu-id="5e442-105">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e442-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5e442-106">Permissions</span></span>

<span data-ttu-id="5e442-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e442-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5e442-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e442-109">Permission type</span></span>                        | <span data-ttu-id="5e442-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e442-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="5e442-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e442-111">Delegated (work or school account)</span></span>| <span data-ttu-id="5e442-112">Для ресурсов " **пользователь** " или " **чат** ": Chat. Read, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e442-112">For **user** or **chat** resource: Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="5e442-113">Для ресурса **Channel** : Чаннелмессаже. Read. ALL, Group. Read. ALL, Group. Read. вритеалл</span><span class="sxs-lookup"><span data-stu-id="5e442-113">For **channel** resource: ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="5e442-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e442-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e442-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e442-115">Not supported.</span></span>|
|<span data-ttu-id="5e442-116">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="5e442-116">Application</span></span>| <span data-ttu-id="5e442-117">Для ресурсов " **пользователь** " или " **чат** ": Chat. Read. ALL, Chat. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5e442-117">For **user** or **chat** resource: Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="5e442-118">Для ресурса **Channel** : Чаннелмессаже. Read. Group \*, Чаннелмессаже. Read. ALL, Group. Read. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5e442-118">For **channel** resource: ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="5e442-119">**Note**: разрешения, помеченные как \* использовать [согласие с определенным ресурсом]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="5e442-119">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="5e442-120">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="5e442-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="5e442-121">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="5e442-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="5e442-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e442-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents
GET /users/{id}/chats/{id}/messages/{id}/hostedContents
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5e442-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5e442-123">Optional query parameters</span></span>

<span data-ttu-id="5e442-124">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5e442-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e442-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e442-125">Request headers</span></span>

| <span data-ttu-id="5e442-126">Имя</span><span class="sxs-lookup"><span data-stu-id="5e442-126">Name</span></span>      |<span data-ttu-id="5e442-127">Описание</span><span class="sxs-lookup"><span data-stu-id="5e442-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5e442-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e442-128">Authorization</span></span> | <span data-ttu-id="5e442-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5e442-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e442-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e442-130">Request body</span></span>

<span data-ttu-id="5e442-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5e442-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e442-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e442-132">Response</span></span>

<span data-ttu-id="5e442-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e442-133">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5e442-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="5e442-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5e442-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e442-135">Request</span></span>

<span data-ttu-id="5e442-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e442-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5e442-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e442-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontents"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents
```
# <a name="c"></a>[<span data-ttu-id="5e442-138">C#</span><span class="sxs-lookup"><span data-stu-id="5e442-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e442-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e442-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e442-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e442-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5e442-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e442-141">Response</span></span>

<span data-ttu-id="5e442-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5e442-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="5e442-143">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5e442-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5e442-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e442-144">All the properties will be returned from an actual call.</span></span>

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
