---
title: Обновление сообщения
description: Обновление свойств объекта сообщения.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6553365ffd31c56348c930be5562ebd65abc734d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977768"
---
# <a name="update-message"></a><span data-ttu-id="19a33-103">Обновление сообщения</span><span class="sxs-lookup"><span data-stu-id="19a33-103">Update message</span></span>

> <span data-ttu-id="19a33-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="19a33-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19a33-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19a33-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19a33-106">Обновляет свойства объекта message.</span><span class="sxs-lookup"><span data-stu-id="19a33-106">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="19a33-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19a33-107">Permissions</span></span>
<span data-ttu-id="19a33-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19a33-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19a33-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19a33-110">Permission type</span></span>      | <span data-ttu-id="19a33-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19a33-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19a33-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19a33-112">Delegated (work or school account)</span></span> | <span data-ttu-id="19a33-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a33-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="19a33-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19a33-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19a33-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a33-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="19a33-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19a33-116">Application</span></span> | <span data-ttu-id="19a33-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a33-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="19a33-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19a33-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="19a33-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19a33-119">Request headers</span></span>
| <span data-ttu-id="19a33-120">Имя</span><span class="sxs-lookup"><span data-stu-id="19a33-120">Name</span></span>       | <span data-ttu-id="19a33-121">Тип</span><span class="sxs-lookup"><span data-stu-id="19a33-121">Type</span></span> | <span data-ttu-id="19a33-122">Описание</span><span class="sxs-lookup"><span data-stu-id="19a33-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="19a33-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="19a33-123">Authorization</span></span>  | <span data-ttu-id="19a33-124">string</span><span class="sxs-lookup"><span data-stu-id="19a33-124">string</span></span>  | <span data-ttu-id="19a33-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19a33-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19a33-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19a33-127">Content-Type</span></span> | <span data-ttu-id="19a33-128">string</span><span class="sxs-lookup"><span data-stu-id="19a33-128">string</span></span>  | <span data-ttu-id="19a33-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19a33-p104">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="19a33-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19a33-131">Request body</span></span>
<span data-ttu-id="19a33-132">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="19a33-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="19a33-133">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="19a33-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="19a33-134">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="19a33-134">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="19a33-135">Следующие свойства могут быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="19a33-135">The following properties can be updated.</span></span>

| <span data-ttu-id="19a33-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="19a33-136">Property</span></span>     | <span data-ttu-id="19a33-137">Тип</span><span class="sxs-lookup"><span data-stu-id="19a33-137">Type</span></span>   |<span data-ttu-id="19a33-138">Описание</span><span class="sxs-lookup"><span data-stu-id="19a33-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19a33-139">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="19a33-139">bccRecipients</span></span>|<span data-ttu-id="19a33-140">Recipient</span><span class="sxs-lookup"><span data-stu-id="19a33-140">Recipient</span></span>|<span data-ttu-id="19a33-141">Получателей скрытой копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="19a33-141">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="19a33-142">Основной текст</span><span class="sxs-lookup"><span data-stu-id="19a33-142">body</span></span>|<span data-ttu-id="19a33-143">ItemBody</span><span class="sxs-lookup"><span data-stu-id="19a33-143">ItemBody</span></span>|<span data-ttu-id="19a33-144">Текст сообщения.</span><span class="sxs-lookup"><span data-stu-id="19a33-144">The body of the message.</span></span> <span data-ttu-id="19a33-145">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="19a33-145">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="19a33-146">categories</span><span class="sxs-lookup"><span data-stu-id="19a33-146">categories</span></span>|<span data-ttu-id="19a33-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="19a33-147">String collection</span></span>|<span data-ttu-id="19a33-148">Категории, сопоставленные с сообщением.</span><span class="sxs-lookup"><span data-stu-id="19a33-148">The categories associated with the message.</span></span>|
|<span data-ttu-id="19a33-149">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="19a33-149">ccRecipients</span></span>|<span data-ttu-id="19a33-150">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="19a33-150">Recipient collection</span></span>|<span data-ttu-id="19a33-151">Получателей копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="19a33-151">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="19a33-152">from</span><span class="sxs-lookup"><span data-stu-id="19a33-152">from</span></span>|<span data-ttu-id="19a33-153">Recipient</span><span class="sxs-lookup"><span data-stu-id="19a33-153">Recipient</span></span>|<span data-ttu-id="19a33-154">Владелец почтового ящика и отправитель сообщения.</span><span class="sxs-lookup"><span data-stu-id="19a33-154">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="19a33-155">Должно соответствовать фактический почтового ящика, используемого.</span><span class="sxs-lookup"><span data-stu-id="19a33-155">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="19a33-156">importance</span><span class="sxs-lookup"><span data-stu-id="19a33-156">importance</span></span>|<span data-ttu-id="19a33-157">String</span><span class="sxs-lookup"><span data-stu-id="19a33-157">String</span></span>|<span data-ttu-id="19a33-p108">Важность сообщения. Возможные значения: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="19a33-p108">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="19a33-160">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="19a33-160">inferenceClassification</span></span> | <span data-ttu-id="19a33-161">String</span><span class="sxs-lookup"><span data-stu-id="19a33-161">String</span></span> | <span data-ttu-id="19a33-p109">Классификация сообщения для пользователя на основании подразумеваемой релевантности или важности либо явного переопределения. Возможные значения: `focused` или `other`.</span><span class="sxs-lookup"><span data-stu-id="19a33-p109">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="19a33-164">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="19a33-164">internetMessageId</span></span> |<span data-ttu-id="19a33-165">String</span><span class="sxs-lookup"><span data-stu-id="19a33-165">String</span></span> |<span data-ttu-id="19a33-166">Идентификатор сообщения в формате, установленном документом [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span><span class="sxs-lookup"><span data-stu-id="19a33-166">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="19a33-167">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="19a33-167">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="19a33-168">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="19a33-168">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="19a33-169">Логический</span><span class="sxs-lookup"><span data-stu-id="19a33-169">Boolean</span></span>|<span data-ttu-id="19a33-170">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="19a33-170">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="19a33-171">isRead</span><span class="sxs-lookup"><span data-stu-id="19a33-171">isRead</span></span>|<span data-ttu-id="19a33-172">Логический</span><span class="sxs-lookup"><span data-stu-id="19a33-172">Boolean</span></span>|<span data-ttu-id="19a33-173">Указывает, прочитано ли сообщение.</span><span class="sxs-lookup"><span data-stu-id="19a33-173">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="19a33-174">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="19a33-174">isReadReceiptRequested</span></span>|<span data-ttu-id="19a33-175">Логический</span><span class="sxs-lookup"><span data-stu-id="19a33-175">Boolean</span></span>|<span data-ttu-id="19a33-176">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="19a33-176">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="19a33-177">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="19a33-177">multiValueExtendedProperties</span></span>|<span data-ttu-id="19a33-178">Коллекция [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="19a33-178">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="19a33-179">Коллекция Многозначный расширенных свойств, определенных для сообщения.</span><span class="sxs-lookup"><span data-stu-id="19a33-179">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="19a33-180">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="19a33-180">Nullable.</span></span>|
|<span data-ttu-id="19a33-181">replyTo</span><span class="sxs-lookup"><span data-stu-id="19a33-181">replyTo</span></span>|<span data-ttu-id="19a33-182">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="19a33-182">Recipient collection</span></span>|<span data-ttu-id="19a33-183">Электронные адреса, которые необходимо использовать при ответе.</span><span class="sxs-lookup"><span data-stu-id="19a33-183">The email addresses to use when replying.</span></span> <span data-ttu-id="19a33-184">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="19a33-184">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="19a33-185">sender</span><span class="sxs-lookup"><span data-stu-id="19a33-185">sender</span></span>|<span data-ttu-id="19a33-186">Recipient</span><span class="sxs-lookup"><span data-stu-id="19a33-186">Recipient</span></span>|<span data-ttu-id="19a33-187">Учетная запись, которая фактически используется для создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="19a33-187">The account that is actually used to generate the message.</span></span> <span data-ttu-id="19a33-188">Обновляемые при отправке сообщения из [общего почтового ящика](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)или отправка сообщения [Делегирование](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="19a33-188">Updatable when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="19a33-189">В любом случае значение должно соответствовать фактический почтового ящика, используемого.</span><span class="sxs-lookup"><span data-stu-id="19a33-189">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="19a33-190">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="19a33-190">singleValueExtendedProperties</span></span>|<span data-ttu-id="19a33-191">Коллекция [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="19a33-191">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="19a33-192">Коллекция расширенные свойства одно значение, определенное для сообщения.</span><span class="sxs-lookup"><span data-stu-id="19a33-192">The collection of single-value extended properties defined for the message.</span></span> <span data-ttu-id="19a33-193">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="19a33-193">Nullable.</span></span>|
|<span data-ttu-id="19a33-194">subject</span><span class="sxs-lookup"><span data-stu-id="19a33-194">subject</span></span>|<span data-ttu-id="19a33-195">String</span><span class="sxs-lookup"><span data-stu-id="19a33-195">String</span></span>|<span data-ttu-id="19a33-196">Тема сообщения.</span><span class="sxs-lookup"><span data-stu-id="19a33-196">The subject of the message.</span></span> <span data-ttu-id="19a33-197">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="19a33-197">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="19a33-198">toRecipients</span><span class="sxs-lookup"><span data-stu-id="19a33-198">toRecipients</span></span>|<span data-ttu-id="19a33-199">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="19a33-199">Recipient collection</span></span>|<span data-ttu-id="19a33-200">Кому получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="19a33-200">The To recipients for the message.</span></span> |

<span data-ttu-id="19a33-201">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="19a33-201">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="19a33-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="19a33-202">Response</span></span>

<span data-ttu-id="19a33-203">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="19a33-203">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="19a33-204">Пример</span><span class="sxs-lookup"><span data-stu-id="19a33-204">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19a33-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="19a33-205">Request</span></span>
<span data-ttu-id="19a33-206">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19a33-206">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="19a33-207">Ответ</span><span class="sxs-lookup"><span data-stu-id="19a33-207">Response</span></span>
<span data-ttu-id="19a33-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="19a33-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="19a33-211">См. также</span><span class="sxs-lookup"><span data-stu-id="19a33-211">See also</span></span>

- [<span data-ttu-id="19a33-212">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="19a33-212">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="19a33-213">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="19a33-213">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="19a33-214">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="19a33-214">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
