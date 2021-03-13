---
title: Список вкладок в чате
description: 'Извлечение списка вкладок в указанном чате. '
author: subray
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9d90b24e8746d53049a82e2f1858ac62d0497cd7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777344"
---
# <a name="list-tabs-in-chat"></a><span data-ttu-id="a55c3-103">Список вкладок в чате</span><span class="sxs-lookup"><span data-stu-id="a55c3-103">List tabs in chat</span></span>

<span data-ttu-id="a55c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a55c3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a55c3-105">Извлечение списка [вкладок](../resources/teamstab.md) в указанном [чате.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="a55c3-105">Retrieve the list of [tabs](../resources/teamstab.md) in the specified [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="a55c3-106">**Примечание.** Если чат связан с экземпляром [onlineMeeting,](../resources/onlinemeeting.md) то фактически вкладки, закрепленные на собрании, будут перечислены.</span><span class="sxs-lookup"><span data-stu-id="a55c3-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the tabs pinned in the meeting will be listed.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a55c3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a55c3-107">Permissions</span></span>
<span data-ttu-id="a55c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a55c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a55c3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a55c3-110">Permission type</span></span>      | <span data-ttu-id="a55c3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a55c3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a55c3-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a55c3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a55c3-113">TeamsTab.ReadWriteForChat, TeamsTab.Read.All, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a55c3-113">TeamsTab.ReadWriteForChat, TeamsTab.Read.All, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="a55c3-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a55c3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a55c3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a55c3-115">Not supported.</span></span>    |
|<span data-ttu-id="a55c3-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="a55c3-116">Application</span></span> | <span data-ttu-id="a55c3-117">TeamsTab.ReadWriteForChat.All, TeamsTab.Read.All, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a55c3-117">TeamsTab.ReadWriteForChat.All, TeamsTab.Read.All, TeamsTab.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a55c3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a55c3-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
GET /chats/{chat-id}/tabs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a55c3-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a55c3-119">Optional query parameters</span></span>

<span data-ttu-id="a55c3-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a55c3-120">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a55c3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a55c3-121">Request headers</span></span>
| <span data-ttu-id="a55c3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a55c3-122">Header</span></span>       | <span data-ttu-id="a55c3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a55c3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a55c3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a55c3-124">Authorization</span></span>  | <span data-ttu-id="a55c3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a55c3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a55c3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a55c3-127">Request body</span></span>
<span data-ttu-id="a55c3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a55c3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a55c3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a55c3-129">Response</span></span>
<span data-ttu-id="a55c3-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [вкладок](../resources/teamstab.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a55c3-130">If successful, this method returns a `200 OK` response code and collection of [tabs](../resources/teamstab.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a55c3-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="a55c3-131">Examples</span></span>

### <a name="example-1-list-all-the-tabs-in-the-chat-along-with-associated-teams-app"></a><span data-ttu-id="a55c3-132">Пример 1. Список всех вкладок в чате вместе со связанным приложением Teams</span><span class="sxs-lookup"><span data-stu-id="a55c3-132">Example 1: List all the tabs in the chat along with associated Teams app</span></span>
#### <a name="request"></a><span data-ttu-id="a55c3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a55c3-133">Request</span></span>
<span data-ttu-id="a55c3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a55c3-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_tabs_in_chat"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs?$expand=teamsApp
```


#### <a name="response"></a><span data-ttu-id="a55c3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a55c3-135">Response</span></span>
<span data-ttu-id="a55c3-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a55c3-136">The following is an example of the response.</span></span>
><span data-ttu-id="a55c3-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a55c3-137">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamsTab)"
}
-->

```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "value": [
    {
      "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
      "displayName": "My Contoso Tab - updated",
      "sortOrderIndex": "20",
      "webUrl": "https://teams.microsoft.com/l/entity/com.microsoft.teamspace.tab.web/_djb2_msteams_prefix_193fe248-24e6-478f-a66c-ede9ce6dd547?context=%7b%0d%0a++%22context%22%3a+%22chat%22%2c%0d%0a++%22chatId%22%3a+%2219%3ad65713bc498c4a428c71ef9353e6ce20%40thread.v2%22%2c%0d%0a++%22subEntityId%22%3a+null%0d%0a%7d&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924",
      "configuration": {
        "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
        "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
        "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
        "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
      },
      "teamsApp": {
        "id": "06805b9e-77e3-4b93-ac81-525eb87513b8",
        "displayName": "Contoso",
        "distributionMethod": "store"
      }
    },
    {
      "id": "1f7b40e5-ecdf-40cb-b02e-e785cf71c0e9",
      "displayName": "Website2",
      "teamsAppId": null,
      "sortOrderIndex": "10000100",
      "messageId": "1607411851584",
      "webUrl": "https://teams.microsoft.com/l/entity/com.microsoft.teamspace.tab.web/_djb2_msteams_prefix_44125e1d-04b1-421a-9f45-19d913494b3e?context=%7b%0d%0a++%22context%22%3a+%22chat%22%2c%0d%0a++%22chatId%22%3a+%2219%3ad65713bc498c4a428c71ef9353e6ce20%40thread.v2%22%2c%0d%0a++%22subEntityId%22%3a+null%0d%0a%7d&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924",
      "configuration": {
        "entityId": null,
        "contentUrl": "https://www.bing.com",
        "removeUrl": null,
        "websiteUrl": "https://www.bing.com",
        "dateAdded": "2020-12-08T07:17:29.748Z"
      },
      "teamsApp": {
        "id": "com.microsoft.teamspace.tab.web",
        "externalId": null,
        "displayName": "Website",
        "distributionMethod": "store"
      }
    },
    {
      "id": "b92dd123-1624-425c-a808-2f11e03534a5",
      "displayName": "Some random board",
      "sortOrderIndex": "10000100100",
      "messageId": "1607412162267",
      "webUrl": "https://teams.microsoft.com/l/entity/49e6f432-d79c-49e8-94f7-89b94f3672fd/_djb2_msteams_prefix_2919ec48-12d8-4533-b849-56c4d207734b?context=%7b%0d%0a++%22context%22%3a+%22chat%22%2c%0d%0a++%22chatId%22%3a+%2219%3ad65713bc498c4a428c71ef9353e6ce20%40thread.v2%22%2c%0d%0a++%22subEntityId%22%3a+null%0d%0a%7d&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924",
      "configuration": {
        "entityId": "5fcf29c17a3a3142160b8694",
        "contentUrl": "https://trello.com/integrations/teams/tab-content?iframeSource=msteams&contentUrl=https%3A%2F%2Ftrello.com%2Fb%2FkS2FslqK%2Fsome-random-board",
        "removeUrl": "https://trello.com/integrations/teams/tab-delete?iframeSource=msteams",
        "websiteUrl": "https://trello.com/b/kS2FslqK/some-random-board",
        "dateAdded": "2020-12-08T07:22:40.001Z"
      },
      "teamsApp": {
        "id": "49e6f432-d79c-49e8-94f7-89b94f3672fd",
        "externalId": null,
        "displayName": "Trello",
        "distributionMethod": "store"
      }
    }
  ]
}
```

### <a name="example-2-list-all-the-tabs-belonging-to-a-specific-app-in-a-chat"></a><span data-ttu-id="a55c3-138">Пример 2. Список всех вкладок, принадлежащих определенному приложению в чате</span><span class="sxs-lookup"><span data-stu-id="a55c3-138">Example 2: List all the tabs belonging to a specific app in a chat</span></span>
#### <a name="request"></a><span data-ttu-id="a55c3-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a55c3-139">Request</span></span>
<span data-ttu-id="a55c3-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a55c3-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_tabs_in_chat_app_filter"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs?$expand=teamsApp&$filter=teamsApp/id eq 'com.microsoft.teamspace.tab.web'
```


#### <a name="response"></a><span data-ttu-id="a55c3-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a55c3-141">Response</span></span>
<span data-ttu-id="a55c3-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a55c3-142">The following is an example of the response.</span></span>
><span data-ttu-id="a55c3-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a55c3-143">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamsTab)"
}
-->

```http
HTTP/1.1 200 Success
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats('19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2')/tabs(teamsApp())",
    "@odata.count": 1,
    "value": [
        {
            "id": "1f7b40e5-ecdf-40cb-b02e-e785cf71c0e9",
            "displayName": "Website2",
            "teamsAppId": null,
            "sortOrderIndex": "10000100",
            "messageId": "1607411851584",
            "webUrl": "https://teams.microsoft.com/l/entity/com.microsoft.teamspace.tab.web/_djb2_msteams_prefix_44125e1d-04b1-421a-9f45-19d913494b3e?context=%7b%0d%0a++%22context%22%3a+%22chat%22%2c%0d%0a++%22chatId%22%3a+%2219%3ad65713bc498c4a428c71ef9353e6ce20%40thread.v2%22%2c%0d%0a++%22subEntityId%22%3a+null%0d%0a%7d&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924",
            "configuration": {
                "entityId": null,
                "contentUrl": "https://www.bing.com",
                "removeUrl": null,
                "websiteUrl": "https://www.bing.com",
                "dateAdded": "2020-12-08T07:17:29.748Z"
            },
            "teamsApp": {
                "id": "com.microsoft.teamspace.tab.web",
                "externalId": null,
                "displayName": "Website",
                "distributionMethod": "store"
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="a55c3-144">См. также</span><span class="sxs-lookup"><span data-stu-id="a55c3-144">See also</span></span>

- [<span data-ttu-id="a55c3-145">Список вкладок на канале</span><span class="sxs-lookup"><span data-stu-id="a55c3-145">List tabs in channel</span></span>](channel-list-tabs.md)
- 
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List all tabs in chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


