# <a name="update-message"></a><span data-ttu-id="e5300-101">Обновление сообщения</span><span class="sxs-lookup"><span data-stu-id="e5300-101">Update message</span></span>

<span data-ttu-id="e5300-102">Обновление свойств объекта сообщения.</span><span class="sxs-lookup"><span data-stu-id="e5300-102">Update the properties of message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e5300-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5300-103">Permissions</span></span>
<span data-ttu-id="e5300-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e5300-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e5300-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5300-106">Permission type</span></span>      | <span data-ttu-id="e5300-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5300-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5300-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5300-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e5300-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5300-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e5300-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5300-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5300-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5300-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e5300-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5300-112">Application</span></span> | <span data-ttu-id="e5300-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5300-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5300-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5300-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e5300-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5300-115">Request headers</span></span>
| <span data-ttu-id="e5300-116">Имя</span><span class="sxs-lookup"><span data-stu-id="e5300-116">Name</span></span>       | <span data-ttu-id="e5300-117">Тип</span><span class="sxs-lookup"><span data-stu-id="e5300-117">Type</span></span> | <span data-ttu-id="e5300-118">Описание</span><span class="sxs-lookup"><span data-stu-id="e5300-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e5300-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5300-119">Authorization</span></span>  | <span data-ttu-id="e5300-120">string</span><span class="sxs-lookup"><span data-stu-id="e5300-120">string</span></span>  | <span data-ttu-id="e5300-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5300-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e5300-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e5300-123">Content-Type</span></span> | <span data-ttu-id="e5300-124">string</span><span class="sxs-lookup"><span data-stu-id="e5300-124">string</span></span>  | <span data-ttu-id="e5300-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5300-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="e5300-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5300-127">Request body</span></span>
<span data-ttu-id="e5300-p104">В основном тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, доступные для записи и обновления.</span><span class="sxs-lookup"><span data-stu-id="e5300-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="e5300-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5300-132">Property</span></span>     | <span data-ttu-id="e5300-133">Тип</span><span class="sxs-lookup"><span data-stu-id="e5300-133">Type</span></span>   |<span data-ttu-id="e5300-134">Описание</span><span class="sxs-lookup"><span data-stu-id="e5300-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5300-135">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="e5300-135">bccRecipients</span></span>|<span data-ttu-id="e5300-136">Recipient</span><span class="sxs-lookup"><span data-stu-id="e5300-136">Recipient</span></span>|<span data-ttu-id="e5300-137">Получателей скрытой копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="e5300-137">The Bcc recipients for the message.</span></span> <span data-ttu-id="e5300-138">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="e5300-138">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="e5300-139">categories</span><span class="sxs-lookup"><span data-stu-id="e5300-139">categories</span></span>|<span data-ttu-id="e5300-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e5300-140">String collection</span></span>|<span data-ttu-id="e5300-141">Категории, сопоставленные с сообщением.</span><span class="sxs-lookup"><span data-stu-id="e5300-141">The categories associated with the message.</span></span>|
|<span data-ttu-id="e5300-142">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="e5300-142">ccRecipients</span></span>|<span data-ttu-id="e5300-143">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="e5300-143">Recipient collection</span></span>|<span data-ttu-id="e5300-144">Получателей копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="e5300-144">The Cc recipients for the message.</span></span> <span data-ttu-id="e5300-145">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="e5300-145">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="e5300-146">from</span><span class="sxs-lookup"><span data-stu-id="e5300-146">from</span></span>|<span data-ttu-id="e5300-147">Recipient</span><span class="sxs-lookup"><span data-stu-id="e5300-147">Recipient</span></span>|<span data-ttu-id="e5300-148">Владелец почтового ящика и отправитель сообщения.</span><span class="sxs-lookup"><span data-stu-id="e5300-148">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="e5300-149">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="e5300-149">Updatable only if isDraft = true.</span></span> <span data-ttu-id="e5300-150">Должно соответствовать фактический почтового ящика, используемого.</span><span class="sxs-lookup"><span data-stu-id="e5300-150">Must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="e5300-151">importance</span><span class="sxs-lookup"><span data-stu-id="e5300-151">importance</span></span>|<span data-ttu-id="e5300-152">String</span><span class="sxs-lookup"><span data-stu-id="e5300-152">String</span></span>|<span data-ttu-id="e5300-153">Важность сообщения.</span><span class="sxs-lookup"><span data-stu-id="e5300-153">The importance of the message.</span></span> <span data-ttu-id="e5300-154">Возможные значения: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="e5300-154">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="e5300-155">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="e5300-155">inferenceClassification</span></span> | <span data-ttu-id="e5300-156">String</span><span class="sxs-lookup"><span data-stu-id="e5300-156">String</span></span> | <span data-ttu-id="e5300-157">Классификация сообщений для пользователя, на основе предполагаемых релевантность или важность, или явное переопределение.</span><span class="sxs-lookup"><span data-stu-id="e5300-157">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override.</span></span> <span data-ttu-id="e5300-158">Возможные значения: `focused` или `other`.</span><span class="sxs-lookup"><span data-stu-id="e5300-158">The possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="e5300-159">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="e5300-159">internetMessageId</span></span> |<span data-ttu-id="e5300-160">String</span><span class="sxs-lookup"><span data-stu-id="e5300-160">String</span></span> |<span data-ttu-id="e5300-161">Идентификатор сообщения в формате, установленном документом [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span><span class="sxs-lookup"><span data-stu-id="e5300-161">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="e5300-162">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="e5300-162">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="e5300-163">isRead</span><span class="sxs-lookup"><span data-stu-id="e5300-163">isRead</span></span>|<span data-ttu-id="e5300-164">Логический</span><span class="sxs-lookup"><span data-stu-id="e5300-164">Boolean</span></span>|<span data-ttu-id="e5300-165">Указывает, прочитано ли сообщение.</span><span class="sxs-lookup"><span data-stu-id="e5300-165">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="e5300-166">replyTo</span><span class="sxs-lookup"><span data-stu-id="e5300-166">replyTo</span></span>|<span data-ttu-id="e5300-167">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="e5300-167">Recipient collection</span></span>|<span data-ttu-id="e5300-168">Электронные адреса, которые необходимо использовать при ответе.</span><span class="sxs-lookup"><span data-stu-id="e5300-168">The email addresses to use when replying.</span></span> <span data-ttu-id="e5300-169">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="e5300-169">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="e5300-170">sender</span><span class="sxs-lookup"><span data-stu-id="e5300-170">sender</span></span>|<span data-ttu-id="e5300-171">Recipient</span><span class="sxs-lookup"><span data-stu-id="e5300-171">Recipient</span></span>|<span data-ttu-id="e5300-172">Учетная запись, которая фактически используется для создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="e5300-172">The account that is actually used to generate the message.</span></span> <span data-ttu-id="e5300-173">Обновляемые только если isDraft = true, а также время отправки сообщения из [общего почтового ящика](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)или отправка сообщения [Делегирование](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="e5300-173">Updatable only if isDraft = true, and when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="e5300-174">В любом случае значение должно соответствовать фактический почтового ящика, используемого.</span><span class="sxs-lookup"><span data-stu-id="e5300-174">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="e5300-175">toRecipients</span><span class="sxs-lookup"><span data-stu-id="e5300-175">toRecipients</span></span>|<span data-ttu-id="e5300-176">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="e5300-176">Recipient collection</span></span>|<span data-ttu-id="e5300-177">Кому получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="e5300-177">The To recipients for the message.</span></span> <span data-ttu-id="e5300-178">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="e5300-178">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="e5300-179">Основной текст</span><span class="sxs-lookup"><span data-stu-id="e5300-179">body</span></span>|<span data-ttu-id="e5300-180">ItemBody</span><span class="sxs-lookup"><span data-stu-id="e5300-180">ItemBody</span></span>|<span data-ttu-id="e5300-181">Текст сообщения.</span><span class="sxs-lookup"><span data-stu-id="e5300-181">The body of the message.</span></span> <span data-ttu-id="e5300-182">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="e5300-182">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="e5300-183">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="e5300-183">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="e5300-184">Логический</span><span class="sxs-lookup"><span data-stu-id="e5300-184">Boolean</span></span>|<span data-ttu-id="e5300-185">Указывает, необходимо ли запрашивать уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="e5300-185">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="e5300-186">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="e5300-186">isReadReceiptRequested</span></span>|<span data-ttu-id="e5300-187">Логический</span><span class="sxs-lookup"><span data-stu-id="e5300-187">Boolean</span></span>|<span data-ttu-id="e5300-188">Указывает, необходимо ли запрашивать уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="e5300-188">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="e5300-189">subject</span><span class="sxs-lookup"><span data-stu-id="e5300-189">subject</span></span>|<span data-ttu-id="e5300-190">String</span><span class="sxs-lookup"><span data-stu-id="e5300-190">String</span></span>|<span data-ttu-id="e5300-191">Тема сообщения.</span><span class="sxs-lookup"><span data-stu-id="e5300-191">The subject of the message.</span></span> <span data-ttu-id="e5300-192">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="e5300-192">Updatable only if isDraft = true.</span></span>|

<span data-ttu-id="e5300-193">Так как ресурс **message** поддерживает [расширения](../../../concepts/extensibility_overview.md), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="e5300-193">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="e5300-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5300-194">Response</span></span>

<span data-ttu-id="e5300-195">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5300-195">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e5300-196">Пример</span><span class="sxs-lookup"><span data-stu-id="e5300-196">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5300-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5300-197">Request</span></span>
<span data-ttu-id="e5300-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5300-198">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="e5300-199">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5300-199">Response</span></span>
<span data-ttu-id="e5300-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e5300-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="e5300-203">См. также</span><span class="sxs-lookup"><span data-stu-id="e5300-203">See also</span></span>

- [<span data-ttu-id="e5300-204">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="e5300-204">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="e5300-205">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e5300-205">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
