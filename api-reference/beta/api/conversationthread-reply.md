---
title: 'conversationThread: reply'
description: 'Ответ на поток во время групповой беседы и добавьте новую запись. Можно указать родительский беседы '
author: dkershaw10
ms.openlocfilehash: 9e439901fd2fa9c37ab30c746628e7fcd771edc2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314100"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="8fa6a-104">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="8fa6a-104">conversationThread: reply</span></span>

> <span data-ttu-id="8fa6a-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8fa6a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8fa6a-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fa6a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8fa6a-p103">Ответ на цепочку в беседе группы и добавление в нее новой записи. Вы можете указать в запросе всю родительскую беседу или только цепочку.</span><span class="sxs-lookup"><span data-stu-id="8fa6a-p103">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="8fa6a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8fa6a-109">Permissions</span></span>
<span data-ttu-id="8fa6a-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fa6a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fa6a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8fa6a-112">Permission type</span></span>      | <span data-ttu-id="8fa6a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8fa6a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fa6a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8fa6a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8fa6a-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fa6a-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8fa6a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8fa6a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fa6a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fa6a-117">Not supported.</span></span>    |
|<span data-ttu-id="8fa6a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8fa6a-118">Application</span></span> | <span data-ttu-id="8fa6a-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fa6a-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8fa6a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8fa6a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="8fa6a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8fa6a-121">Request headers</span></span>
| <span data-ttu-id="8fa6a-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8fa6a-122">Header</span></span>       | <span data-ttu-id="8fa6a-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8fa6a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8fa6a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8fa6a-124">Authorization</span></span>  | <span data-ttu-id="8fa6a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8fa6a-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8fa6a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8fa6a-127">Content-Type</span></span>  | <span data-ttu-id="8fa6a-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8fa6a-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8fa6a-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8fa6a-130">Request body</span></span>
<span data-ttu-id="8fa6a-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8fa6a-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8fa6a-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="8fa6a-132">Parameter</span></span>    | <span data-ttu-id="8fa6a-133">Тип</span><span class="sxs-lookup"><span data-stu-id="8fa6a-133">Type</span></span>   |<span data-ttu-id="8fa6a-134">Описание</span><span class="sxs-lookup"><span data-stu-id="8fa6a-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fa6a-135">post</span><span class="sxs-lookup"><span data-stu-id="8fa6a-135">post</span></span>|[<span data-ttu-id="8fa6a-136">post</span><span class="sxs-lookup"><span data-stu-id="8fa6a-136">post</span></span>](../resources/post.md)|<span data-ttu-id="8fa6a-137">Новая запись для ответа.</span><span class="sxs-lookup"><span data-stu-id="8fa6a-137">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="8fa6a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fa6a-138">Response</span></span>

<span data-ttu-id="8fa6a-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8fa6a-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fa6a-141">Пример</span><span class="sxs-lookup"><span data-stu-id="8fa6a-141">Example</span></span>
<span data-ttu-id="8fa6a-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8fa6a-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8fa6a-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="8fa6a-143">Request</span></span>
<span data-ttu-id="8fa6a-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8fa6a-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    }
  }
}
```

##### <a name="response"></a><span data-ttu-id="8fa6a-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="8fa6a-145">Response</span></span>
<span data-ttu-id="8fa6a-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8fa6a-146">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
