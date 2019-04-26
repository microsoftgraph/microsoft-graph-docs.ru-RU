---
title: 'post: forward'
description: 'Переадресация публикации получателю. Вы можете указать родительский сеанс связи и поток в запросе, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 1c2bc617bb1867f5debd90a9f23f9aa3a6761476
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332230"
---
# <a name="post-forward"></a><span data-ttu-id="eeab4-104">post: forward</span><span class="sxs-lookup"><span data-stu-id="eeab4-104">post: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eeab4-p102">Пересылка записи получателю. Вы можете указать в запросе родительскую беседу вместе с цепочкой или только родительскую цепочку.</span><span class="sxs-lookup"><span data-stu-id="eeab4-p102">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="eeab4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eeab4-107">Permissions</span></span>
<span data-ttu-id="eeab4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eeab4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eeab4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eeab4-110">Permission type</span></span>      | <span data-ttu-id="eeab4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eeab4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eeab4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eeab4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eeab4-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eeab4-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="eeab4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eeab4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eeab4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eeab4-115">Not supported.</span></span>    |
|<span data-ttu-id="eeab4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eeab4-116">Application</span></span> | <span data-ttu-id="eeab4-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eeab4-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eeab4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eeab4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="eeab4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eeab4-119">Request headers</span></span>
| <span data-ttu-id="eeab4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eeab4-120">Header</span></span>       | <span data-ttu-id="eeab4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="eeab4-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eeab4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eeab4-122">Authorization</span></span>  | <span data-ttu-id="eeab4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eeab4-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eeab4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eeab4-125">Request body</span></span>
<span data-ttu-id="eeab4-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="eeab4-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eeab4-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="eeab4-127">Parameter</span></span>    | <span data-ttu-id="eeab4-128">Тип</span><span class="sxs-lookup"><span data-stu-id="eeab4-128">Type</span></span>   |<span data-ttu-id="eeab4-129">Описание</span><span class="sxs-lookup"><span data-stu-id="eeab4-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eeab4-130">comment</span><span class="sxs-lookup"><span data-stu-id="eeab4-130">comment</span></span>|<span data-ttu-id="eeab4-131">String</span><span class="sxs-lookup"><span data-stu-id="eeab4-131">String</span></span>|<span data-ttu-id="eeab4-132">Необязательный комментарий, который пересылается вместе с записью.</span><span class="sxs-lookup"><span data-stu-id="eeab4-132">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="eeab4-133">toRecipients</span><span class="sxs-lookup"><span data-stu-id="eeab4-133">toRecipients</span></span>|<span data-ttu-id="eeab4-134">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="eeab4-134">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="eeab4-135">Получатели, которым пересылается цепочка.</span><span class="sxs-lookup"><span data-stu-id="eeab4-135">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="eeab4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="eeab4-136">Response</span></span>

<span data-ttu-id="eeab4-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="eeab4-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eeab4-139">Пример</span><span class="sxs-lookup"><span data-stu-id="eeab4-139">Example</span></span>
<span data-ttu-id="eeab4-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="eeab4-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="eeab4-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="eeab4-141">Request</span></span>
<span data-ttu-id="eeab4-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eeab4-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="eeab4-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="eeab4-143">Response</span></span>
<span data-ttu-id="eeab4-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eeab4-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
