# <a name="message-createreply"></a><span data-ttu-id="1aaba-101">message: createReply</span><span class="sxs-lookup"><span data-stu-id="1aaba-101">message: createReply</span></span>

<span data-ttu-id="1aaba-102">Создание черновика ответа на указанное [сообщение](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="1aaba-102">Create a draft of the reply to the specified [message](../resources/message.md).</span></span> <span data-ttu-id="1aaba-103">После этого можно [обновить](../api/message_update.md) черновик, чтобы добавить содержимое ответа в **текст** или изменить другие свойства сообщения, либо просто [отправить](../api/message_send.md) черновик.</span><span class="sxs-lookup"><span data-stu-id="1aaba-103">You can then [update](../api/message_update.md) the draft to add reply content to the **body** or change other message properties, or, simply [send](../api/message_send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="1aaba-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1aaba-104">Permissions</span></span>
<span data-ttu-id="1aaba-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1aaba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1aaba-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1aaba-107">Permission type</span></span>      | <span data-ttu-id="1aaba-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1aaba-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1aaba-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1aaba-109">Delegated (work or school account)</span></span> | <span data-ttu-id="1aaba-110">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1aaba-110">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1aaba-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1aaba-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1aaba-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1aaba-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1aaba-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1aaba-113">Application</span></span> | <span data-ttu-id="1aaba-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1aaba-114">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1aaba-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1aaba-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="1aaba-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1aaba-116">Request headers</span></span>
| <span data-ttu-id="1aaba-117">Имя</span><span class="sxs-lookup"><span data-stu-id="1aaba-117">Name</span></span>       | <span data-ttu-id="1aaba-118">Тип</span><span class="sxs-lookup"><span data-stu-id="1aaba-118">Type</span></span> | <span data-ttu-id="1aaba-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1aaba-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1aaba-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1aaba-120">Authorization</span></span>  | <span data-ttu-id="1aaba-121">string</span><span class="sxs-lookup"><span data-stu-id="1aaba-121">string</span></span>  | <span data-ttu-id="1aaba-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1aaba-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1aaba-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1aaba-124">Request body</span></span>
<span data-ttu-id="1aaba-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1aaba-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1aaba-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1aaba-126">Response</span></span>

<span data-ttu-id="1aaba-127">В случае успеха этот метод возвращает код отклика `201, Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1aaba-127">If successful, this method returns `201, Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1aaba-128">Пример</span><span class="sxs-lookup"><span data-stu-id="1aaba-128">Example</span></span>
<span data-ttu-id="1aaba-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1aaba-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1aaba-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1aaba-130">Request</span></span>
<span data-ttu-id="1aaba-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1aaba-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReply
```

##### <a name="response"></a><span data-ttu-id="1aaba-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="1aaba-132">Response</span></span>
<span data-ttu-id="1aaba-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1aaba-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
