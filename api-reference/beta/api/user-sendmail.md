---
title: Отправка почты
description: Отправка сообщения, указанного в теле запроса. Сообщение сохраняется в папке "Отправленные" по умолчанию.
ms.openlocfilehash: 8103a1f0b4004e602c23d114e199b60fa96c15e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081970"
---
# <a name="send-mail"></a><span data-ttu-id="9678c-104">Отправка почты</span><span class="sxs-lookup"><span data-stu-id="9678c-104">Send mail</span></span>

> <span data-ttu-id="9678c-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9678c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9678c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9678c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9678c-p103">Отправка сообщения, указанного в теле запроса. Сообщение сохраняется в папке "Отправленные" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9678c-p103">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="9678c-109">В одном вызове действие **sendMail** можно выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="9678c-109">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="9678c-110">Включить [вложения](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="9678c-110">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="9678c-111">Используйте [упомянуть](../resources/mention.md) помечать другого пользователя в новое сообщение</span><span class="sxs-lookup"><span data-stu-id="9678c-111">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="9678c-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9678c-112">Permissions</span></span>
<span data-ttu-id="9678c-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9678c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9678c-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9678c-115">Permission type</span></span>      | <span data-ttu-id="9678c-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9678c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9678c-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9678c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="9678c-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9678c-118">Mail.Send</span></span>    |
|<span data-ttu-id="9678c-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9678c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9678c-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9678c-120">Mail.Send</span></span>    |
|<span data-ttu-id="9678c-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9678c-121">Application</span></span> | <span data-ttu-id="9678c-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9678c-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="9678c-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9678c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="9678c-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9678c-124">Request headers</span></span>
| <span data-ttu-id="9678c-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9678c-125">Header</span></span>       | <span data-ttu-id="9678c-126">Значение</span><span class="sxs-lookup"><span data-stu-id="9678c-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9678c-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9678c-127">Authorization</span></span>  | <span data-ttu-id="9678c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9678c-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9678c-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9678c-130">Content-Type</span></span>  | <span data-ttu-id="9678c-131">application/json</span><span class="sxs-lookup"><span data-stu-id="9678c-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9678c-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9678c-132">Request body</span></span>
<span data-ttu-id="9678c-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9678c-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9678c-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="9678c-134">Parameter</span></span>    | <span data-ttu-id="9678c-135">Тип</span><span class="sxs-lookup"><span data-stu-id="9678c-135">Type</span></span>   |<span data-ttu-id="9678c-136">Описание</span><span class="sxs-lookup"><span data-stu-id="9678c-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9678c-137">Message</span><span class="sxs-lookup"><span data-stu-id="9678c-137">Message</span></span>|[<span data-ttu-id="9678c-138">Message</span><span class="sxs-lookup"><span data-stu-id="9678c-138">Message</span></span>](../resources/message.md)|<span data-ttu-id="9678c-p106">Отправляемое сообщение. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9678c-p106">The message to send. Required.</span></span>|
|<span data-ttu-id="9678c-141">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="9678c-141">SaveToSentItems</span></span>|<span data-ttu-id="9678c-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="9678c-142">Boolean</span></span>|<span data-ttu-id="9678c-p107">Указывает, нужно ли сохранять сообщение в папке "Отправленные". Указывайте этот параметр, если задано значение false (по умолчанию используется true).  Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9678c-p107">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="9678c-146">Если вы хотите использовать **упомянуть** помечать другого пользователя в новое сообщение:</span><span class="sxs-lookup"><span data-stu-id="9678c-146">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="9678c-147">Включите свойства необходимые **toRecipients** , свойство **упоминания** и все свойства для записи сообщений в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="9678c-147">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="9678c-148">Для каждого упоминаются в свойстве **упоминания** необходимо указать свойство **упомянутые** .</span><span class="sxs-lookup"><span data-stu-id="9678c-148">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="9678c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="9678c-149">Response</span></span>

<span data-ttu-id="9678c-p108">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9678c-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9678c-152">Пример</span><span class="sxs-lookup"><span data-stu-id="9678c-152">Example</span></span>
<span data-ttu-id="9678c-153">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9678c-153">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="9678c-154">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="9678c-154">Request 1</span></span>
<span data-ttu-id="9678c-155">Ниже приведен пример запроса для создания и отправки сообщения во время выполнения.</span><span class="sxs-lookup"><span data-stu-id="9678c-155">Here is an example of the request to create and send a message on the fly.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: application/json
Content-length: 512

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "samanthab@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients": [
      {
        "emailAddress": {
          "address": "danas@contoso.onmicrosoft.com"
        }
      }
    ]
  },
  "saveToSentItems": "false"
}
```

##### <a name="response-1"></a><span data-ttu-id="9678c-156">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="9678c-156">Response 1</span></span>
<span data-ttu-id="9678c-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9678c-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


##### <a name="request-2"></a><span data-ttu-id="9678c-158">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="9678c-158">Request 2</span></span>
<span data-ttu-id="9678c-159">В следующем примере показаны сообщения, пользователь выполнил вход в Samantha стенда.</span><span class="sxs-lookup"><span data-stu-id="9678c-159">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="9678c-160">Сообщение также включает в себя упоминание другому пользователю, Swope Дану.</span><span class="sxs-lookup"><span data-stu-id="9678c-160">The message also includes a mention of another user, Dana Swope.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_mentions"
}-->
```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: application/json
Content-length: 344

{
  "Message": {
    "subject": "Project kickoff",
    "toRecipients":[
      {
          "emailAddress":{
              "name":"Samantha Booth",
              "address":"samanthab@contoso.onmicrosoft.com"
          }
      }
    ],
    "mentions":[
      {
        "mentioned":{
          "name":"Dana Swope",
          "address":"danas@contoso.onmicrosoft.com"
         }
      }
    ]
  }
}
```

##### <a name="response-2"></a><span data-ttu-id="9678c-161">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="9678c-161">Response 2</span></span>
<span data-ttu-id="9678c-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9678c-162">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="9678c-163">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="9678c-163">Request 3</span></span>
<span data-ttu-id="9678c-164">Следующий пример создает сообщение с использованием настраиваемых заголовков сообщений Интернета и отправляет сообщение.</span><span class="sxs-lookup"><span data-stu-id="9678c-164">The next example creates a message with custom Internet message headers and sends the message.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_headers"
}-->
```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: application/json

{
  "message": {
    "subject": "9/9/2018: concert",
    "body": {
      "contentType": "HTML",
      "content": "The group represents Nevada."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "AlexW@contoso.OnMicrosoft.com"
        }
      }
    ],
    "internetMessageHeaders":[
      {
        "name":"x-custom-header-group-name",
        "value":"Nevada"
      },
      {
        "name":"x-custom-header-group-id",
        "value":"NV001"
      }
    ]
  }
}
```

##### <a name="response-3"></a><span data-ttu-id="9678c-165">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="9678c-165">Response 3</span></span>
<span data-ttu-id="9678c-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9678c-166">Here is an example of the response.</span></span>
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
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
