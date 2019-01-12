---
title: Отправка почты
description: Отправка сообщения, указанного в теле запроса. Сообщение сохраняется в папке "Отправленные" по умолчанию.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 542c36f4d52c461b5a423d9a7fb93a06b94b9b70
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975808"
---
# <a name="send-mail"></a><span data-ttu-id="b89e3-104">Отправка почты</span><span class="sxs-lookup"><span data-stu-id="b89e3-104">Send mail</span></span>

<span data-ttu-id="b89e3-p102">Отправка сообщения, указанного в теле запроса. Сообщение сохраняется в папке "Отправленные" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b89e3-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="b89e3-107">Вы можете включить [вложенный файл](../resources/fileattachment.md) при вызове действия **sendMail**.</span><span class="sxs-lookup"><span data-stu-id="b89e3-107">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="permissions"></a><span data-ttu-id="b89e3-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b89e3-108">Permissions</span></span>
<span data-ttu-id="b89e3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b89e3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b89e3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b89e3-111">Permission type</span></span>      | <span data-ttu-id="b89e3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b89e3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b89e3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b89e3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b89e3-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b89e3-114">Mail.Send</span></span>    |
|<span data-ttu-id="b89e3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b89e3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b89e3-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b89e3-116">Mail.Send</span></span>    |
|<span data-ttu-id="b89e3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b89e3-117">Application</span></span> | <span data-ttu-id="b89e3-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b89e3-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="b89e3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b89e3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="b89e3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b89e3-120">Request headers</span></span>
| <span data-ttu-id="b89e3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b89e3-121">Header</span></span>       | <span data-ttu-id="b89e3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b89e3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b89e3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b89e3-123">Authorization</span></span>  | <span data-ttu-id="b89e3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b89e3-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b89e3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b89e3-126">Content-Type</span></span>  | <span data-ttu-id="b89e3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b89e3-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b89e3-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b89e3-128">Request body</span></span>
<span data-ttu-id="b89e3-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b89e3-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b89e3-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="b89e3-130">Parameter</span></span>    | <span data-ttu-id="b89e3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b89e3-131">Type</span></span>   |<span data-ttu-id="b89e3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b89e3-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b89e3-133">message</span><span class="sxs-lookup"><span data-stu-id="b89e3-133">message</span></span>|[<span data-ttu-id="b89e3-134">Message</span><span class="sxs-lookup"><span data-stu-id="b89e3-134">Message</span></span>](../resources/message.md)|<span data-ttu-id="b89e3-p105">Отправляемое сообщение. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b89e3-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="b89e3-137">saveToSentItems</span><span class="sxs-lookup"><span data-stu-id="b89e3-137">saveToSentItems</span></span>|<span data-ttu-id="b89e3-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="b89e3-138">Boolean</span></span>|<span data-ttu-id="b89e3-p106">Указывает, нужно ли сохранять сообщение в папке "Отправленные". Указывайте этот параметр, если задано значение false (по умолчанию используется true).  Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b89e3-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b89e3-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b89e3-142">Response</span></span>

<span data-ttu-id="b89e3-p107">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b89e3-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b89e3-145">Пример</span><span class="sxs-lookup"><span data-stu-id="b89e3-145">Example</span></span>
<span data-ttu-id="b89e3-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b89e3-146">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="b89e3-147">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="b89e3-147">Request 1</span></span>
<span data-ttu-id="b89e3-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b89e3-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: application/json

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
          "address": "fannyd@contoso.onmicrosoft.com"
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

##### <a name="response-1"></a><span data-ttu-id="b89e3-149">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="b89e3-149">Response 1</span></span>
<span data-ttu-id="b89e3-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b89e3-150">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-2"></a><span data-ttu-id="b89e3-151">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="b89e3-151">Request 2</span></span>
<span data-ttu-id="b89e3-152">Следующий пример создает сообщение с использованием настраиваемых заголовков сообщений Интернета и отправляет сообщение.</span><span class="sxs-lookup"><span data-stu-id="b89e3-152">The next example creates a message with custom Internet message headers and sends the message.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_headers"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
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

##### <a name="response-2"></a><span data-ttu-id="b89e3-153">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="b89e3-153">Response 2</span></span>
<span data-ttu-id="b89e3-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b89e3-154">Here is an example of the response.</span></span>
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
