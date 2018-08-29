# <a name="send-mail"></a><span data-ttu-id="12a32-101">Отправка почты</span><span class="sxs-lookup"><span data-stu-id="12a32-101">Send mail</span></span>

<span data-ttu-id="12a32-p101">Отправка сообщения, указанного в теле запроса. Сообщение сохраняется в папке "Отправленные" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="12a32-p101">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="12a32-104">Вы можете включить [вложенный файл](../resources/fileattachment.md) при вызове действия **sendMail**.</span><span class="sxs-lookup"><span data-stu-id="12a32-104">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="permissions"></a><span data-ttu-id="12a32-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12a32-105">Permissions</span></span>
<span data-ttu-id="12a32-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="12a32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="12a32-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12a32-108">Permission type</span></span>      | <span data-ttu-id="12a32-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12a32-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12a32-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12a32-110">Delegated (work or school account)</span></span> | <span data-ttu-id="12a32-111">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="12a32-111">Mail.Send</span></span>    |
|<span data-ttu-id="12a32-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12a32-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12a32-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="12a32-113">Mail.Send</span></span>    |
|<span data-ttu-id="12a32-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12a32-114">Application</span></span> | <span data-ttu-id="12a32-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="12a32-115">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="12a32-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12a32-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="12a32-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12a32-117">Request headers</span></span>
| <span data-ttu-id="12a32-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12a32-118">Header</span></span>       | <span data-ttu-id="12a32-119">Значение</span><span class="sxs-lookup"><span data-stu-id="12a32-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="12a32-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12a32-120">Authorization</span></span>  | <span data-ttu-id="12a32-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12a32-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="12a32-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12a32-123">Content-Type</span></span>  | <span data-ttu-id="12a32-124">application/json</span><span class="sxs-lookup"><span data-stu-id="12a32-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="12a32-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12a32-125">Request body</span></span>
<span data-ttu-id="12a32-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="12a32-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="12a32-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="12a32-127">Parameter</span></span>    | <span data-ttu-id="12a32-128">Тип</span><span class="sxs-lookup"><span data-stu-id="12a32-128">Type</span></span>   |<span data-ttu-id="12a32-129">Описание</span><span class="sxs-lookup"><span data-stu-id="12a32-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12a32-130">message</span><span class="sxs-lookup"><span data-stu-id="12a32-130">message</span></span>|[<span data-ttu-id="12a32-131">Message</span><span class="sxs-lookup"><span data-stu-id="12a32-131">Message</span></span>](../resources/message.md)|<span data-ttu-id="12a32-p104">Отправляемое сообщение. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12a32-p104">The message to send. Required.</span></span>|
|<span data-ttu-id="12a32-134">saveToSentItems</span><span class="sxs-lookup"><span data-stu-id="12a32-134">SaveToSentItems</span></span>|<span data-ttu-id="12a32-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="12a32-135">Boolean</span></span>|<span data-ttu-id="12a32-p105">Указывает, нужно ли сохранять сообщение в папке "Отправленные". Указывайте этот параметр, если задано значение false (по умолчанию используется true).  Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="12a32-p105">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="12a32-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="12a32-139">Response</span></span>

<span data-ttu-id="12a32-p106">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="12a32-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12a32-142">Пример</span><span class="sxs-lookup"><span data-stu-id="12a32-142">Example</span></span>
<span data-ttu-id="12a32-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="12a32-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="12a32-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="12a32-144">Request</span></span>
<span data-ttu-id="12a32-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12a32-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
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

##### <a name="response"></a><span data-ttu-id="12a32-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="12a32-146">Response</span></span>
<span data-ttu-id="12a32-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="12a32-147">Here is an example of the response.</span></span>
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
