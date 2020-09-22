---
title: Обновление сообщения
description: Обновление свойств объекта сообщения.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 821db8f4115b551b93d65592b5ffb2cc51513758
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058811"
---
# <a name="update-message"></a><span data-ttu-id="2127e-103">Обновление сообщения</span><span class="sxs-lookup"><span data-stu-id="2127e-103">Update message</span></span>

<span data-ttu-id="2127e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2127e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2127e-105">Обновление свойств объекта сообщения.</span><span class="sxs-lookup"><span data-stu-id="2127e-105">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2127e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2127e-106">Permissions</span></span>
<span data-ttu-id="2127e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2127e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2127e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2127e-109">Permission type</span></span>      | <span data-ttu-id="2127e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2127e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2127e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2127e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2127e-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2127e-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2127e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2127e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2127e-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2127e-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2127e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2127e-115">Application</span></span> | <span data-ttu-id="2127e-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2127e-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2127e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2127e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2127e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2127e-118">Request headers</span></span>
| <span data-ttu-id="2127e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2127e-119">Name</span></span>       | <span data-ttu-id="2127e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="2127e-120">Type</span></span> | <span data-ttu-id="2127e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2127e-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2127e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2127e-122">Authorization</span></span>  | <span data-ttu-id="2127e-123">string</span><span class="sxs-lookup"><span data-stu-id="2127e-123">string</span></span>  | <span data-ttu-id="2127e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2127e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2127e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2127e-126">Content-Type</span></span> | <span data-ttu-id="2127e-127">string</span><span class="sxs-lookup"><span data-stu-id="2127e-127">string</span></span>  | <span data-ttu-id="2127e-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2127e-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="2127e-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2127e-130">Request body</span></span>
<span data-ttu-id="2127e-131">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="2127e-131">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2127e-132">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="2127e-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2127e-133">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2127e-133">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="2127e-134">Могут быть обновлены перечисленные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="2127e-134">The following properties can be updated.</span></span>

| <span data-ttu-id="2127e-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="2127e-135">Property</span></span>     | <span data-ttu-id="2127e-136">Тип</span><span class="sxs-lookup"><span data-stu-id="2127e-136">Type</span></span>   |<span data-ttu-id="2127e-137">Описание</span><span class="sxs-lookup"><span data-stu-id="2127e-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2127e-138">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="2127e-138">bccRecipients</span></span>|<span data-ttu-id="2127e-139">Recipient</span><span class="sxs-lookup"><span data-stu-id="2127e-139">Recipient</span></span>|<span data-ttu-id="2127e-140">Получатели скрытой копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="2127e-140">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="2127e-141">body</span><span class="sxs-lookup"><span data-stu-id="2127e-141">body</span></span>|<span data-ttu-id="2127e-142">ItemBody</span><span class="sxs-lookup"><span data-stu-id="2127e-142">ItemBody</span></span>|<span data-ttu-id="2127e-143">Текст сообщения.</span><span class="sxs-lookup"><span data-stu-id="2127e-143">The body of the message.</span></span> <span data-ttu-id="2127e-144">Можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="2127e-144">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="2127e-145">categories</span><span class="sxs-lookup"><span data-stu-id="2127e-145">categories</span></span>|<span data-ttu-id="2127e-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2127e-146">String collection</span></span>|<span data-ttu-id="2127e-147">Категории, сопоставленные с сообщением.</span><span class="sxs-lookup"><span data-stu-id="2127e-147">The categories associated with the message.</span></span>|
|<span data-ttu-id="2127e-148">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="2127e-148">ccRecipients</span></span>|<span data-ttu-id="2127e-149">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="2127e-149">Recipient collection</span></span>|<span data-ttu-id="2127e-150">Получатели копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="2127e-150">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="2127e-151">flag</span><span class="sxs-lookup"><span data-stu-id="2127e-151">flag</span></span>|[<span data-ttu-id="2127e-152">followupFlag</span><span class="sxs-lookup"><span data-stu-id="2127e-152">followupFlag</span></span>](../resources/followupflag.md)|<span data-ttu-id="2127e-153">Значение флага, которое указывает статус, дату начала, дату выполнения или дату завершения сообщения.</span><span class="sxs-lookup"><span data-stu-id="2127e-153">The flag value that indicates the status, start date, due date, or completion date for the message.</span></span>|
|<span data-ttu-id="2127e-154">from</span><span class="sxs-lookup"><span data-stu-id="2127e-154">from</span></span>|<span data-ttu-id="2127e-155">Recipient</span><span class="sxs-lookup"><span data-stu-id="2127e-155">Recipient</span></span>|<span data-ttu-id="2127e-156">Владелец почтового ящика и отправитель сообщения.</span><span class="sxs-lookup"><span data-stu-id="2127e-156">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="2127e-157">Должно соответствовать фактически используемому почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="2127e-157">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="2127e-158">importance</span><span class="sxs-lookup"><span data-stu-id="2127e-158">importance</span></span>|<span data-ttu-id="2127e-159">String</span><span class="sxs-lookup"><span data-stu-id="2127e-159">String</span></span>|<span data-ttu-id="2127e-p107">Важность сообщения. Возможные значения: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="2127e-p107">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="2127e-162">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="2127e-162">inferenceClassification</span></span> | <span data-ttu-id="2127e-163">String</span><span class="sxs-lookup"><span data-stu-id="2127e-163">String</span></span> | <span data-ttu-id="2127e-p108">Классификация сообщения для пользователя на основании подразумеваемой релевантности или важности либо явного переопределения. Возможные значения: `focused` или `other`.</span><span class="sxs-lookup"><span data-stu-id="2127e-p108">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="2127e-166">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="2127e-166">internetMessageId</span></span> |<span data-ttu-id="2127e-167">String</span><span class="sxs-lookup"><span data-stu-id="2127e-167">String</span></span> |<span data-ttu-id="2127e-168">Идентификатор сообщения в формате, установленном документом [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span><span class="sxs-lookup"><span data-stu-id="2127e-168">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="2127e-169">Можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="2127e-169">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="2127e-170">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="2127e-170">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="2127e-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="2127e-171">Boolean</span></span>|<span data-ttu-id="2127e-172">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="2127e-172">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="2127e-173">isRead</span><span class="sxs-lookup"><span data-stu-id="2127e-173">isRead</span></span>|<span data-ttu-id="2127e-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="2127e-174">Boolean</span></span>|<span data-ttu-id="2127e-175">Указывает, прочитано ли сообщение.</span><span class="sxs-lookup"><span data-stu-id="2127e-175">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="2127e-176">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="2127e-176">isReadReceiptRequested</span></span>|<span data-ttu-id="2127e-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="2127e-177">Boolean</span></span>|<span data-ttu-id="2127e-178">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="2127e-178">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="2127e-179">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="2127e-179">multiValueExtendedProperties</span></span>|<span data-ttu-id="2127e-180">Коллекция [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="2127e-180">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="2127e-181">Коллекция многозначных расширенных свойств, определенных для сообщения.</span><span class="sxs-lookup"><span data-stu-id="2127e-181">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="2127e-182">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2127e-182">Nullable.</span></span>|
|<span data-ttu-id="2127e-183">replyTo</span><span class="sxs-lookup"><span data-stu-id="2127e-183">replyTo</span></span>|<span data-ttu-id="2127e-184">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="2127e-184">Recipient collection</span></span>|<span data-ttu-id="2127e-185">Электронные адреса, которые необходимо использовать при ответе.</span><span class="sxs-lookup"><span data-stu-id="2127e-185">The email addresses to use when replying.</span></span> <span data-ttu-id="2127e-186">Можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="2127e-186">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="2127e-187">sender</span><span class="sxs-lookup"><span data-stu-id="2127e-187">sender</span></span>|<span data-ttu-id="2127e-188">Recipient</span><span class="sxs-lookup"><span data-stu-id="2127e-188">Recipient</span></span>|<span data-ttu-id="2127e-189">Учетная запись, которая фактически используется для создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="2127e-189">The account that is actually used to generate the message.</span></span> <span data-ttu-id="2127e-190">Можно изменять при отправке сообщения из [общего почтового ящика](/exchange/collaboration/shared-mailboxes/shared-mailboxes) или отправке сообщения в качестве [представителя](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="2127e-190">Updatable when sending a message from a [shared mailbox](/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="2127e-191">В любом случае значение должно соответствовать фактически используемому почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="2127e-191">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="2127e-192">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="2127e-192">singleValueExtendedProperties</span></span>|<span data-ttu-id="2127e-193">Коллекция [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="2127e-193">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="2127e-194">Коллекция однозначных расширенных свойств, определенных для сообщения.</span><span class="sxs-lookup"><span data-stu-id="2127e-194">The collection of single-value extended properties defined for the message.</span></span> <span data-ttu-id="2127e-195">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2127e-195">Nullable.</span></span>|
|<span data-ttu-id="2127e-196">subject</span><span class="sxs-lookup"><span data-stu-id="2127e-196">subject</span></span>|<span data-ttu-id="2127e-197">String</span><span class="sxs-lookup"><span data-stu-id="2127e-197">String</span></span>|<span data-ttu-id="2127e-198">Тема сообщения.</span><span class="sxs-lookup"><span data-stu-id="2127e-198">The subject of the message.</span></span> <span data-ttu-id="2127e-199">Можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="2127e-199">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="2127e-200">toRecipients</span><span class="sxs-lookup"><span data-stu-id="2127e-200">toRecipients</span></span>|<span data-ttu-id="2127e-201">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="2127e-201">Recipient collection</span></span>|<span data-ttu-id="2127e-202">Получатели сообщения, указанные в поле "Кому".</span><span class="sxs-lookup"><span data-stu-id="2127e-202">The To recipients for the message.</span></span> |

<span data-ttu-id="2127e-203">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="2127e-203">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="2127e-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="2127e-204">Response</span></span>

<span data-ttu-id="2127e-205">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2127e-205">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2127e-206">Пример</span><span class="sxs-lookup"><span data-stu-id="2127e-206">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2127e-207">Запрос</span><span class="sxs-lookup"><span data-stu-id="2127e-207">Request</span></span>
<span data-ttu-id="2127e-208">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2127e-208">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2127e-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="2127e-209">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2127e-210">C#</span><span class="sxs-lookup"><span data-stu-id="2127e-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2127e-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2127e-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2127e-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="2127e-212">Response</span></span>
<span data-ttu-id="2127e-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2127e-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="2127e-216">См. также</span><span class="sxs-lookup"><span data-stu-id="2127e-216">See also</span></span>

- [<span data-ttu-id="2127e-217">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="2127e-217">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="2127e-218">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2127e-218">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="2127e-219">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2127e-219">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
  ]
}
-->


