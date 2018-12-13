---
title: 'conversationThread: reply'
description: 'Ответ на поток во время групповой беседы и добавьте новую запись. Можно указать родительский беседы '
ms.openlocfilehash: 9e191a53b2427b8c9def2acf15d48b7c8605437f
ms.sourcegitcommit: 9f953e0c4cd624ba31919bfd5e82bf3e33cb9e21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/13/2018
ms.locfileid: "27245080"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="47798-104">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="47798-104">conversationThread: reply</span></span>

<span data-ttu-id="47798-p102">Ответ на цепочку в беседе группы и добавление в нее новой записи. Вы можете указать в запросе всю родительскую беседу или только цепочку.</span><span class="sxs-lookup"><span data-stu-id="47798-p102">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="47798-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47798-107">Permissions</span></span>
<span data-ttu-id="47798-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47798-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47798-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47798-110">Permission type</span></span>      | <span data-ttu-id="47798-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47798-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47798-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47798-112">Delegated (work or school account)</span></span> | <span data-ttu-id="47798-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47798-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="47798-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47798-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47798-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47798-115">Not supported.</span></span>    |
|<span data-ttu-id="47798-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47798-116">Application</span></span> | <span data-ttu-id="47798-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47798-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="47798-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47798-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="47798-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47798-119">Request headers</span></span>
| <span data-ttu-id="47798-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47798-120">Header</span></span>       | <span data-ttu-id="47798-121">Значение</span><span class="sxs-lookup"><span data-stu-id="47798-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="47798-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47798-122">Authorization</span></span>  | <span data-ttu-id="47798-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47798-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="47798-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="47798-125">Content-Type</span></span>  | <span data-ttu-id="47798-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47798-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="47798-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47798-128">Request body</span></span>
<span data-ttu-id="47798-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="47798-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="47798-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="47798-130">Parameter</span></span>    | <span data-ttu-id="47798-131">Тип</span><span class="sxs-lookup"><span data-stu-id="47798-131">Type</span></span>   |<span data-ttu-id="47798-132">Описание</span><span class="sxs-lookup"><span data-stu-id="47798-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47798-133">post</span><span class="sxs-lookup"><span data-stu-id="47798-133">post</span></span>|[<span data-ttu-id="47798-134">post</span><span class="sxs-lookup"><span data-stu-id="47798-134">post</span></span>](../resources/post.md)|<span data-ttu-id="47798-135">Новая запись для ответа.</span><span class="sxs-lookup"><span data-stu-id="47798-135">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="47798-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="47798-136">Response</span></span>

<span data-ttu-id="47798-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="47798-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47798-139">Пример</span><span class="sxs-lookup"><span data-stu-id="47798-139">Example</span></span>
<span data-ttu-id="47798-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="47798-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="47798-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="47798-141">Request</span></span>
<span data-ttu-id="47798-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47798-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/reply
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

##### <a name="response"></a><span data-ttu-id="47798-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="47798-143">Response</span></span>
<span data-ttu-id="47798-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="47798-144">Here is an example of the response.</span></span>
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
