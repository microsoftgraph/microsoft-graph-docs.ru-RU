---
title: Удаление вкладки из чата
description: 'Удаление (открепление) вкладки из указанного чата. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c83e8c9d1c501b27c46a6df3958008fb4447c06b
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607620"
---
# <a name="delete-tab-from-chat"></a><span data-ttu-id="cc952-103">Удаление вкладки из чата</span><span class="sxs-lookup"><span data-stu-id="cc952-103">Delete tab from chat</span></span>

<span data-ttu-id="cc952-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc952-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc952-105">Удаление (открепление) вкладки из указанного [чата](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="cc952-105">Remove (unpin) a tab from the specified [chat](../resources/chat.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="cc952-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc952-106">Permissions</span></span>
<span data-ttu-id="cc952-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc952-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc952-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc952-109">Permission type</span></span>      | <span data-ttu-id="cc952-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc952-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc952-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc952-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cc952-112">TeamsTab. Реадвритефорчат, TeamsTab. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cc952-112">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="cc952-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc952-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc952-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc952-114">Not supported.</span></span>    |
|<span data-ttu-id="cc952-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="cc952-115">Application</span></span> | <span data-ttu-id="cc952-116">TeamsTab. Реадвритефорчат, TeamsTab. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cc952-116">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="cc952-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc952-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /chats/{chat-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="cc952-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc952-118">Request headers</span></span>
| <span data-ttu-id="cc952-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc952-119">Header</span></span>       | <span data-ttu-id="cc952-120">Значение</span><span class="sxs-lookup"><span data-stu-id="cc952-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc952-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc952-121">Authorization</span></span>  | <span data-ttu-id="cc952-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc952-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc952-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc952-124">Request body</span></span>
<span data-ttu-id="cc952-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cc952-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc952-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc952-126">Response</span></span>

<span data-ttu-id="cc952-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cc952-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc952-129">Пример</span><span class="sxs-lookup"><span data-stu-id="cc952-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="cc952-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc952-130">Request</span></span>
<span data-ttu-id="cc952-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc952-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tab_in_chat"
}-->
```http
DELETE https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d
```
### <a name="response"></a><span data-ttu-id="cc952-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc952-132">Response</span></span>
<span data-ttu-id="cc952-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc952-133">The following is an example of the response.</span></span> <span data-ttu-id="cc952-134">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="cc952-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cc952-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc952-135">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
}
-->

```http
HTTP/1.1 204 No Content
```
## <a name="see-also"></a><span data-ttu-id="cc952-136">См. также</span><span class="sxs-lookup"><span data-stu-id="cc952-136">See also</span></span>

- [<span data-ttu-id="cc952-137">Удаление вкладки из канала</span><span class="sxs-lookup"><span data-stu-id="cc952-137">Delete tab from channel</span></span>](channel-delete-tabs.md)

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


