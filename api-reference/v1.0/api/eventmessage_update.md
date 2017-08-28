# <a name="update-eventmessage"></a><span data-ttu-id="4450c-101">Обновление объекта eventmessage</span><span class="sxs-lookup"><span data-stu-id="4450c-101">Update eventmessage</span></span>

<span data-ttu-id="4450c-102">Обновление свойств объекта eventmessage.</span><span class="sxs-lookup"><span data-stu-id="4450c-102">Update the properties of eventmessage object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4450c-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4450c-103">Permissions</span></span>
<span data-ttu-id="4450c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4450c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4450c-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4450c-106">Permission type</span></span>      | <span data-ttu-id="4450c-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4450c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4450c-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4450c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4450c-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4450c-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4450c-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4450c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4450c-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4450c-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4450c-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4450c-112">Application</span></span> | <span data-ttu-id="4450c-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4450c-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4450c-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4450c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4450c-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4450c-115">Request headers</span></span>
| <span data-ttu-id="4450c-116">Имя</span><span class="sxs-lookup"><span data-stu-id="4450c-116">Name</span></span>       | <span data-ttu-id="4450c-117">Тип</span><span class="sxs-lookup"><span data-stu-id="4450c-117">Type</span></span> | <span data-ttu-id="4450c-118">Описание</span><span class="sxs-lookup"><span data-stu-id="4450c-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4450c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4450c-119">Authorization</span></span>  | <span data-ttu-id="4450c-120">string</span><span class="sxs-lookup"><span data-stu-id="4450c-120">string</span></span>  | <span data-ttu-id="4450c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4450c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4450c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4450c-123">Content-Type</span></span> | <span data-ttu-id="4450c-124">string</span><span class="sxs-lookup"><span data-stu-id="4450c-124">string</span></span>  | <span data-ttu-id="4450c-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4450c-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="4450c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4450c-127">Request body</span></span>
<span data-ttu-id="4450c-p104">В основном тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, доступные для записи и обновления.</span><span class="sxs-lookup"><span data-stu-id="4450c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="4450c-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="4450c-132">Property</span></span>     | <span data-ttu-id="4450c-133">Тип</span><span class="sxs-lookup"><span data-stu-id="4450c-133">Type</span></span>   |<span data-ttu-id="4450c-134">Описание</span><span class="sxs-lookup"><span data-stu-id="4450c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4450c-135">categories</span><span class="sxs-lookup"><span data-stu-id="4450c-135">categories</span></span>|<span data-ttu-id="4450c-136">String</span><span class="sxs-lookup"><span data-stu-id="4450c-136">String</span></span>|<span data-ttu-id="4450c-137">Категории, связанные с сообщением.</span><span class="sxs-lookup"><span data-stu-id="4450c-137">The categories associated with the message.</span></span>|
|<span data-ttu-id="4450c-138">importance</span><span class="sxs-lookup"><span data-stu-id="4450c-138">importance</span></span>|<span data-ttu-id="4450c-139">String</span><span class="sxs-lookup"><span data-stu-id="4450c-139">String</span></span>|<span data-ttu-id="4450c-p105">Важность сообщения. Возможные значения: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="4450c-p105">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="4450c-142">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="4450c-142">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="4450c-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="4450c-143">Boolean</span></span>|<span data-ttu-id="4450c-144">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="4450c-144">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="4450c-145">isRead</span><span class="sxs-lookup"><span data-stu-id="4450c-145">isRead</span></span>|<span data-ttu-id="4450c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="4450c-146">Boolean</span></span>|<span data-ttu-id="4450c-147">Указывает, прочитано ли сообщение.</span><span class="sxs-lookup"><span data-stu-id="4450c-147">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="4450c-148">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="4450c-148">isReadReceiptRequested</span></span>|<span data-ttu-id="4450c-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="4450c-149">Boolean</span></span>|<span data-ttu-id="4450c-150">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="4450c-150">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="4450c-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="4450c-151">Response</span></span>

<span data-ttu-id="4450c-152">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [eventMessage](../resources/eventmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4450c-152">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4450c-153">Пример</span><span class="sxs-lookup"><span data-stu-id="4450c-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4450c-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="4450c-154">Request</span></span>
<span data-ttu-id="4450c-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4450c-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_eventmessage"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "isRead": "true",
}
```
##### <a name="response"></a><span data-ttu-id="4450c-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="4450c-156">Response</span></span>
<span data-ttu-id="4450c-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4450c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventmessage"
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
  "bodyPreview": "bodyPreview-value",
  "meetingMessageType": "meetingMessageType-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update eventmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
