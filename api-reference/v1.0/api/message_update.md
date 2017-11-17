# <a name="update-message"></a><span data-ttu-id="dad34-101">Обновление сообщения</span><span class="sxs-lookup"><span data-stu-id="dad34-101">Update message</span></span>

<span data-ttu-id="dad34-102">Обновление свойств объекта сообщения.</span><span class="sxs-lookup"><span data-stu-id="dad34-102">Update the properties of message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dad34-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dad34-103">Permissions</span></span>
<span data-ttu-id="dad34-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dad34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dad34-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dad34-106">Permission type</span></span>      | <span data-ttu-id="dad34-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dad34-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dad34-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dad34-108">Delegated (work or school account)</span></span> | <span data-ttu-id="dad34-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dad34-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dad34-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dad34-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dad34-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dad34-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dad34-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dad34-112">Application</span></span> | <span data-ttu-id="dad34-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dad34-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dad34-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dad34-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="dad34-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dad34-115">Request headers</span></span>
| <span data-ttu-id="dad34-116">Имя</span><span class="sxs-lookup"><span data-stu-id="dad34-116">Name</span></span>       | <span data-ttu-id="dad34-117">Тип</span><span class="sxs-lookup"><span data-stu-id="dad34-117">Type</span></span> | <span data-ttu-id="dad34-118">Описание</span><span class="sxs-lookup"><span data-stu-id="dad34-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dad34-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="dad34-119">Authorization</span></span>  | <span data-ttu-id="dad34-120">string</span><span class="sxs-lookup"><span data-stu-id="dad34-120">string</span></span>  | <span data-ttu-id="dad34-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dad34-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dad34-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dad34-123">Content-Type</span></span> | <span data-ttu-id="dad34-124">string</span><span class="sxs-lookup"><span data-stu-id="dad34-124">string</span></span>  | <span data-ttu-id="dad34-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dad34-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="dad34-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dad34-127">Request body</span></span>
<span data-ttu-id="dad34-p104">В основном тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, доступные для записи и обновления.</span><span class="sxs-lookup"><span data-stu-id="dad34-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="dad34-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="dad34-132">Property</span></span>     | <span data-ttu-id="dad34-133">Тип</span><span class="sxs-lookup"><span data-stu-id="dad34-133">Type</span></span>   |<span data-ttu-id="dad34-134">Описание</span><span class="sxs-lookup"><span data-stu-id="dad34-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dad34-135">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="dad34-135">bccRecipients</span></span>|<span data-ttu-id="dad34-136">Область записи</span><span class="sxs-lookup"><span data-stu-id="dad34-136">Recipient</span></span>|<span data-ttu-id="dad34-p105">Получатели скрытой копии сообщения. Это свойство можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="dad34-p105">The Bcc recipients for the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="dad34-139">categories</span><span class="sxs-lookup"><span data-stu-id="dad34-139">categories</span></span>|<span data-ttu-id="dad34-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dad34-140">String collection</span></span>|<span data-ttu-id="dad34-141">Категории, сопоставленные с сообщением.</span><span class="sxs-lookup"><span data-stu-id="dad34-141">The categories associated with the message.</span></span>|
|<span data-ttu-id="dad34-142">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="dad34-142">ccRecipients</span></span>|<span data-ttu-id="dad34-143">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="dad34-143">Recipient collection</span></span>|<span data-ttu-id="dad34-p106">Получатели копии сообщения. Это свойство можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="dad34-p106">The Cc recipients for the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="dad34-146">from</span><span class="sxs-lookup"><span data-stu-id="dad34-146">from</span></span>|<span data-ttu-id="dad34-147">Область записи</span><span class="sxs-lookup"><span data-stu-id="dad34-147">Recipient</span></span>|<span data-ttu-id="dad34-p107">Владелец почтового ящика и отправитель сообщения. Это свойство можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="dad34-p107">The mailbox owner and sender of the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="dad34-150">importance</span><span class="sxs-lookup"><span data-stu-id="dad34-150">importance</span></span>|<span data-ttu-id="dad34-151">String</span><span class="sxs-lookup"><span data-stu-id="dad34-151">String</span></span>|<span data-ttu-id="dad34-p108">Важность сообщения. Возможные значения: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="dad34-p108">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="dad34-154">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="dad34-154">inferenceClassification</span></span> | <span data-ttu-id="dad34-155">String</span><span class="sxs-lookup"><span data-stu-id="dad34-155">String</span></span> | <span data-ttu-id="dad34-p109">Классификация сообщения для пользователя на основании подразумеваемой релевантности или важности либо явного переопределения. Возможные значения: `focused` или `other`.</span><span class="sxs-lookup"><span data-stu-id="dad34-p109">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="dad34-158">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="dad34-158">internetMessageId</span></span> |<span data-ttu-id="dad34-159">Строка</span><span class="sxs-lookup"><span data-stu-id="dad34-159">String</span></span> |<span data-ttu-id="dad34-p110">Идентификатор сообщения в формате, определенном в документе [RFC2822](http://www.ietf.org/rfc/rfc2822.txt). Это свойство можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="dad34-p110">The message ID in the format specified by [RFC2822](http://www.ietf.org/rfc/rfc2822.txt). Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="dad34-162">isRead</span><span class="sxs-lookup"><span data-stu-id="dad34-162">isRead</span></span>|<span data-ttu-id="dad34-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="dad34-163">Boolean</span></span>|<span data-ttu-id="dad34-164">Указывает, прочитано ли сообщение.</span><span class="sxs-lookup"><span data-stu-id="dad34-164">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="dad34-165">replyTo</span><span class="sxs-lookup"><span data-stu-id="dad34-165">replyTo</span></span>|<span data-ttu-id="dad34-166">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="dad34-166">Recipient collection</span></span>|<span data-ttu-id="dad34-p111">Электронные адреса, которые необходимо использовать при ответе. Это свойство можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="dad34-p111">The email addresses to use when replying. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="dad34-169">sender</span><span class="sxs-lookup"><span data-stu-id="dad34-169">sender</span></span>|<span data-ttu-id="dad34-170">Область записи</span><span class="sxs-lookup"><span data-stu-id="dad34-170">Recipient</span></span>|<span data-ttu-id="dad34-p112">Учетная запись, которая фактически используется для создания сообщения. Это свойство можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="dad34-p112">The account that is actually used to generate the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="dad34-173">toRecipients</span><span class="sxs-lookup"><span data-stu-id="dad34-173">toRecipients</span></span>|<span data-ttu-id="dad34-174">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="dad34-174">Recipient collection</span></span>|<span data-ttu-id="dad34-p113">Получатели сообщения, указанные в поле "Кому". Это свойство можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="dad34-p113">The To recipients for the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="dad34-177">Основной текст</span><span class="sxs-lookup"><span data-stu-id="dad34-177">body</span></span>|<span data-ttu-id="dad34-178">ItemBody</span><span class="sxs-lookup"><span data-stu-id="dad34-178">ItemBody</span></span>|<span data-ttu-id="dad34-p114">Текст сообщения. Это свойство можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="dad34-p114">The body of the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="dad34-181">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="dad34-181">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="dad34-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="dad34-182">Boolean</span></span>|<span data-ttu-id="dad34-183">Указывает, необходимо ли запрашивать уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="dad34-183">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="dad34-184">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="dad34-184">isReadReceiptRequested</span></span>|<span data-ttu-id="dad34-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="dad34-185">Boolean</span></span>|<span data-ttu-id="dad34-186">Указывает, необходимо ли запрашивать уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="dad34-186">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="dad34-187">subject</span><span class="sxs-lookup"><span data-stu-id="dad34-187">subject</span></span>|<span data-ttu-id="dad34-188">String</span><span class="sxs-lookup"><span data-stu-id="dad34-188">String</span></span>|<span data-ttu-id="dad34-p115">Тема сообщения. Это свойство можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="dad34-p115">The subject of the message. Updatable only if IsDraft = true.</span></span>|

<span data-ttu-id="dad34-191">Так как ресурс **message** поддерживает [расширения](../../../concepts/extensibility_overview.md), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="dad34-191">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="dad34-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="dad34-192">Response</span></span>

<span data-ttu-id="dad34-193">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dad34-193">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dad34-194">Пример</span><span class="sxs-lookup"><span data-stu-id="dad34-194">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dad34-195">Запрос</span><span class="sxs-lookup"><span data-stu-id="dad34-195">Request</span></span>
<span data-ttu-id="dad34-196">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dad34-196">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "inferenceClassification": "other"
}
```
##### <a name="response"></a><span data-ttu-id="dad34-197">Ответ</span><span class="sxs-lookup"><span data-stu-id="dad34-197">Response</span></span>
<span data-ttu-id="dad34-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dad34-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "bodyPreview": "bodyPreview-value",
  "inferenceClassification": "other"
}
```

## <a name="see-also"></a><span data-ttu-id="dad34-201">См. также</span><span class="sxs-lookup"><span data-stu-id="dad34-201">See also</span></span>

- [<span data-ttu-id="dad34-202">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="dad34-202">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="dad34-203">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="dad34-203">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
