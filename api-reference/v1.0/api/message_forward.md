# <a name="message-forward"></a><span data-ttu-id="33a4c-101">message: forward</span><span class="sxs-lookup"><span data-stu-id="33a4c-101">message: forward</span></span>

<span data-ttu-id="33a4c-p101">Пересылка сообщения. Сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="33a4c-p101">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33a4c-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="33a4c-104">Prerequisites</span></span>
<span data-ttu-id="33a4c-105">Для применения этого API требуется одна из указанных **областей**: *Mail.Send*</span><span class="sxs-lookup"><span data-stu-id="33a4c-105">One of the following **scopes** is required to execute this API: *Mail.Send*</span></span>
## <a name="http-request"></a><span data-ttu-id="33a4c-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33a4c-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="33a4c-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33a4c-107">Request headers</span></span>
| <span data-ttu-id="33a4c-108">Имя</span><span class="sxs-lookup"><span data-stu-id="33a4c-108">Name</span></span>       | <span data-ttu-id="33a4c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="33a4c-109">Type</span></span> | <span data-ttu-id="33a4c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="33a4c-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="33a4c-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="33a4c-111">Authorization</span></span>  | <span data-ttu-id="33a4c-112">string</span><span class="sxs-lookup"><span data-stu-id="33a4c-112">string</span></span>  | <span data-ttu-id="33a4c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33a4c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="33a4c-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="33a4c-115">Content-Type</span></span> | <span data-ttu-id="33a4c-116">string</span><span class="sxs-lookup"><span data-stu-id="33a4c-116">string</span></span>  | <span data-ttu-id="33a4c-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33a4c-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33a4c-119">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33a4c-119">Request body</span></span>
<span data-ttu-id="33a4c-120">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="33a4c-120">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="33a4c-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="33a4c-121">Parameter</span></span>    | <span data-ttu-id="33a4c-122">Тип</span><span class="sxs-lookup"><span data-stu-id="33a4c-122">Type</span></span>   |<span data-ttu-id="33a4c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="33a4c-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33a4c-124">comment</span><span class="sxs-lookup"><span data-stu-id="33a4c-124">comment</span></span>|<span data-ttu-id="33a4c-125">String</span><span class="sxs-lookup"><span data-stu-id="33a4c-125">String</span></span>|<span data-ttu-id="33a4c-p104">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="33a4c-p104">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="33a4c-128">toRecipients</span><span class="sxs-lookup"><span data-stu-id="33a4c-128">toRecipients</span></span>|<span data-ttu-id="33a4c-129">Коллекция объектов [Recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="33a4c-129">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="33a4c-130">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="33a4c-130">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="33a4c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="33a4c-131">Response</span></span>

<span data-ttu-id="33a4c-p105">В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="33a4c-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33a4c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="33a4c-134">Example</span></span>
<span data-ttu-id="33a4c-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="33a4c-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="33a4c-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="33a4c-136">Request</span></span>
<span data-ttu-id="33a4c-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33a4c-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
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

##### <a name="response"></a><span data-ttu-id="33a4c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="33a4c-138">Response</span></span>
##### <a name="response"></a><span data-ttu-id="33a4c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="33a4c-139">Response</span></span>
<span data-ttu-id="33a4c-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="33a4c-140">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
