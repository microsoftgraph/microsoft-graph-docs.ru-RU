---
title: Обновление сообщения
description: Обновление свойств объекта сообщения.
author: angelgolfer-ms
ms.openlocfilehash: b8f39dc9648203f86749ba06b88bf2f74b79d88a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337543"
---
# <a name="update-message"></a><span data-ttu-id="0213d-103">Обновление сообщения</span><span class="sxs-lookup"><span data-stu-id="0213d-103">Update message</span></span>

<span data-ttu-id="0213d-104">Обновление свойств объекта сообщения.</span><span class="sxs-lookup"><span data-stu-id="0213d-104">Update the properties of message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0213d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0213d-105">Permissions</span></span>
<span data-ttu-id="0213d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0213d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0213d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0213d-108">Permission type</span></span>      | <span data-ttu-id="0213d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0213d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0213d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0213d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0213d-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0213d-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0213d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0213d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0213d-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0213d-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0213d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0213d-114">Application</span></span> | <span data-ttu-id="0213d-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0213d-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0213d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0213d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0213d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0213d-117">Request headers</span></span>
| <span data-ttu-id="0213d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0213d-118">Name</span></span>       | <span data-ttu-id="0213d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0213d-119">Type</span></span> | <span data-ttu-id="0213d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0213d-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0213d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0213d-121">Authorization</span></span>  | <span data-ttu-id="0213d-122">string</span><span class="sxs-lookup"><span data-stu-id="0213d-122">string</span></span>  | <span data-ttu-id="0213d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0213d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0213d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0213d-125">Content-Type</span></span> | <span data-ttu-id="0213d-126">string</span><span class="sxs-lookup"><span data-stu-id="0213d-126">string</span></span>  | <span data-ttu-id="0213d-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0213d-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="0213d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0213d-129">Request body</span></span>
<span data-ttu-id="0213d-p104">В основном тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, доступные для записи и обновления.</span><span class="sxs-lookup"><span data-stu-id="0213d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="0213d-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="0213d-134">Property</span></span>     | <span data-ttu-id="0213d-135">Тип</span><span class="sxs-lookup"><span data-stu-id="0213d-135">Type</span></span>   |<span data-ttu-id="0213d-136">Описание</span><span class="sxs-lookup"><span data-stu-id="0213d-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0213d-137">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="0213d-137">bccRecipients</span></span>|<span data-ttu-id="0213d-138">Recipient</span><span class="sxs-lookup"><span data-stu-id="0213d-138">Recipient</span></span>|<span data-ttu-id="0213d-139">Получателей скрытой копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="0213d-139">The Bcc recipients for the message.</span></span> <span data-ttu-id="0213d-140">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="0213d-140">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="0213d-141">categories</span><span class="sxs-lookup"><span data-stu-id="0213d-141">categories</span></span>|<span data-ttu-id="0213d-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0213d-142">String collection</span></span>|<span data-ttu-id="0213d-143">Категории, сопоставленные с сообщением.</span><span class="sxs-lookup"><span data-stu-id="0213d-143">The categories associated with the message.</span></span>|
|<span data-ttu-id="0213d-144">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="0213d-144">ccRecipients</span></span>|<span data-ttu-id="0213d-145">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="0213d-145">Recipient collection</span></span>|<span data-ttu-id="0213d-146">Получателей копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="0213d-146">The Cc recipients for the message.</span></span> <span data-ttu-id="0213d-147">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="0213d-147">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="0213d-148">from</span><span class="sxs-lookup"><span data-stu-id="0213d-148">from</span></span>|<span data-ttu-id="0213d-149">Recipient</span><span class="sxs-lookup"><span data-stu-id="0213d-149">Recipient</span></span>|<span data-ttu-id="0213d-150">Владелец почтового ящика и отправитель сообщения.</span><span class="sxs-lookup"><span data-stu-id="0213d-150">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="0213d-151">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="0213d-151">Updatable only if isDraft = true.</span></span> <span data-ttu-id="0213d-152">Должно соответствовать фактический почтового ящика, используемого.</span><span class="sxs-lookup"><span data-stu-id="0213d-152">Must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="0213d-153">importance</span><span class="sxs-lookup"><span data-stu-id="0213d-153">importance</span></span>|<span data-ttu-id="0213d-154">Строка</span><span class="sxs-lookup"><span data-stu-id="0213d-154">String</span></span>|<span data-ttu-id="0213d-155">Важность сообщения.</span><span class="sxs-lookup"><span data-stu-id="0213d-155">The importance of the message.</span></span> <span data-ttu-id="0213d-156">Возможные значения: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="0213d-156">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="0213d-157">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="0213d-157">inferenceClassification</span></span> | <span data-ttu-id="0213d-158">Строка</span><span class="sxs-lookup"><span data-stu-id="0213d-158">String</span></span> | <span data-ttu-id="0213d-159">Классификация сообщений для пользователя, на основе предполагаемых релевантность или важность, или явное переопределение.</span><span class="sxs-lookup"><span data-stu-id="0213d-159">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override.</span></span> <span data-ttu-id="0213d-160">Возможные значения: `focused` или `other`.</span><span class="sxs-lookup"><span data-stu-id="0213d-160">The possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="0213d-161">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="0213d-161">internetMessageId</span></span> |<span data-ttu-id="0213d-162">String</span><span class="sxs-lookup"><span data-stu-id="0213d-162">String</span></span> |<span data-ttu-id="0213d-163">Идентификатор сообщения в формате, установленном документом [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span><span class="sxs-lookup"><span data-stu-id="0213d-163">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="0213d-164">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="0213d-164">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="0213d-165">isRead</span><span class="sxs-lookup"><span data-stu-id="0213d-165">isRead</span></span>|<span data-ttu-id="0213d-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="0213d-166">Boolean</span></span>|<span data-ttu-id="0213d-167">Указывает, прочитано ли сообщение.</span><span class="sxs-lookup"><span data-stu-id="0213d-167">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="0213d-168">replyTo</span><span class="sxs-lookup"><span data-stu-id="0213d-168">replyTo</span></span>|<span data-ttu-id="0213d-169">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="0213d-169">Recipient collection</span></span>|<span data-ttu-id="0213d-170">Электронные адреса, которые необходимо использовать при ответе.</span><span class="sxs-lookup"><span data-stu-id="0213d-170">The email addresses to use when replying.</span></span> <span data-ttu-id="0213d-171">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="0213d-171">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="0213d-172">sender</span><span class="sxs-lookup"><span data-stu-id="0213d-172">sender</span></span>|<span data-ttu-id="0213d-173">Recipient</span><span class="sxs-lookup"><span data-stu-id="0213d-173">Recipient</span></span>|<span data-ttu-id="0213d-174">Учетная запись, которая фактически используется для создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="0213d-174">The account that is actually used to generate the message.</span></span> <span data-ttu-id="0213d-175">Обновляемые только если isDraft = true, а также время отправки сообщения из [общего почтового ящика](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)или отправка сообщения [Делегирование](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="0213d-175">Updatable only if isDraft = true, and when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="0213d-176">В любом случае значение должно соответствовать фактический почтового ящика, используемого.</span><span class="sxs-lookup"><span data-stu-id="0213d-176">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="0213d-177">toRecipients</span><span class="sxs-lookup"><span data-stu-id="0213d-177">toRecipients</span></span>|<span data-ttu-id="0213d-178">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="0213d-178">Recipient collection</span></span>|<span data-ttu-id="0213d-179">Кому получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="0213d-179">The To recipients for the message.</span></span> <span data-ttu-id="0213d-180">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="0213d-180">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="0213d-181">Основной текст</span><span class="sxs-lookup"><span data-stu-id="0213d-181">body</span></span>|<span data-ttu-id="0213d-182">ItemBody</span><span class="sxs-lookup"><span data-stu-id="0213d-182">ItemBody</span></span>|<span data-ttu-id="0213d-183">Текст сообщения.</span><span class="sxs-lookup"><span data-stu-id="0213d-183">The body of the message.</span></span> <span data-ttu-id="0213d-184">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="0213d-184">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="0213d-185">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="0213d-185">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="0213d-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="0213d-186">Boolean</span></span>|<span data-ttu-id="0213d-187">Указывает, необходимо ли запрашивать уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="0213d-187">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="0213d-188">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="0213d-188">isReadReceiptRequested</span></span>|<span data-ttu-id="0213d-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="0213d-189">Boolean</span></span>|<span data-ttu-id="0213d-190">Указывает, необходимо ли запрашивать уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="0213d-190">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="0213d-191">subject</span><span class="sxs-lookup"><span data-stu-id="0213d-191">subject</span></span>|<span data-ttu-id="0213d-192">String</span><span class="sxs-lookup"><span data-stu-id="0213d-192">String</span></span>|<span data-ttu-id="0213d-193">Тема сообщения.</span><span class="sxs-lookup"><span data-stu-id="0213d-193">The subject of the message.</span></span> <span data-ttu-id="0213d-194">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="0213d-194">Updatable only if isDraft = true.</span></span>|

<span data-ttu-id="0213d-195">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="0213d-195">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="0213d-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="0213d-196">Response</span></span>

<span data-ttu-id="0213d-197">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0213d-197">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0213d-198">Пример</span><span class="sxs-lookup"><span data-stu-id="0213d-198">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0213d-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="0213d-199">Request</span></span>
<span data-ttu-id="0213d-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0213d-200">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="0213d-201">Ответ</span><span class="sxs-lookup"><span data-stu-id="0213d-201">Response</span></span>
<span data-ttu-id="0213d-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0213d-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="0213d-205">См. также</span><span class="sxs-lookup"><span data-stu-id="0213d-205">See also</span></span>

- [<span data-ttu-id="0213d-206">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="0213d-206">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0213d-207">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="0213d-207">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
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
