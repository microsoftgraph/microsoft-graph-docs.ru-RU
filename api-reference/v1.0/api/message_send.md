# <a name="message-send"></a><span data-ttu-id="f9196-101">message: send</span><span class="sxs-lookup"><span data-stu-id="f9196-101">message: send</span></span>

<span data-ttu-id="f9196-p101">Отправка сообщения из папки черновиков. Черновик сообщения может быть предназначен для нового сообщения, ответа, ответа всем пользователям или пересылки. Затем сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="f9196-p101">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9196-105">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f9196-105">Prerequisites</span></span>
<span data-ttu-id="f9196-106">Для применения этого API требуется одна из указанных **областей**: *Mail.Send*</span><span class="sxs-lookup"><span data-stu-id="f9196-106">One of the following **scopes** is required to execute this API: *Mail.Send*</span></span>
## <a name="http-request"></a><span data-ttu-id="f9196-107">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9196-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```
## <a name="request-headers"></a><span data-ttu-id="f9196-108">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9196-108">Request headers</span></span>
| <span data-ttu-id="f9196-109">Имя</span><span class="sxs-lookup"><span data-stu-id="f9196-109">Name</span></span>       | <span data-ttu-id="f9196-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f9196-110">Type</span></span> | <span data-ttu-id="f9196-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f9196-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f9196-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9196-112">Authorization</span></span>  | <span data-ttu-id="f9196-113">string</span><span class="sxs-lookup"><span data-stu-id="f9196-113">string</span></span>  | <span data-ttu-id="f9196-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9196-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9196-116">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9196-116">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f9196-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9196-117">Response</span></span>

<span data-ttu-id="f9196-p103">В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f9196-p103">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9196-120">Пример</span><span class="sxs-lookup"><span data-stu-id="f9196-120">Example</span></span>
<span data-ttu-id="f9196-121">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f9196-121">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f9196-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9196-122">Request</span></span>
<span data-ttu-id="f9196-123">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9196-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="f9196-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9196-124">Response</span></span>
##### <a name="response"></a><span data-ttu-id="f9196-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9196-125">Response</span></span>
<span data-ttu-id="f9196-126">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f9196-126">Here is an example of the response.</span></span>
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
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
