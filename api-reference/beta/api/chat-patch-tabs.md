---
title: Вкладка "Обновление" в чате
description: Обновление свойств указанной вкладки в чате.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0225dd70a952d7d977c77c42595d19f7e671f9ff
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689831"
---
# <a name="update-tab-in-chat"></a><span data-ttu-id="dd109-103">Вкладка "Обновление" в чате</span><span class="sxs-lookup"><span data-stu-id="dd109-103">Update tab in chat</span></span>

<span data-ttu-id="dd109-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd109-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd109-105">Обновление свойств указанной вкладки [в](../resources/teamstab.md) [чате.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="dd109-105">Update the properties of the specified [tab](../resources/teamstab.md) in a [chat](../resources/chat.md).</span></span> <span data-ttu-id="dd109-106">Это можно использовать для настройки содержимого вкладки.</span><span class="sxs-lookup"><span data-stu-id="dd109-106">This can be used to configure the content of the tab.</span></span>

> <span data-ttu-id="dd109-107">**Примечание.** Если чат связан с экземпляром [onlineMeeting,](../resources/onlinemeeting.md) фактически вкладка, закрепленная на собрании, будет обновлена.</span><span class="sxs-lookup"><span data-stu-id="dd109-107">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the tab pinned in the meeting will be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd109-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd109-108">Permissions</span></span>
<span data-ttu-id="dd109-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd109-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dd109-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd109-111">Permission type</span></span>      | <span data-ttu-id="dd109-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd109-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd109-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd109-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dd109-114">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd109-114">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="dd109-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd109-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd109-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd109-116">Not supported.</span></span>    |
|<span data-ttu-id="dd109-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="dd109-117">Application</span></span> | <span data-ttu-id="dd109-118">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd109-118">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="dd109-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd109-119">HTTP request</span></span>
```http
PATCH /chats/{chat-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="dd109-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd109-120">Request headers</span></span>
| <span data-ttu-id="dd109-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd109-121">Header</span></span>       | <span data-ttu-id="dd109-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dd109-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dd109-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd109-123">Authorization</span></span>  | <span data-ttu-id="dd109-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd109-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dd109-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd109-126">Content-Type</span></span>  | <span data-ttu-id="dd109-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd109-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dd109-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd109-129">Request body</span></span>
<span data-ttu-id="dd109-130">В теле запроса укажу представление объекта [tab](../resources/teamstab.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="dd109-130">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dd109-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd109-131">Response</span></span>

<span data-ttu-id="dd109-132">В случае успеха этот метод возвращает код отклика и обновленный ресурс `200 OK` **teamsTab** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd109-132">If successful, this method returns a `200 OK` response code and the updated **teamsTab** resource in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dd109-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="dd109-133">Examples</span></span>
### <a name="example-1-update-the-name-of-a-tab-in-a-chat"></a><span data-ttu-id="dd109-134">Пример 1. Обновление имени вкладки в чате</span><span class="sxs-lookup"><span data-stu-id="dd109-134">Example 1: Update the name of a tab in a chat</span></span>

#### <a name="request"></a><span data-ttu-id="dd109-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd109-135">Request</span></span>
<span data-ttu-id="dd109-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd109-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd109-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd109-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tabs_in_chat"
}-->
```http
PATCH https://graph.microsoft.com/beta/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs/794f0e4e-4d10-4bb5-9079-3a465a629eff
Content-type: application/json
Content-length: 211

{
  "displayName": "My Contoso Tab - updated again"
}
```
# <a name="c"></a>[<span data-ttu-id="dd109-138">C#</span><span class="sxs-lookup"><span data-stu-id="dd109-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tabs-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd109-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd109-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tabs-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd109-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd109-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tabs-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd109-141">Java</span><span class="sxs-lookup"><span data-stu-id="dd109-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tabs-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="dd109-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd109-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsTab"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
  "displayName": "My Contoso Tab - updated again",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": "20",
  "webUrl": "https://teams.microsoft.com/l/entity/com.microsoft.teamspace.tab.web/_djb2_msteams_prefix_193fe248-24e6-478f-a66c-ede9ce6dd547?context=%7b%0d%0a++%22context%22%3a+%22chat%22%2c%0d%0a++%22chatId%22%3a+%2219%3ad65713bc498c4a428c71ef9353e6ce20%40thread.v2%22%2c%0d%0a++%22subEntityId%22%3a+null%0d%0a%7d&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924"
}
```

## <a name="see-also"></a><span data-ttu-id="dd109-143">См. также</span><span class="sxs-lookup"><span data-stu-id="dd109-143">See also</span></span>

- [<span data-ttu-id="dd109-144">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="dd109-144">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
- [<span data-ttu-id="dd109-145">Вкладка "обновление" на канале</span><span class="sxs-lookup"><span data-stu-id="dd109-145">Update tab in channel</span></span>](channel-patch-tabs.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update tab in chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


