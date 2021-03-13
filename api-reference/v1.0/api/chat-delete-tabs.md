---
title: Удаление вкладки из чата
description: 'Удалите (открепите) вкладку из указанного чата. '
author: subray
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 70fb781618c094406948b52e4c8068163ad1808e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777589"
---
# <a name="delete-tab-from-chat"></a><span data-ttu-id="9c84e-103">Удаление вкладки из чата</span><span class="sxs-lookup"><span data-stu-id="9c84e-103">Delete tab from chat</span></span>

<span data-ttu-id="9c84e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c84e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9c84e-105">Удалите (открепите) вкладку из указанного [чата.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="9c84e-105">Remove (unpin) a tab from the specified [chat](../resources/chat.md).</span></span> 

> <span data-ttu-id="9c84e-106">**Примечание.** Если чат связан с экземпляром [onlineMeeting,](../resources/onlinemeeting.md) вкладка будет удалена с собрания.</span><span class="sxs-lookup"><span data-stu-id="9c84e-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the tab will get removed from the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c84e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c84e-107">Permissions</span></span>
<span data-ttu-id="9c84e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c84e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c84e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c84e-110">Permission type</span></span>      | <span data-ttu-id="9c84e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c84e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c84e-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c84e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9c84e-113">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c84e-113">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="9c84e-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c84e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c84e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c84e-115">Not supported.</span></span>    |
|<span data-ttu-id="9c84e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9c84e-116">Application</span></span> | <span data-ttu-id="9c84e-117">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c84e-117">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="9c84e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c84e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /chats/{chat-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="9c84e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c84e-119">Request headers</span></span>
| <span data-ttu-id="9c84e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9c84e-120">Header</span></span>       | <span data-ttu-id="9c84e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9c84e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9c84e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c84e-122">Authorization</span></span>  | <span data-ttu-id="9c84e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c84e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9c84e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c84e-125">Request body</span></span>
<span data-ttu-id="9c84e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9c84e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c84e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c84e-127">Response</span></span>

<span data-ttu-id="9c84e-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9c84e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c84e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9c84e-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="9c84e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c84e-131">Request</span></span>
<span data-ttu-id="9c84e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c84e-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_tab_in_chat"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d
```


### <a name="response"></a><span data-ttu-id="9c84e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c84e-133">Response</span></span>
<span data-ttu-id="9c84e-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9c84e-134">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
}
-->

```http
HTTP/1.1 204 No Content
```
## <a name="see-also"></a><span data-ttu-id="9c84e-135">См. также</span><span class="sxs-lookup"><span data-stu-id="9c84e-135">See also</span></span>

- [<span data-ttu-id="9c84e-136">Удаление вкладки из канала</span><span class="sxs-lookup"><span data-stu-id="9c84e-136">Delete tab from channel</span></span>](channel-delete-tabs.md)

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


