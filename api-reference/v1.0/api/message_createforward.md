# <a name="message-createforward"></a><span data-ttu-id="71b2e-101">message: createForward</span><span class="sxs-lookup"><span data-stu-id="71b2e-101">message: createForward</span></span>

<span data-ttu-id="71b2e-102">Создание черновика для пересылки указанного ресурса [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="71b2e-102">Create a draft to forward the specified [message](../resources/message.md).</span></span> <span data-ttu-id="71b2e-103">После этого можно [обновить](../api/message_update.md) черновик, чтобы добавить содержимое в **текст** или изменить другие свойства сообщения, либо просто [отправить](../api/message_send.md) черновик.</span><span class="sxs-lookup"><span data-stu-id="71b2e-103">You can then [update](../api/message_update.md) the draft to add content to the **body** or change other message properties, or, simply [send](../api/message_send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="71b2e-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71b2e-104">Permissions</span></span>
<span data-ttu-id="71b2e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="71b2e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="71b2e-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71b2e-107">Permission type</span></span>      | <span data-ttu-id="71b2e-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71b2e-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71b2e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71b2e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="71b2e-110">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71b2e-110">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="71b2e-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71b2e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71b2e-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71b2e-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="71b2e-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71b2e-113">Application</span></span> | <span data-ttu-id="71b2e-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71b2e-114">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="71b2e-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71b2e-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="71b2e-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71b2e-116">Request headers</span></span>
| <span data-ttu-id="71b2e-117">Имя</span><span class="sxs-lookup"><span data-stu-id="71b2e-117">Name</span></span>       | <span data-ttu-id="71b2e-118">Тип</span><span class="sxs-lookup"><span data-stu-id="71b2e-118">Type</span></span> | <span data-ttu-id="71b2e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="71b2e-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="71b2e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="71b2e-120">Authorization</span></span>  | <span data-ttu-id="71b2e-121">string</span><span class="sxs-lookup"><span data-stu-id="71b2e-121">string</span></span>  | <span data-ttu-id="71b2e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71b2e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71b2e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71b2e-124">Request body</span></span>
<span data-ttu-id="71b2e-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71b2e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71b2e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="71b2e-126">Response</span></span>

<span data-ttu-id="71b2e-127">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71b2e-127">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71b2e-128">Пример</span><span class="sxs-lookup"><span data-stu-id="71b2e-128">Example</span></span>
<span data-ttu-id="71b2e-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="71b2e-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="71b2e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="71b2e-130">Request</span></span>
<span data-ttu-id="71b2e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71b2e-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createForward
```

##### <a name="response"></a><span data-ttu-id="71b2e-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="71b2e-132">Response</span></span>
<span data-ttu-id="71b2e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="71b2e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
