---
title: Добавление вкладки в чат
description: 'Добавляет (пин-коды) вкладку в указанный чат. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f422823b8646bd695c94640b15f456e3e372e0d5
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971260"
---
# <a name="add-tab-to-chat"></a><span data-ttu-id="f6da3-103">Добавление вкладки в чат</span><span class="sxs-lookup"><span data-stu-id="f6da3-103">Add tab to chat</span></span>

<span data-ttu-id="f6da3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6da3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6da3-105">Добавьте (пин-код) [вкладку](../resources/teamstab.md) в указанный [чат.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="f6da3-105">Add (pin) a [tab](../resources/teamstab.md) to the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="f6da3-106">Соответствующее приложение уже должно [быть установлено в чате.](../api/chat-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="f6da3-106">The corresponding app must already be [installed in the chat](../api/chat-list-installedapps.md).</span></span>

> <span data-ttu-id="f6da3-107">**Примечание.** Если чат связан с экземпляром [onlineMeeting,](../resources/onlinemeeting.md) вкладка будет добавлена к собранию.</span><span class="sxs-lookup"><span data-stu-id="f6da3-107">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the tab will get added to the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6da3-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6da3-108">Permissions</span></span>
<span data-ttu-id="f6da3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6da3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6da3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6da3-111">Permission type</span></span>      | <span data-ttu-id="f6da3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6da3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6da3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6da3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f6da3-114">TeamsTab.Create, TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6da3-114">TeamsTab.Create, TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="f6da3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6da3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6da3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6da3-116">Not supported.</span></span>    |
| <span data-ttu-id="f6da3-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f6da3-117">Application</span></span>                            | <span data-ttu-id="f6da3-118">TeamsTab.Create.Chat,*TeamsTab.ReadWrite.Chat,* TeamsTab.Create, TeamsTab.ReadWriteForChat.All, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6da3-118">TeamsTab.Create.Chat *, TeamsTab.ReadWrite.Chat*, TeamsTab.Create, TeamsTab.ReadWriteForChat.All, TeamsTab.ReadWrite.All</span></span> |

> <span data-ttu-id="f6da3-119">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="f6da3-119">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="f6da3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6da3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /chats/{chat-id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="f6da3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6da3-121">Request headers</span></span>
| <span data-ttu-id="f6da3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6da3-122">Header</span></span>       | <span data-ttu-id="f6da3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f6da3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f6da3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6da3-124">Authorization</span></span>  | <span data-ttu-id="f6da3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6da3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f6da3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6da3-127">Request body</span></span>

<span data-ttu-id="f6da3-128">В орган запроса включаем представление JSON [teamsTab](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="f6da3-128">In the request body include a JSON representation of a [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="f6da3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6da3-129">Response</span></span>

<span data-ttu-id="f6da3-130">В случае успешного использования этот метод возвращает код ответа и экземпляр ресурса `201 Created` [teamsTab](../resources/teamstab.md) в теле.</span><span class="sxs-lookup"><span data-stu-id="f6da3-130">If successful, this method returns a `201 Created` response code and an instance of the [teamsTab](../resources/teamstab.md) resource in the body.</span></span>

## <a name="example"></a><span data-ttu-id="f6da3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f6da3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6da3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6da3-132">Request</span></span>

<span data-ttu-id="f6da3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6da3-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f6da3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6da3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_tab_to_chat"
}
-->

```http
POST https://graph.microsoft.com/beta/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs
Content-Type: application/json

{
  "displayName": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="f6da3-135">C#</span><span class="sxs-lookup"><span data-stu-id="f6da3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-tab-to-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6da3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6da3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-tab-to-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6da3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6da3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-tab-to-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f6da3-138">Java</span><span class="sxs-lookup"><span data-stu-id="f6da3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-tab-to-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f6da3-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6da3-139">Response</span></span>

<span data-ttu-id="f6da3-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f6da3-140">The following is an example of the response.</span></span> 

><span data-ttu-id="f6da3-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f6da3-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsTab"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
  "displayName": "My Contoso Tab",
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

## <a name="see-also"></a><span data-ttu-id="f6da3-142">См. также</span><span class="sxs-lookup"><span data-stu-id="f6da3-142">See also</span></span>

- [<span data-ttu-id="f6da3-143">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="f6da3-143">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
- [<span data-ttu-id="f6da3-144">Добавление вкладки в канал</span><span class="sxs-lookup"><span data-stu-id="f6da3-144">Add tab to channel</span></span>](channel-post-tabs.md)
- [<span data-ttu-id="f6da3-145">Добавление приложения в чат</span><span class="sxs-lookup"><span data-stu-id="f6da3-145">Add app to chat</span></span>](chat-post-installedapps.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add tab to chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


