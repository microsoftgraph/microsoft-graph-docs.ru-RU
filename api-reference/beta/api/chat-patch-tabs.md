---
title: Вкладка "обновление" в чате
description: Обновление свойств указанной вкладки в чате.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e7b8a1bb20b9e80dc8e86768ae5edf3216090287
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607583"
---
# <a name="update-tab-in-chat"></a><span data-ttu-id="9e9e9-103">Вкладка "обновление" в чате</span><span class="sxs-lookup"><span data-stu-id="9e9e9-103">Update tab in chat</span></span>

<span data-ttu-id="9e9e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e9e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e9e9-105">Обновление свойств указанной [вкладки](../resources/teamstab.md) в [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="9e9e9-105">Update the properties of the specified [tab](../resources/teamstab.md) in a [chat](../resources/chat.md).</span></span> <span data-ttu-id="9e9e9-106">Это можно использовать для настройки контента вкладки.</span><span class="sxs-lookup"><span data-stu-id="9e9e9-106">This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e9e9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e9e9-107">Permissions</span></span>
<span data-ttu-id="9e9e9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e9e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9e9e9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e9e9-110">Permission type</span></span>      | <span data-ttu-id="9e9e9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e9e9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e9e9-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e9e9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9e9e9-113">TeamsTab. Реадвритефорчат, TeamsTab. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9e9e9-113">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="9e9e9-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e9e9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e9e9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e9e9-115">Not supported.</span></span>    |
|<span data-ttu-id="9e9e9-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9e9e9-116">Application</span></span> | <span data-ttu-id="9e9e9-117">TeamsTab. Реадвритефорчат, TeamsTab. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9e9e9-117">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="9e9e9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e9e9-118">HTTP request</span></span>
```http
PATCH /chats/{chat-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="9e9e9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e9e9-119">Request headers</span></span>
| <span data-ttu-id="9e9e9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9e9e9-120">Header</span></span>       | <span data-ttu-id="9e9e9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9e9e9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9e9e9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e9e9-122">Authorization</span></span>  | <span data-ttu-id="9e9e9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e9e9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9e9e9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9e9e9-125">Content-Type</span></span>  | <span data-ttu-id="9e9e9-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e9e9-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9e9e9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e9e9-128">Request body</span></span>
<span data-ttu-id="9e9e9-129">В тексте запроса добавьте представление объекта [Tab](../resources/teamstab.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e9e9-129">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9e9e9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e9e9-130">Response</span></span>

<span data-ttu-id="9e9e9-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный ресурс **teamsTab** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9e9e9-131">If successful, this method returns a `200 OK` response code and the updated **teamsTab** resource in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9e9e9-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="9e9e9-132">Examples</span></span>
### <a name="example-1-update-the-name-of-a-tab-in-a-chat"></a><span data-ttu-id="9e9e9-133">Пример 1: обновление имени вкладки в чате</span><span class="sxs-lookup"><span data-stu-id="9e9e9-133">Example 1: Update the name of a tab in a chat</span></span>

#### <a name="request"></a><span data-ttu-id="9e9e9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e9e9-134">Request</span></span>
<span data-ttu-id="9e9e9-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e9e9-135">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="9e9e9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e9e9-136">Response</span></span>

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

## <a name="see-also"></a><span data-ttu-id="9e9e9-137">См. также</span><span class="sxs-lookup"><span data-stu-id="9e9e9-137">See also</span></span>

- [<span data-ttu-id="9e9e9-138">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="9e9e9-138">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
- [<span data-ttu-id="9e9e9-139">Вкладка "обновление" в канале</span><span class="sxs-lookup"><span data-stu-id="9e9e9-139">Update tab in channel</span></span>](channel-patch-tabs.md)

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


