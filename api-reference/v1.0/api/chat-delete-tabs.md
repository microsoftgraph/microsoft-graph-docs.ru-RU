---
title: Удаление вкладки из чата
description: 'Удалите (открепите) вкладку из указанного чата. '
author: subray
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b5885926bd9abbe85392a30da7dedf8db22a2692
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958385"
---
# <a name="delete-tab-from-chat"></a><span data-ttu-id="4a912-103">Удаление вкладки из чата</span><span class="sxs-lookup"><span data-stu-id="4a912-103">Delete tab from chat</span></span>

<span data-ttu-id="4a912-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a912-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4a912-105">Удалите (открепите) вкладку из указанного [чата.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="4a912-105">Remove (unpin) a tab from the specified [chat](../resources/chat.md).</span></span> 

> <span data-ttu-id="4a912-106">**Примечание.** Если чат связан с экземпляром [onlineMeeting,](../resources/onlinemeeting.md) вкладка будет удалена с собрания.</span><span class="sxs-lookup"><span data-stu-id="4a912-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the tab will get removed from the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a912-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a912-107">Permissions</span></span>
<span data-ttu-id="4a912-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a912-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a912-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a912-110">Permission type</span></span>      | <span data-ttu-id="4a912-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a912-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a912-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a912-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4a912-113">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a912-113">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="4a912-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a912-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a912-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a912-115">Not supported.</span></span>    |
|<span data-ttu-id="4a912-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a912-116">Application</span></span> | <span data-ttu-id="4a912-117">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a912-117">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="4a912-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a912-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /chats/{chat-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="4a912-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a912-119">Request headers</span></span>
| <span data-ttu-id="4a912-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a912-120">Header</span></span>       | <span data-ttu-id="4a912-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4a912-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4a912-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a912-122">Authorization</span></span>  | <span data-ttu-id="4a912-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a912-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4a912-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a912-125">Request body</span></span>
<span data-ttu-id="4a912-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a912-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a912-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a912-127">Response</span></span>

<span data-ttu-id="4a912-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4a912-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a912-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4a912-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="4a912-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a912-131">Request</span></span>
<span data-ttu-id="4a912-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a912-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4a912-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a912-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tab_in_chat"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d
```
# <a name="c"></a>[<span data-ttu-id="4a912-134">C#</span><span class="sxs-lookup"><span data-stu-id="4a912-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tab-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a912-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a912-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tab-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a912-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a912-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tab-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a912-137">Java</span><span class="sxs-lookup"><span data-stu-id="4a912-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tab-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4a912-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a912-138">Response</span></span>
<span data-ttu-id="4a912-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4a912-139">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
}
-->

```http
HTTP/1.1 204 No Content
```
## <a name="see-also"></a><span data-ttu-id="4a912-140">См. также</span><span class="sxs-lookup"><span data-stu-id="4a912-140">See also</span></span>

- [<span data-ttu-id="4a912-141">Удаление вкладки из канала</span><span class="sxs-lookup"><span data-stu-id="4a912-141">Delete tab from channel</span></span>](channel-delete-tabs.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete tab from chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


