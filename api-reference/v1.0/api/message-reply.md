---
title: 'message: reply'
description: Ответ отправителю сообщения. После этого сообщение сохраняется в папке "Отправленные".
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 2ba3df6551aab9138e90fa5e3fc452f2929b4815
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856325"
---
# <a name="message-reply"></a><span data-ttu-id="5c20f-104">message: reply</span><span class="sxs-lookup"><span data-stu-id="5c20f-104">message: reply</span></span>

<span data-ttu-id="5c20f-p102">Ответ отправителю сообщения. После этого сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="5c20f-p102">Reply to the sender of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c20f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c20f-107">Permissions</span></span>
<span data-ttu-id="5c20f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c20f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c20f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c20f-110">Permission type</span></span>      | <span data-ttu-id="5c20f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c20f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c20f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c20f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5c20f-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="5c20f-113">Mail.Send</span></span>    |
|<span data-ttu-id="5c20f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c20f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c20f-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="5c20f-115">Mail.Send</span></span>    |
|<span data-ttu-id="5c20f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c20f-116">Application</span></span> | <span data-ttu-id="5c20f-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="5c20f-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c20f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c20f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="5c20f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c20f-119">Request headers</span></span>
| <span data-ttu-id="5c20f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5c20f-120">Name</span></span>       | <span data-ttu-id="5c20f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5c20f-121">Type</span></span> | <span data-ttu-id="5c20f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5c20f-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5c20f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c20f-123">Authorization</span></span>  | <span data-ttu-id="5c20f-124">string</span><span class="sxs-lookup"><span data-stu-id="5c20f-124">string</span></span>  | <span data-ttu-id="5c20f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c20f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5c20f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5c20f-127">Content-Type</span></span> | <span data-ttu-id="5c20f-128">string</span><span class="sxs-lookup"><span data-stu-id="5c20f-128">string</span></span>  | <span data-ttu-id="5c20f-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c20f-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c20f-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c20f-131">Request body</span></span>
<span data-ttu-id="5c20f-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5c20f-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5c20f-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="5c20f-133">Parameter</span></span>    | <span data-ttu-id="5c20f-134">Тип</span><span class="sxs-lookup"><span data-stu-id="5c20f-134">Type</span></span>   |<span data-ttu-id="5c20f-135">Описание</span><span class="sxs-lookup"><span data-stu-id="5c20f-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c20f-136">comment</span><span class="sxs-lookup"><span data-stu-id="5c20f-136">comment</span></span>|<span data-ttu-id="5c20f-137">String</span><span class="sxs-lookup"><span data-stu-id="5c20f-137">String</span></span>|<span data-ttu-id="5c20f-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="5c20f-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="5c20f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c20f-140">Response</span></span>

<span data-ttu-id="5c20f-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5c20f-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c20f-143">Пример</span><span class="sxs-lookup"><span data-stu-id="5c20f-143">Example</span></span>
<span data-ttu-id="5c20f-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5c20f-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5c20f-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c20f-145">Request</span></span>
<span data-ttu-id="5c20f-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c20f-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/reply
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```

##### <a name="response"></a><span data-ttu-id="5c20f-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c20f-147">Response</span></span>
##### <a name="response"></a><span data-ttu-id="5c20f-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c20f-148">Response</span></span>
<span data-ttu-id="5c20f-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5c20f-149">Here is an example of the response.</span></span>
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
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
