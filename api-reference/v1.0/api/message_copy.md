# <a name="message-copy"></a><span data-ttu-id="1431f-101">message: copy</span><span class="sxs-lookup"><span data-stu-id="1431f-101">message: copy</span></span>

<span data-ttu-id="1431f-102">Копирование сообщения в папку.</span><span class="sxs-lookup"><span data-stu-id="1431f-102">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="1431f-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1431f-103">Permissions</span></span>
<span data-ttu-id="1431f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1431f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1431f-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1431f-106">Permission type</span></span>      | <span data-ttu-id="1431f-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1431f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1431f-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1431f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1431f-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1431f-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1431f-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1431f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1431f-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1431f-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1431f-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1431f-112">Application</span></span> | <span data-ttu-id="1431f-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1431f-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1431f-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1431f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```
## <a name="request-headers"></a><span data-ttu-id="1431f-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1431f-115">Request headers</span></span>
| <span data-ttu-id="1431f-116">Имя</span><span class="sxs-lookup"><span data-stu-id="1431f-116">Name</span></span>       | <span data-ttu-id="1431f-117">Тип</span><span class="sxs-lookup"><span data-stu-id="1431f-117">Type</span></span> | <span data-ttu-id="1431f-118">Описание</span><span class="sxs-lookup"><span data-stu-id="1431f-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1431f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1431f-119">Authorization</span></span>  | <span data-ttu-id="1431f-120">string</span><span class="sxs-lookup"><span data-stu-id="1431f-120">string</span></span>  | <span data-ttu-id="1431f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1431f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1431f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1431f-123">Content-Type</span></span> | <span data-ttu-id="1431f-124">string</span><span class="sxs-lookup"><span data-stu-id="1431f-124">string</span></span>  | <span data-ttu-id="1431f-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1431f-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1431f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1431f-127">Request body</span></span>
<span data-ttu-id="1431f-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1431f-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1431f-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="1431f-129">Parameter</span></span>    | <span data-ttu-id="1431f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1431f-130">Type</span></span>   |<span data-ttu-id="1431f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1431f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1431f-132">destinationId</span><span class="sxs-lookup"><span data-stu-id="1431f-132">destinationId</span></span>|<span data-ttu-id="1431f-133">String</span><span class="sxs-lookup"><span data-stu-id="1431f-133">String</span></span>|<span data-ttu-id="1431f-134">Идентификатор или известное имя целевой папки, такое как *Inbox*, *Drafts*, *SentItems* или *DeletedItems*.</span><span class="sxs-lookup"><span data-stu-id="1431f-134">The destination folder ID, or a well-known folder name such as *Inbox*, *Drafts*, *SentItems*, or *DeletedItems*.</span></span> <span data-ttu-id="1431f-135">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="1431f-135">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="1431f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="1431f-136">Response</span></span>

<span data-ttu-id="1431f-137">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1431f-137">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1431f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="1431f-138">Example</span></span>
<span data-ttu-id="1431f-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1431f-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1431f-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="1431f-140">Request</span></span>
<span data-ttu-id="1431f-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1431f-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="1431f-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="1431f-142">Response</span></span>
<span data-ttu-id="1431f-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1431f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
