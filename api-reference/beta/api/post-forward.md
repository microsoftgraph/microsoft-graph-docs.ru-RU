---
title: 'post: forward'
description: 'Переадресация публикации получателю. Можно указать в приглашении на родительский беседы и поток '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 557eaa7455600fe6da864a70457b4f3094df8c41
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512054"
---
# <a name="post-forward"></a><span data-ttu-id="a8480-104">post: forward</span><span class="sxs-lookup"><span data-stu-id="a8480-104">post: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8480-p102">Пересылка записи получателю. Вы можете указать в запросе родительскую беседу вместе с цепочкой или только родительскую цепочку.</span><span class="sxs-lookup"><span data-stu-id="a8480-p102">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a8480-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8480-107">Permissions</span></span>
<span data-ttu-id="a8480-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8480-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8480-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8480-110">Permission type</span></span>      | <span data-ttu-id="a8480-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8480-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8480-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8480-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a8480-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8480-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a8480-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8480-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8480-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8480-115">Not supported.</span></span>    |
|<span data-ttu-id="a8480-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8480-116">Application</span></span> | <span data-ttu-id="a8480-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8480-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8480-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8480-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="a8480-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8480-119">Request headers</span></span>
| <span data-ttu-id="a8480-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8480-120">Header</span></span>       | <span data-ttu-id="a8480-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a8480-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a8480-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8480-122">Authorization</span></span>  | <span data-ttu-id="a8480-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8480-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a8480-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8480-125">Request body</span></span>
<span data-ttu-id="a8480-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a8480-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a8480-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="a8480-127">Parameter</span></span>    | <span data-ttu-id="a8480-128">Тип</span><span class="sxs-lookup"><span data-stu-id="a8480-128">Type</span></span>   |<span data-ttu-id="a8480-129">Описание</span><span class="sxs-lookup"><span data-stu-id="a8480-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8480-130">comment</span><span class="sxs-lookup"><span data-stu-id="a8480-130">comment</span></span>|<span data-ttu-id="a8480-131">String</span><span class="sxs-lookup"><span data-stu-id="a8480-131">String</span></span>|<span data-ttu-id="a8480-132">Необязательный комментарий, который пересылается вместе с записью.</span><span class="sxs-lookup"><span data-stu-id="a8480-132">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="a8480-133">toRecipients</span><span class="sxs-lookup"><span data-stu-id="a8480-133">toRecipients</span></span>|<span data-ttu-id="a8480-134">Коллекция объектов [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="a8480-134">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="a8480-135">Получатели, которым пересылается цепочка.</span><span class="sxs-lookup"><span data-stu-id="a8480-135">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="a8480-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8480-136">Response</span></span>

<span data-ttu-id="a8480-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a8480-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8480-139">Пример</span><span class="sxs-lookup"><span data-stu-id="a8480-139">Example</span></span>
<span data-ttu-id="a8480-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a8480-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a8480-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8480-141">Request</span></span>
<span data-ttu-id="a8480-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8480-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a8480-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8480-143">Response</span></span>
<span data-ttu-id="a8480-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a8480-144">Here is an example of the response.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/post-forward.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
