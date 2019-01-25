---
title: 'conversationThread: reply'
description: 'Ответ на поток во время групповой беседы и добавьте новую запись. Можно указать родительский беседы '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 54609d291180fba6bc771ac2932ff3ef25d5d82f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513517"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="ad2aa-104">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="ad2aa-104">conversationThread: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad2aa-p102">Ответ на цепочку в беседе группы и добавление в нее новой записи. Вы можете указать в запросе всю родительскую беседу или только цепочку.</span><span class="sxs-lookup"><span data-stu-id="ad2aa-p102">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad2aa-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad2aa-107">Permissions</span></span>
<span data-ttu-id="ad2aa-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad2aa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad2aa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad2aa-110">Permission type</span></span>      | <span data-ttu-id="ad2aa-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad2aa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad2aa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad2aa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ad2aa-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad2aa-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad2aa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad2aa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad2aa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad2aa-115">Not supported.</span></span>    |
|<span data-ttu-id="ad2aa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad2aa-116">Application</span></span> | <span data-ttu-id="ad2aa-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad2aa-117">Not supported.</span></span>    |

## <a name="http-request"></a><span data-ttu-id="ad2aa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad2aa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="ad2aa-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad2aa-119">Request headers</span></span>
| <span data-ttu-id="ad2aa-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad2aa-120">Header</span></span>       | <span data-ttu-id="ad2aa-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ad2aa-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ad2aa-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad2aa-122">Authorization</span></span>  | <span data-ttu-id="ad2aa-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad2aa-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ad2aa-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ad2aa-125">Content-Type</span></span>  | <span data-ttu-id="ad2aa-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad2aa-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ad2aa-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad2aa-128">Request body</span></span>
<span data-ttu-id="ad2aa-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ad2aa-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ad2aa-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="ad2aa-130">Parameter</span></span>    | <span data-ttu-id="ad2aa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ad2aa-131">Type</span></span>   |<span data-ttu-id="ad2aa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ad2aa-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad2aa-133">post</span><span class="sxs-lookup"><span data-stu-id="ad2aa-133">post</span></span>|[<span data-ttu-id="ad2aa-134">post</span><span class="sxs-lookup"><span data-stu-id="ad2aa-134">post</span></span>](../resources/post.md)|<span data-ttu-id="ad2aa-135">Новая запись для ответа.</span><span class="sxs-lookup"><span data-stu-id="ad2aa-135">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="ad2aa-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad2aa-136">Response</span></span>

<span data-ttu-id="ad2aa-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ad2aa-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad2aa-139">Пример</span><span class="sxs-lookup"><span data-stu-id="ad2aa-139">Example</span></span>
<span data-ttu-id="ad2aa-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ad2aa-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ad2aa-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad2aa-141">Request</span></span>
<span data-ttu-id="ad2aa-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad2aa-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ad2aa-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad2aa-143">Response</span></span>
<span data-ttu-id="ad2aa-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ad2aa-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/conversationthread-reply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
