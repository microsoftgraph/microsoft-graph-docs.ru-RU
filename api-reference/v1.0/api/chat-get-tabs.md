---
title: Получить вкладку в чате
description: 'Извлечение свойств и связей указанной вкладки в чате. '
author: subray
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ca4c9e882de974df8a7ffb79fc168593acaa3f61
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950161"
---
# <a name="get-tab-in-chat"></a><span data-ttu-id="bebed-103">Получить вкладку в чате</span><span class="sxs-lookup"><span data-stu-id="bebed-103">Get tab in chat</span></span>

<span data-ttu-id="bebed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bebed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bebed-105">Извлечение свойств и связей указанной [вкладки](../resources/teamstab.md) в [чате.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="bebed-105">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md) in a [chat](../resources/chat.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="bebed-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bebed-106">Permissions</span></span>
<span data-ttu-id="bebed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bebed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bebed-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bebed-109">Permission type</span></span>      | <span data-ttu-id="bebed-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bebed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bebed-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bebed-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bebed-112">TeamsTab.ReadWriteForChat, TeamsTab.Read.All, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bebed-112">TeamsTab.ReadWriteForChat, TeamsTab.Read.All, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="bebed-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bebed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bebed-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bebed-114">Not supported.</span></span>    |
|<span data-ttu-id="bebed-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bebed-115">Application</span></span> | <span data-ttu-id="bebed-116">TeamsTab.ReadWriteForChat.All, TeamsTab.Read.All, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bebed-116">TeamsTab.ReadWriteForChat.All, TeamsTab.Read.All, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="bebed-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bebed-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
GET /chats/{chat-id}/tabs/{tab-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bebed-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bebed-118">Optional query parameters</span></span>

<span data-ttu-id="bebed-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="bebed-119">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bebed-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bebed-120">Request headers</span></span>
| <span data-ttu-id="bebed-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bebed-121">Header</span></span>       | <span data-ttu-id="bebed-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bebed-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bebed-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bebed-123">Authorization</span></span>  | <span data-ttu-id="bebed-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bebed-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bebed-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bebed-126">Request body</span></span>
<span data-ttu-id="bebed-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bebed-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bebed-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="bebed-128">Response</span></span>

<span data-ttu-id="bebed-129">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [вкладки](../resources/teamstab.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bebed-129">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bebed-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bebed-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="bebed-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bebed-131">Request</span></span>
<span data-ttu-id="bebed-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bebed-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bebed-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bebed-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tab_in_chat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d?$expand=teamsApp
```
# <a name="c"></a>[<span data-ttu-id="bebed-134">C#</span><span class="sxs-lookup"><span data-stu-id="bebed-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tab-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bebed-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bebed-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tab-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bebed-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bebed-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tab-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bebed-137">Java</span><span class="sxs-lookup"><span data-stu-id="bebed-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tab-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="bebed-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="bebed-138">Response</span></span>
<span data-ttu-id="bebed-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bebed-139">The following is an example of the response.</span></span> 

><span data-ttu-id="bebed-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bebed-140">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsTab"
}
-->  

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "tabId",
  "displayName": "My Contoso Tab - updated",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "teamsApp": {
      "id": "0d820ecd-def2-4297-adad-78056cde7c78",
      "externalId": null,
      "displayName": "Contoso",
      "distributionMethod": "store"
  },
  "sortOrderIndex": "20",
  "messageId": "1607411534158",
  "webUrl": "https://teams.microsoft.com/l/entity/com.microsoft.teamspace.tab.web/_djb2_msteams_prefix_193fe248-24e6-478f-a66c-ede9ce6dd547?context=%7b%0d%0a++%22context%22%3a+%22chat%22%2c%0d%0a++%22chatId%22%3a+%2219%3ad65713bc498c4a428c71ef9353e6ce20%40thread.v2%22%2c%0d%0a++%22subEntityId%22%3a+null%0d%0a%7d&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924"
}
```

## <a name="see-also"></a><span data-ttu-id="bebed-141">См. также</span><span class="sxs-lookup"><span data-stu-id="bebed-141">See also</span></span>

- [<span data-ttu-id="bebed-142">Получение вкладки на канале</span><span class="sxs-lookup"><span data-stu-id="bebed-142">Get tab in channel</span></span>](channel-get-tabs.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a tab in chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


