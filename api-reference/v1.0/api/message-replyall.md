---
title: 'message: replyAll'
description: Ответ всем получателям сообщения. После этого сообщение сохраняется в папке "Отправленные".
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 8e2d9b2481e4fb0fc4e6e166dae1189baa77b7e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884310"
---
# <a name="message-replyall"></a><span data-ttu-id="0aaef-104">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="0aaef-104">message: replyAll</span></span>

<span data-ttu-id="0aaef-p102">Ответ всем получателям сообщения. После этого сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="0aaef-p102">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="0aaef-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0aaef-107">Permissions</span></span>
<span data-ttu-id="0aaef-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0aaef-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0aaef-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0aaef-110">Permission type</span></span>      | <span data-ttu-id="0aaef-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0aaef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0aaef-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0aaef-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0aaef-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0aaef-113">Mail.Send</span></span>    |
|<span data-ttu-id="0aaef-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0aaef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0aaef-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0aaef-115">Mail.Send</span></span>    |
|<span data-ttu-id="0aaef-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0aaef-116">Application</span></span> | <span data-ttu-id="0aaef-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0aaef-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="0aaef-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0aaef-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="0aaef-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0aaef-119">Request headers</span></span>
| <span data-ttu-id="0aaef-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0aaef-120">Name</span></span>       | <span data-ttu-id="0aaef-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0aaef-121">Type</span></span> | <span data-ttu-id="0aaef-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0aaef-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0aaef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0aaef-123">Authorization</span></span>  | <span data-ttu-id="0aaef-124">string</span><span class="sxs-lookup"><span data-stu-id="0aaef-124">string</span></span>  | <span data-ttu-id="0aaef-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0aaef-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0aaef-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0aaef-127">Content-Type</span></span> | <span data-ttu-id="0aaef-128">string</span><span class="sxs-lookup"><span data-stu-id="0aaef-128">string</span></span>  | <span data-ttu-id="0aaef-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0aaef-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0aaef-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0aaef-131">Request body</span></span>
<span data-ttu-id="0aaef-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0aaef-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0aaef-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="0aaef-133">Parameter</span></span>    | <span data-ttu-id="0aaef-134">Тип</span><span class="sxs-lookup"><span data-stu-id="0aaef-134">Type</span></span>   |<span data-ttu-id="0aaef-135">Описание</span><span class="sxs-lookup"><span data-stu-id="0aaef-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0aaef-136">comment</span><span class="sxs-lookup"><span data-stu-id="0aaef-136">comment</span></span>|<span data-ttu-id="0aaef-137">String</span><span class="sxs-lookup"><span data-stu-id="0aaef-137">String</span></span>|<span data-ttu-id="0aaef-p106">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="0aaef-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="0aaef-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="0aaef-140">Response</span></span>

<span data-ttu-id="0aaef-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0aaef-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0aaef-143">Пример</span><span class="sxs-lookup"><span data-stu-id="0aaef-143">Example</span></span>
<span data-ttu-id="0aaef-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0aaef-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0aaef-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="0aaef-145">Request</span></span>
<span data-ttu-id="0aaef-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0aaef-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/replyAll
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```


##### <a name="response"></a><span data-ttu-id="0aaef-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="0aaef-147">Response</span></span>
<span data-ttu-id="0aaef-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0aaef-148">Here is an example of the response.</span></span>
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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
