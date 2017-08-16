# <a name="message-replyall"></a><span data-ttu-id="aeace-101">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="aeace-101">message: replyAll</span></span>

<span data-ttu-id="aeace-p101">Ответ всем получателям сообщения. Затем сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="aeace-p101">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aeace-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="aeace-104">Prerequisites</span></span>
<span data-ttu-id="aeace-105">Для применения этого API требуется одна из указанных **областей**: *Mail.Send*</span><span class="sxs-lookup"><span data-stu-id="aeace-105">One of the following **scopes** is required to execute this API: *Mail.Send*</span></span>
## <a name="http-request"></a><span data-ttu-id="aeace-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aeace-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="aeace-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aeace-107">Request headers</span></span>
| <span data-ttu-id="aeace-108">Имя</span><span class="sxs-lookup"><span data-stu-id="aeace-108">Name</span></span>       | <span data-ttu-id="aeace-109">Тип</span><span class="sxs-lookup"><span data-stu-id="aeace-109">Type</span></span> | <span data-ttu-id="aeace-110">Описание</span><span class="sxs-lookup"><span data-stu-id="aeace-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aeace-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="aeace-111">Authorization</span></span>  | <span data-ttu-id="aeace-112">string</span><span class="sxs-lookup"><span data-stu-id="aeace-112">string</span></span>  | <span data-ttu-id="aeace-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aeace-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aeace-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aeace-115">Content-Type</span></span> | <span data-ttu-id="aeace-116">string</span><span class="sxs-lookup"><span data-stu-id="aeace-116">string</span></span>  | <span data-ttu-id="aeace-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aeace-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aeace-119">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aeace-119">Request body</span></span>
<span data-ttu-id="aeace-120">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="aeace-120">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aeace-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="aeace-121">Parameter</span></span>    | <span data-ttu-id="aeace-122">Тип</span><span class="sxs-lookup"><span data-stu-id="aeace-122">Type</span></span>   |<span data-ttu-id="aeace-123">Описание</span><span class="sxs-lookup"><span data-stu-id="aeace-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aeace-124">comment</span><span class="sxs-lookup"><span data-stu-id="aeace-124">comment</span></span>|<span data-ttu-id="aeace-125">String</span><span class="sxs-lookup"><span data-stu-id="aeace-125">String</span></span>|<span data-ttu-id="aeace-p104">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="aeace-p104">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="aeace-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="aeace-128">Response</span></span>

<span data-ttu-id="aeace-p105">В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="aeace-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aeace-131">Пример</span><span class="sxs-lookup"><span data-stu-id="aeace-131">Example</span></span>
<span data-ttu-id="aeace-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="aeace-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="aeace-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="aeace-133">Request</span></span>
<span data-ttu-id="aeace-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aeace-134">Here is an example of the request.</span></span>
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


##### <a name="response"></a><span data-ttu-id="aeace-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="aeace-135">Response</span></span>
<span data-ttu-id="aeace-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="aeace-136">Here is an example of the response.</span></span>
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
