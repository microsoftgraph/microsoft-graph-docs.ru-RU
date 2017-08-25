# <a name="message-copy"></a><span data-ttu-id="a854a-101">message: copy</span><span class="sxs-lookup"><span data-stu-id="a854a-101">message: copy</span></span>

<span data-ttu-id="a854a-102">Копирование сообщения в папку.</span><span class="sxs-lookup"><span data-stu-id="a854a-102">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="a854a-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a854a-103">Permissions</span></span>
<span data-ttu-id="a854a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a854a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a854a-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a854a-106">Permission type</span></span>      | <span data-ttu-id="a854a-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a854a-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="a854a-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a854a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a854a-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a854a-109">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="a854a-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a854a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a854a-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a854a-111">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="a854a-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a854a-112">Application</span></span> | <span data-ttu-id="a854a-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a854a-113">Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a854a-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a854a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```
## <a name="request-headers"></a><span data-ttu-id="a854a-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a854a-115">Request headers</span></span>
| <span data-ttu-id="a854a-116">Имя</span><span class="sxs-lookup"><span data-stu-id="a854a-116">Name</span></span>       | <span data-ttu-id="a854a-117">Тип</span><span class="sxs-lookup"><span data-stu-id="a854a-117">Type</span></span> | <span data-ttu-id="a854a-118">Описание</span><span class="sxs-lookup"><span data-stu-id="a854a-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a854a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a854a-119">Authorization</span></span>  | <span data-ttu-id="a854a-120">string</span><span class="sxs-lookup"><span data-stu-id="a854a-120">string</span></span>  | <span data-ttu-id="a854a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a854a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a854a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a854a-123">Content-Type</span></span> | <span data-ttu-id="a854a-124">string</span><span class="sxs-lookup"><span data-stu-id="a854a-124">string</span></span>  | <span data-ttu-id="a854a-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a854a-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a854a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a854a-127">Request body</span></span>
<span data-ttu-id="a854a-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a854a-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a854a-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="a854a-129">Parameter</span></span>    | <span data-ttu-id="a854a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a854a-130">Type</span></span>   |<span data-ttu-id="a854a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a854a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a854a-132">destinationId</span><span class="sxs-lookup"><span data-stu-id="a854a-132">destinationId</span></span>|<span data-ttu-id="a854a-133">String</span><span class="sxs-lookup"><span data-stu-id="a854a-133">String</span></span>|<span data-ttu-id="a854a-134">Идентификатор целевой папки либо имя известной папки `Inbox`, `Drafts`, `SentItems` или `DeletedItems`.</span><span class="sxs-lookup"><span data-stu-id="a854a-134">The destination folder ID, or the `Inbox`, `Drafts`, `SentItems`, or `DeletedItems` well-known folder name.</span></span>|

## <a name="response"></a><span data-ttu-id="a854a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a854a-135">Response</span></span>

<span data-ttu-id="a854a-136">В случае успеха этот метод возвращает код отклика `201, Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a854a-136">If successful, this method returns `201, Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a854a-137">Пример</span><span class="sxs-lookup"><span data-stu-id="a854a-137">Example</span></span>
<span data-ttu-id="a854a-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a854a-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a854a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a854a-139">Request</span></span>
<span data-ttu-id="a854a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a854a-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="a854a-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="a854a-141">Response</span></span>
<span data-ttu-id="a854a-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a854a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
