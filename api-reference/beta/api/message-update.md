---
title: Обновление сообщения
description: Обновление свойств объекта сообщения.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: fbb2654dba88693964b20368c2c7a54daf3f5356
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33597829"
---
# <a name="update-message"></a><span data-ttu-id="39092-103">Обновление сообщения</span><span class="sxs-lookup"><span data-stu-id="39092-103">Update message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39092-104">Обновление свойств объекта сообщения.</span><span class="sxs-lookup"><span data-stu-id="39092-104">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="39092-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39092-105">Permissions</span></span>
<span data-ttu-id="39092-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39092-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39092-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39092-108">Permission type</span></span>      | <span data-ttu-id="39092-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39092-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39092-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39092-110">Delegated (work or school account)</span></span> | <span data-ttu-id="39092-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39092-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="39092-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39092-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39092-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39092-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="39092-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39092-114">Application</span></span> | <span data-ttu-id="39092-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39092-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="39092-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39092-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="39092-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39092-117">Request headers</span></span>
| <span data-ttu-id="39092-118">Имя</span><span class="sxs-lookup"><span data-stu-id="39092-118">Name</span></span>       | <span data-ttu-id="39092-119">Тип</span><span class="sxs-lookup"><span data-stu-id="39092-119">Type</span></span> | <span data-ttu-id="39092-120">Описание</span><span class="sxs-lookup"><span data-stu-id="39092-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="39092-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="39092-121">Authorization</span></span>  | <span data-ttu-id="39092-122">string</span><span class="sxs-lookup"><span data-stu-id="39092-122">string</span></span>  | <span data-ttu-id="39092-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39092-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="39092-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="39092-125">Content-Type</span></span> | <span data-ttu-id="39092-126">string</span><span class="sxs-lookup"><span data-stu-id="39092-126">string</span></span>  | <span data-ttu-id="39092-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39092-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="39092-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39092-129">Request body</span></span>
<span data-ttu-id="39092-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="39092-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="39092-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="39092-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="39092-132">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="39092-132">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="39092-133">Могут быть обновлены перечисленные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="39092-133">The following properties can be updated.</span></span>

| <span data-ttu-id="39092-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="39092-134">Property</span></span>     | <span data-ttu-id="39092-135">Тип</span><span class="sxs-lookup"><span data-stu-id="39092-135">Type</span></span>   |<span data-ttu-id="39092-136">Описание</span><span class="sxs-lookup"><span data-stu-id="39092-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39092-137">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="39092-137">bccRecipients</span></span>|<span data-ttu-id="39092-138">Recipient</span><span class="sxs-lookup"><span data-stu-id="39092-138">Recipient</span></span>|<span data-ttu-id="39092-139">Получатели скрытой копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="39092-139">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="39092-140">body</span><span class="sxs-lookup"><span data-stu-id="39092-140">body</span></span>|<span data-ttu-id="39092-141">ItemBody</span><span class="sxs-lookup"><span data-stu-id="39092-141">ItemBody</span></span>|<span data-ttu-id="39092-142">Текст сообщения.</span><span class="sxs-lookup"><span data-stu-id="39092-142">The body of the message.</span></span> <span data-ttu-id="39092-143">Можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="39092-143">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="39092-144">categories</span><span class="sxs-lookup"><span data-stu-id="39092-144">categories</span></span>|<span data-ttu-id="39092-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="39092-145">String collection</span></span>|<span data-ttu-id="39092-146">Категории, сопоставленные с сообщением.</span><span class="sxs-lookup"><span data-stu-id="39092-146">The categories associated with the message.</span></span>|
|<span data-ttu-id="39092-147">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="39092-147">ccRecipients</span></span>|<span data-ttu-id="39092-148">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="39092-148">Recipient collection</span></span>|<span data-ttu-id="39092-149">Получатели копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="39092-149">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="39092-150">flag</span><span class="sxs-lookup"><span data-stu-id="39092-150">flag</span></span>|[<span data-ttu-id="39092-151">followupFlag</span><span class="sxs-lookup"><span data-stu-id="39092-151">followupFlag</span></span>](../resources/followupflag.md)|<span data-ttu-id="39092-152">Значение флага, которое указывает статус, дату начала, дату выполнения или дату завершения сообщения.</span><span class="sxs-lookup"><span data-stu-id="39092-152">The flag value that indicates the status, start date, due date, or completion date for the message.</span></span>|
|<span data-ttu-id="39092-153">from</span><span class="sxs-lookup"><span data-stu-id="39092-153">from</span></span>|<span data-ttu-id="39092-154">Recipient</span><span class="sxs-lookup"><span data-stu-id="39092-154">Recipient</span></span>|<span data-ttu-id="39092-155">Владелец почтового ящика и отправитель сообщения.</span><span class="sxs-lookup"><span data-stu-id="39092-155">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="39092-156">Должно соответствовать фактически используемому почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="39092-156">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="39092-157">importance</span><span class="sxs-lookup"><span data-stu-id="39092-157">importance</span></span>|<span data-ttu-id="39092-158">String</span><span class="sxs-lookup"><span data-stu-id="39092-158">String</span></span>|<span data-ttu-id="39092-p107">Важность сообщения. Возможные значения: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="39092-p107">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="39092-161">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="39092-161">inferenceClassification</span></span> | <span data-ttu-id="39092-162">String</span><span class="sxs-lookup"><span data-stu-id="39092-162">String</span></span> | <span data-ttu-id="39092-p108">Классификация сообщения для пользователя на основании подразумеваемой релевантности или важности либо явного переопределения. Возможные значения: `focused` или `other`.</span><span class="sxs-lookup"><span data-stu-id="39092-p108">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="39092-165">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="39092-165">internetMessageId</span></span> |<span data-ttu-id="39092-166">String</span><span class="sxs-lookup"><span data-stu-id="39092-166">String</span></span> |<span data-ttu-id="39092-167">Идентификатор сообщения в формате, установленном документом [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span><span class="sxs-lookup"><span data-stu-id="39092-167">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="39092-168">Можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="39092-168">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="39092-169">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="39092-169">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="39092-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="39092-170">Boolean</span></span>|<span data-ttu-id="39092-171">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="39092-171">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="39092-172">isRead</span><span class="sxs-lookup"><span data-stu-id="39092-172">isRead</span></span>|<span data-ttu-id="39092-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="39092-173">Boolean</span></span>|<span data-ttu-id="39092-174">Указывает, прочитано ли сообщение.</span><span class="sxs-lookup"><span data-stu-id="39092-174">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="39092-175">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="39092-175">isReadReceiptRequested</span></span>|<span data-ttu-id="39092-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="39092-176">Boolean</span></span>|<span data-ttu-id="39092-177">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="39092-177">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="39092-178">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="39092-178">multiValueExtendedProperties</span></span>|<span data-ttu-id="39092-179">Коллекция [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="39092-179">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="39092-180">Коллекция многозначных расширенных свойств, определенных для сообщения.</span><span class="sxs-lookup"><span data-stu-id="39092-180">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="39092-181">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="39092-181">Nullable.</span></span>|
|<span data-ttu-id="39092-182">replyTo</span><span class="sxs-lookup"><span data-stu-id="39092-182">replyTo</span></span>|<span data-ttu-id="39092-183">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="39092-183">Recipient collection</span></span>|<span data-ttu-id="39092-184">Электронные адреса, которые необходимо использовать при ответе.</span><span class="sxs-lookup"><span data-stu-id="39092-184">The email addresses to use when replying.</span></span> <span data-ttu-id="39092-185">Можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="39092-185">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="39092-186">sender</span><span class="sxs-lookup"><span data-stu-id="39092-186">sender</span></span>|<span data-ttu-id="39092-187">Recipient</span><span class="sxs-lookup"><span data-stu-id="39092-187">Recipient</span></span>|<span data-ttu-id="39092-188">Учетная запись, которая фактически используется для создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="39092-188">The account that is actually used to generate the message.</span></span> <span data-ttu-id="39092-189">Можно изменять при отправке сообщения из [общего почтового ящика](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes) или отправке сообщения в качестве [представителя](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="39092-189">Updatable when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="39092-190">В любом случае значение должно соответствовать фактически используемому почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="39092-190">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="39092-191">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="39092-191">singleValueExtendedProperties</span></span>|<span data-ttu-id="39092-192">Коллекция [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="39092-192">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="39092-193">Коллекция однозначных расширенных свойств, определенных для сообщения.</span><span class="sxs-lookup"><span data-stu-id="39092-193">The collection of single-value extended properties defined for the message.</span></span> <span data-ttu-id="39092-194">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="39092-194">Nullable.</span></span>|
|<span data-ttu-id="39092-195">subject</span><span class="sxs-lookup"><span data-stu-id="39092-195">subject</span></span>|<span data-ttu-id="39092-196">String</span><span class="sxs-lookup"><span data-stu-id="39092-196">String</span></span>|<span data-ttu-id="39092-197">Тема сообщения.</span><span class="sxs-lookup"><span data-stu-id="39092-197">The subject of the message.</span></span> <span data-ttu-id="39092-198">Можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="39092-198">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="39092-199">toRecipients</span><span class="sxs-lookup"><span data-stu-id="39092-199">toRecipients</span></span>|<span data-ttu-id="39092-200">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="39092-200">Recipient collection</span></span>|<span data-ttu-id="39092-201">Получатели сообщения, указанные в поле "Кому".</span><span class="sxs-lookup"><span data-stu-id="39092-201">The To recipients for the message.</span></span> |

<span data-ttu-id="39092-202">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="39092-202">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="39092-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="39092-203">Response</span></span>

<span data-ttu-id="39092-204">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="39092-204">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="39092-205">Пример</span><span class="sxs-lookup"><span data-stu-id="39092-205">Example</span></span>
##### <a name="request"></a><span data-ttu-id="39092-206">Запрос</span><span class="sxs-lookup"><span data-stu-id="39092-206">Request</span></span>
<span data-ttu-id="39092-207">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39092-207">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="39092-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="39092-208">Response</span></span>
<span data-ttu-id="39092-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="39092-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="39092-212">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="39092-212">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="39092-213">Языках</span><span class="sxs-lookup"><span data-stu-id="39092-213">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="39092-214">Язык</span><span class="sxs-lookup"><span data-stu-id="39092-214">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_message-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="39092-215">См. также</span><span class="sxs-lookup"><span data-stu-id="39092-215">See also</span></span>

- [<span data-ttu-id="39092-216">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="39092-216">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="39092-217">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="39092-217">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="39092-218">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="39092-218">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
