---
title: Добавление вкладки в чат
description: 'Добавляет (пин-коды) вкладку в указанный чат. '
author: subray
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1056a2b04a684102b52f8544724cf0e8c6be1404
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960070"
---
# <a name="add-tab-to-chat"></a><span data-ttu-id="57152-103">Добавление вкладки в чат</span><span class="sxs-lookup"><span data-stu-id="57152-103">Add tab to chat</span></span>

<span data-ttu-id="57152-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57152-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="57152-105">Добавьте (пин-код) [вкладку](../resources/teamstab.md) в указанный [чат.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="57152-105">Add (pin) a [tab](../resources/teamstab.md) to the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="57152-106">Соответствующее приложение уже должно [быть установлено в чате.](../api/chat-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="57152-106">The corresponding app must already be [installed in the chat](../api/chat-list-installedapps.md).</span></span>

> <span data-ttu-id="57152-107">**Примечание.** Если чат связан с экземпляром [onlineMeeting,](../resources/onlinemeeting.md) вкладка будет добавлена к собранию.</span><span class="sxs-lookup"><span data-stu-id="57152-107">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the tab will get added to the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="57152-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57152-108">Permissions</span></span>
<span data-ttu-id="57152-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57152-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57152-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57152-111">Permission type</span></span>      | <span data-ttu-id="57152-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57152-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57152-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57152-113">Delegated (work or school account)</span></span> | <span data-ttu-id="57152-114">TeamsTab.Create, TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57152-114">TeamsTab.Create, TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="57152-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57152-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57152-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57152-116">Not supported.</span></span>    |
| <span data-ttu-id="57152-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57152-117">Application</span></span>                            | <span data-ttu-id="57152-118">TeamsTab.Create, TeamsTab.ReadWriteForChat.All, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57152-118">TeamsTab.Create, TeamsTab.ReadWriteForChat.All, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="57152-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57152-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /chats/{chat-id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="57152-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57152-120">Request headers</span></span>
| <span data-ttu-id="57152-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57152-121">Header</span></span>       | <span data-ttu-id="57152-122">Значение</span><span class="sxs-lookup"><span data-stu-id="57152-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="57152-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57152-123">Authorization</span></span>  | <span data-ttu-id="57152-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57152-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="57152-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57152-126">Request body</span></span>

<span data-ttu-id="57152-127">В орган запроса включаем представление JSON [teamsTab](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="57152-127">In the request body include a JSON representation of a [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="57152-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="57152-128">Response</span></span>

<span data-ttu-id="57152-129">В случае успешного использования этот метод возвращает код ответа и экземпляр ресурса `201 Created` [teamsTab](../resources/teamstab.md) в теле.</span><span class="sxs-lookup"><span data-stu-id="57152-129">If successful, this method returns a `201 Created` response code and an instance of the [teamsTab](../resources/teamstab.md) resource in the body.</span></span>

## <a name="example"></a><span data-ttu-id="57152-130">Пример</span><span class="sxs-lookup"><span data-stu-id="57152-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="57152-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="57152-131">Request</span></span>

<span data-ttu-id="57152-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57152-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="57152-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="57152-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_tab_to_chat"
}
-->

```http
POST https://graph.microsoft.com/v1.0/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs
Content-Type: application/json

{
  "displayName": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="57152-134">C#</span><span class="sxs-lookup"><span data-stu-id="57152-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-tab-to-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57152-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57152-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-tab-to-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57152-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57152-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-tab-to-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57152-137">Java</span><span class="sxs-lookup"><span data-stu-id="57152-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-tab-to-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="57152-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="57152-138">Response</span></span>

<span data-ttu-id="57152-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="57152-139">The following is an example of the response.</span></span> 

><span data-ttu-id="57152-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="57152-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="57152-141">См. также</span><span class="sxs-lookup"><span data-stu-id="57152-141">See also</span></span>

- [<span data-ttu-id="57152-142">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="57152-142">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
- [<span data-ttu-id="57152-143">Добавление вкладки в канал</span><span class="sxs-lookup"><span data-stu-id="57152-143">Add tab to channel</span></span>](channel-post-tabs.md)
- [<span data-ttu-id="57152-144">Добавление приложения в чат</span><span class="sxs-lookup"><span data-stu-id="57152-144">Add app to chat</span></span>](chat-post-installedapps.md)


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


