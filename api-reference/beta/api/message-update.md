---
title: Обновление сообщения
description: Обновление свойств объекта сообщения.
ms.openlocfilehash: 0411decc2758505f6116b0a7c619887f3d8e239e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082758"
---
# <a name="update-message"></a><span data-ttu-id="9375f-103">Обновление сообщения</span><span class="sxs-lookup"><span data-stu-id="9375f-103">Update message</span></span>

> <span data-ttu-id="9375f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9375f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9375f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9375f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9375f-106">Обновление свойств объекта сообщения.</span><span class="sxs-lookup"><span data-stu-id="9375f-106">Update the properties of message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9375f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9375f-107">Permissions</span></span>
<span data-ttu-id="9375f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9375f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9375f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9375f-110">Permission type</span></span>      | <span data-ttu-id="9375f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9375f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9375f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9375f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9375f-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9375f-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9375f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9375f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9375f-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9375f-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9375f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9375f-116">Application</span></span> | <span data-ttu-id="9375f-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9375f-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9375f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9375f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9375f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9375f-119">Request headers</span></span>
| <span data-ttu-id="9375f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9375f-120">Name</span></span>       | <span data-ttu-id="9375f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="9375f-121">Type</span></span> | <span data-ttu-id="9375f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9375f-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9375f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9375f-123">Authorization</span></span>  | <span data-ttu-id="9375f-124">string</span><span class="sxs-lookup"><span data-stu-id="9375f-124">string</span></span>  | <span data-ttu-id="9375f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9375f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9375f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9375f-127">Content-Type</span></span> | <span data-ttu-id="9375f-128">string</span><span class="sxs-lookup"><span data-stu-id="9375f-128">string</span></span>  | <span data-ttu-id="9375f-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9375f-p104">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="9375f-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9375f-131">Request body</span></span>
<span data-ttu-id="9375f-p105">В основном тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, доступные для записи и обновления.</span><span class="sxs-lookup"><span data-stu-id="9375f-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="9375f-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="9375f-136">Property</span></span>     | <span data-ttu-id="9375f-137">Тип</span><span class="sxs-lookup"><span data-stu-id="9375f-137">Type</span></span>   |<span data-ttu-id="9375f-138">Описание</span><span class="sxs-lookup"><span data-stu-id="9375f-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9375f-139">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="9375f-139">bccRecipients</span></span>|<span data-ttu-id="9375f-140">Recipient</span><span class="sxs-lookup"><span data-stu-id="9375f-140">Recipient</span></span>|<span data-ttu-id="9375f-141">Получателей скрытой копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="9375f-141">The Bcc recipients for the message.</span></span> <span data-ttu-id="9375f-142">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="9375f-142">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="9375f-143">categories</span><span class="sxs-lookup"><span data-stu-id="9375f-143">categories</span></span>|<span data-ttu-id="9375f-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9375f-144">String collection</span></span>|<span data-ttu-id="9375f-145">Категории, сопоставленные с сообщением.</span><span class="sxs-lookup"><span data-stu-id="9375f-145">The categories associated with the message.</span></span>|
|<span data-ttu-id="9375f-146">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="9375f-146">ccRecipients</span></span>|<span data-ttu-id="9375f-147">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="9375f-147">Recipient collection</span></span>|<span data-ttu-id="9375f-148">Получателей копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="9375f-148">The Cc recipients for the message.</span></span> <span data-ttu-id="9375f-149">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="9375f-149">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="9375f-150">from</span><span class="sxs-lookup"><span data-stu-id="9375f-150">from</span></span>|<span data-ttu-id="9375f-151">Recipient</span><span class="sxs-lookup"><span data-stu-id="9375f-151">Recipient</span></span>|<span data-ttu-id="9375f-152">Владелец почтового ящика и отправитель сообщения.</span><span class="sxs-lookup"><span data-stu-id="9375f-152">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="9375f-153">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="9375f-153">Updatable only if isDraft = true.</span></span> <span data-ttu-id="9375f-154">Должно соответствовать фактический почтового ящика, используемого.</span><span class="sxs-lookup"><span data-stu-id="9375f-154">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="9375f-155">importance</span><span class="sxs-lookup"><span data-stu-id="9375f-155">importance</span></span>|<span data-ttu-id="9375f-156">String</span><span class="sxs-lookup"><span data-stu-id="9375f-156">String</span></span>|<span data-ttu-id="9375f-p109">Важность сообщения. Возможные значения: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="9375f-p109">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="9375f-159">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="9375f-159">inferenceClassification</span></span> | <span data-ttu-id="9375f-160">String</span><span class="sxs-lookup"><span data-stu-id="9375f-160">String</span></span> | <span data-ttu-id="9375f-p110">Классификация сообщения для пользователя на основании подразумеваемой релевантности или важности либо явного переопределения. Возможные значения: `focused` или `other`.</span><span class="sxs-lookup"><span data-stu-id="9375f-p110">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="9375f-163">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="9375f-163">internetMessageId</span></span> |<span data-ttu-id="9375f-164">String</span><span class="sxs-lookup"><span data-stu-id="9375f-164">String</span></span> |<span data-ttu-id="9375f-165">Идентификатор сообщения в формате, установленном документом [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span><span class="sxs-lookup"><span data-stu-id="9375f-165">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="9375f-166">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="9375f-166">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="9375f-167">isRead</span><span class="sxs-lookup"><span data-stu-id="9375f-167">isRead</span></span>|<span data-ttu-id="9375f-168">Логический</span><span class="sxs-lookup"><span data-stu-id="9375f-168">Boolean</span></span>|<span data-ttu-id="9375f-169">Указывает, прочитано ли сообщение.</span><span class="sxs-lookup"><span data-stu-id="9375f-169">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="9375f-170">replyTo</span><span class="sxs-lookup"><span data-stu-id="9375f-170">replyTo</span></span>|<span data-ttu-id="9375f-171">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="9375f-171">Recipient collection</span></span>|<span data-ttu-id="9375f-172">Электронные адреса, которые необходимо использовать при ответе.</span><span class="sxs-lookup"><span data-stu-id="9375f-172">The email addresses to use when replying.</span></span> <span data-ttu-id="9375f-173">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="9375f-173">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="9375f-174">sender</span><span class="sxs-lookup"><span data-stu-id="9375f-174">sender</span></span>|<span data-ttu-id="9375f-175">Recipient</span><span class="sxs-lookup"><span data-stu-id="9375f-175">Recipient</span></span>|<span data-ttu-id="9375f-176">Учетная запись, которая фактически используется для создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="9375f-176">The account that is actually used to generate the message.</span></span> <span data-ttu-id="9375f-177">Обновляемые только если isDraft = true, а также время отправки сообщения из [общего почтового ящика](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)или отправка сообщения [Делегирование](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="9375f-177">Updatable only if isDraft = true, and when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="9375f-178">В любом случае значение должно соответствовать фактический почтового ящика, используемого.</span><span class="sxs-lookup"><span data-stu-id="9375f-178">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="9375f-179">toRecipients</span><span class="sxs-lookup"><span data-stu-id="9375f-179">toRecipients</span></span>|<span data-ttu-id="9375f-180">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="9375f-180">Recipient collection</span></span>|<span data-ttu-id="9375f-181">Кому получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="9375f-181">The To recipients for the message.</span></span> <span data-ttu-id="9375f-182">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="9375f-182">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="9375f-183">Основной текст</span><span class="sxs-lookup"><span data-stu-id="9375f-183">body</span></span>|<span data-ttu-id="9375f-184">ItemBody</span><span class="sxs-lookup"><span data-stu-id="9375f-184">ItemBody</span></span>|<span data-ttu-id="9375f-185">Текст сообщения.</span><span class="sxs-lookup"><span data-stu-id="9375f-185">The body of the message.</span></span> <span data-ttu-id="9375f-186">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="9375f-186">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="9375f-187">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="9375f-187">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="9375f-188">Логический</span><span class="sxs-lookup"><span data-stu-id="9375f-188">Boolean</span></span>|<span data-ttu-id="9375f-189">Указывает, необходимо ли запрашивать уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="9375f-189">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="9375f-190">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="9375f-190">isReadReceiptRequested</span></span>|<span data-ttu-id="9375f-191">Логический</span><span class="sxs-lookup"><span data-stu-id="9375f-191">Boolean</span></span>|<span data-ttu-id="9375f-192">Указывает, необходимо ли запрашивать уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="9375f-192">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="9375f-193">subject</span><span class="sxs-lookup"><span data-stu-id="9375f-193">subject</span></span>|<span data-ttu-id="9375f-194">String</span><span class="sxs-lookup"><span data-stu-id="9375f-194">String</span></span>|<span data-ttu-id="9375f-195">Тема сообщения.</span><span class="sxs-lookup"><span data-stu-id="9375f-195">The subject of the message.</span></span> <span data-ttu-id="9375f-196">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="9375f-196">Updatable only if isDraft = true.</span></span>|

<span data-ttu-id="9375f-197">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="9375f-197">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="9375f-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="9375f-198">Response</span></span>

<span data-ttu-id="9375f-199">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9375f-199">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9375f-200">Пример</span><span class="sxs-lookup"><span data-stu-id="9375f-200">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9375f-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="9375f-201">Request</span></span>
<span data-ttu-id="9375f-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9375f-202">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/messages/{id}
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
##### <a name="response"></a><span data-ttu-id="9375f-203">Ответ</span><span class="sxs-lookup"><span data-stu-id="9375f-203">Response</span></span>
<span data-ttu-id="9375f-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9375f-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
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

## <a name="see-also"></a><span data-ttu-id="9375f-207">См. также</span><span class="sxs-lookup"><span data-stu-id="9375f-207">See also</span></span>

- [<span data-ttu-id="9375f-208">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="9375f-208">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="9375f-209">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="9375f-209">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="9375f-210">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="9375f-210">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
