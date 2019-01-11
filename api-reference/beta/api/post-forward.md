---
title: 'post: forward'
description: 'Переадресация публикации получателю. Можно указать в приглашении на родительский беседы и поток '
localization_priority: Normal
ms.openlocfilehash: 64b7d87745cf897ea827d37a9cd4f4c60d197068
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889441"
---
# <a name="post-forward"></a><span data-ttu-id="b37dc-104">post: forward</span><span class="sxs-lookup"><span data-stu-id="b37dc-104">post: forward</span></span>

> <span data-ttu-id="b37dc-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b37dc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b37dc-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b37dc-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b37dc-p103">Пересылка записи получателю. Вы можете указать в запросе родительскую беседу вместе с цепочкой или только родительскую цепочку.</span><span class="sxs-lookup"><span data-stu-id="b37dc-p103">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b37dc-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b37dc-109">Permissions</span></span>
<span data-ttu-id="b37dc-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b37dc-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b37dc-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b37dc-112">Permission type</span></span>      | <span data-ttu-id="b37dc-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b37dc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b37dc-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b37dc-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b37dc-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b37dc-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b37dc-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b37dc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b37dc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b37dc-117">Not supported.</span></span>    |
|<span data-ttu-id="b37dc-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b37dc-118">Application</span></span> | <span data-ttu-id="b37dc-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b37dc-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b37dc-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b37dc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="b37dc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b37dc-121">Request headers</span></span>
| <span data-ttu-id="b37dc-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b37dc-122">Header</span></span>       | <span data-ttu-id="b37dc-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b37dc-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b37dc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b37dc-124">Authorization</span></span>  | <span data-ttu-id="b37dc-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b37dc-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b37dc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b37dc-127">Request body</span></span>
<span data-ttu-id="b37dc-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b37dc-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b37dc-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="b37dc-129">Parameter</span></span>    | <span data-ttu-id="b37dc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b37dc-130">Type</span></span>   |<span data-ttu-id="b37dc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b37dc-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b37dc-132">comment</span><span class="sxs-lookup"><span data-stu-id="b37dc-132">comment</span></span>|<span data-ttu-id="b37dc-133">String</span><span class="sxs-lookup"><span data-stu-id="b37dc-133">String</span></span>|<span data-ttu-id="b37dc-134">Необязательный комментарий, который пересылается вместе с записью.</span><span class="sxs-lookup"><span data-stu-id="b37dc-134">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="b37dc-135">toRecipients</span><span class="sxs-lookup"><span data-stu-id="b37dc-135">toRecipients</span></span>|<span data-ttu-id="b37dc-136">Коллекция объектов [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="b37dc-136">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="b37dc-137">Получатели, которым пересылается цепочка.</span><span class="sxs-lookup"><span data-stu-id="b37dc-137">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="b37dc-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b37dc-138">Response</span></span>

<span data-ttu-id="b37dc-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b37dc-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b37dc-141">Пример</span><span class="sxs-lookup"><span data-stu-id="b37dc-141">Example</span></span>
<span data-ttu-id="b37dc-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b37dc-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b37dc-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="b37dc-143">Request</span></span>
<span data-ttu-id="b37dc-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b37dc-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="b37dc-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="b37dc-145">Response</span></span>
<span data-ttu-id="b37dc-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b37dc-146">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
