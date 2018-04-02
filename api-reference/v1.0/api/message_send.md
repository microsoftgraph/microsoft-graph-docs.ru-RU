# <a name="message-send"></a><span data-ttu-id="47f45-101">message: send</span><span class="sxs-lookup"><span data-stu-id="47f45-101">message: send</span></span>

<span data-ttu-id="47f45-p101">Отправка сообщения из папки черновиков. Черновик сообщения может быть предназначен для нового сообщения, ответа, ответа всем пользователям или пересылки. Затем сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="47f45-p101">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="47f45-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47f45-105">Permissions</span></span>
<span data-ttu-id="47f45-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="47f45-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="47f45-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47f45-108">Permission type</span></span>      | <span data-ttu-id="47f45-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47f45-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47f45-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47f45-110">Delegated (work or school account)</span></span> | <span data-ttu-id="47f45-111">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="47f45-111">Mail.Send</span></span>    |
|<span data-ttu-id="47f45-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47f45-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47f45-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="47f45-113">Mail.Send</span></span>    |
|<span data-ttu-id="47f45-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47f45-114">Application</span></span> | <span data-ttu-id="47f45-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="47f45-115">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="47f45-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47f45-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```
## <a name="request-headers"></a><span data-ttu-id="47f45-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47f45-117">Request headers</span></span>
| <span data-ttu-id="47f45-118">Имя</span><span class="sxs-lookup"><span data-stu-id="47f45-118">Name</span></span>       | <span data-ttu-id="47f45-119">Тип</span><span class="sxs-lookup"><span data-stu-id="47f45-119">Type</span></span> | <span data-ttu-id="47f45-120">Описание</span><span class="sxs-lookup"><span data-stu-id="47f45-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="47f45-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="47f45-121">Authorization</span></span>  | <span data-ttu-id="47f45-122">string</span><span class="sxs-lookup"><span data-stu-id="47f45-122">string</span></span>  | <span data-ttu-id="47f45-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47f45-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47f45-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47f45-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="47f45-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="47f45-126">Response</span></span>

<span data-ttu-id="47f45-p104">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="47f45-p104">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47f45-129">Пример</span><span class="sxs-lookup"><span data-stu-id="47f45-129">Example</span></span>
<span data-ttu-id="47f45-130">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="47f45-130">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="47f45-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="47f45-131">Request</span></span>
<span data-ttu-id="47f45-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47f45-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="47f45-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="47f45-133">Response</span></span>

<span data-ttu-id="47f45-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="47f45-134">Here is an example of the response.</span></span>
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
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
