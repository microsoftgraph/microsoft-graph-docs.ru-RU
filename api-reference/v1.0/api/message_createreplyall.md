# <a name="message-createreplyall"></a><span data-ttu-id="51e48-101">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="51e48-101">message: createReplyAll</span></span>

<span data-ttu-id="51e48-p101">Создание черновика сообщения ответа всем пользователям. После этого вы сможете [обновить](../api/message_update.md) или [отправить](../api/message_send.md) черновик.</span><span class="sxs-lookup"><span data-stu-id="51e48-p101">Create a draft of the Reply All message. You can then [update](../api/message_update.md) or [send](../api/message_send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="51e48-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51e48-104">Permissions</span></span>
<span data-ttu-id="51e48-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="51e48-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="51e48-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51e48-107">Permission type</span></span>      | <span data-ttu-id="51e48-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51e48-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="51e48-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51e48-109">Delegated (work or school account)</span></span> | <span data-ttu-id="51e48-110">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51e48-110">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="51e48-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51e48-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51e48-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51e48-112">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="51e48-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51e48-113">Application</span></span> | <span data-ttu-id="51e48-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51e48-114">Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="51e48-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51e48-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="51e48-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51e48-116">Request headers</span></span>
| <span data-ttu-id="51e48-117">Имя</span><span class="sxs-lookup"><span data-stu-id="51e48-117">Name</span></span>       | <span data-ttu-id="51e48-118">Тип</span><span class="sxs-lookup"><span data-stu-id="51e48-118">Type</span></span> | <span data-ttu-id="51e48-119">Описание</span><span class="sxs-lookup"><span data-stu-id="51e48-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="51e48-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="51e48-120">Authorization</span></span>  | <span data-ttu-id="51e48-121">string</span><span class="sxs-lookup"><span data-stu-id="51e48-121">string</span></span>  | <span data-ttu-id="51e48-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51e48-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="51e48-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51e48-124">Content-Type</span></span> | <span data-ttu-id="51e48-125">string</span><span class="sxs-lookup"><span data-stu-id="51e48-125">string</span></span>  | <span data-ttu-id="51e48-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51e48-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51e48-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51e48-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="51e48-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="51e48-129">Response</span></span>

<span data-ttu-id="51e48-130">В случае успеха этот метод возвращает код отклика `201, Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51e48-130">If successful, this method returns `201, Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51e48-131">Пример</span><span class="sxs-lookup"><span data-stu-id="51e48-131">Example</span></span>
<span data-ttu-id="51e48-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="51e48-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="51e48-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="51e48-133">Request</span></span>
<span data-ttu-id="51e48-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51e48-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReplyAll
Content-type: application/json
Content-length: 248

{
  "comment": "comment-value"
}
```

##### <a name="response"></a><span data-ttu-id="51e48-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="51e48-135">Response</span></span>
<span data-ttu-id="51e48-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="51e48-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
