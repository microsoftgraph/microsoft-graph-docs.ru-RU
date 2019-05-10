---
title: Обновление сообщения
description: Обновление свойств объекта сообщения.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: c16f86ad525fbeef13584cd94d809c0652da8157
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612431"
---
# <a name="update-message"></a><span data-ttu-id="30a4f-103">Обновление сообщения</span><span class="sxs-lookup"><span data-stu-id="30a4f-103">Update message</span></span>

<span data-ttu-id="30a4f-104">Обновление свойств объекта сообщения.</span><span class="sxs-lookup"><span data-stu-id="30a4f-104">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="30a4f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30a4f-105">Permissions</span></span>
<span data-ttu-id="30a4f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30a4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30a4f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30a4f-108">Permission type</span></span>      | <span data-ttu-id="30a4f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30a4f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30a4f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30a4f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="30a4f-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30a4f-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="30a4f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30a4f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30a4f-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30a4f-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="30a4f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30a4f-114">Application</span></span> | <span data-ttu-id="30a4f-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30a4f-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="30a4f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30a4f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="30a4f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30a4f-117">Request headers</span></span>
| <span data-ttu-id="30a4f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="30a4f-118">Name</span></span>       | <span data-ttu-id="30a4f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="30a4f-119">Type</span></span> | <span data-ttu-id="30a4f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="30a4f-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="30a4f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="30a4f-121">Authorization</span></span>  | <span data-ttu-id="30a4f-122">string</span><span class="sxs-lookup"><span data-stu-id="30a4f-122">string</span></span>  | <span data-ttu-id="30a4f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30a4f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="30a4f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="30a4f-125">Content-Type</span></span> | <span data-ttu-id="30a4f-126">string</span><span class="sxs-lookup"><span data-stu-id="30a4f-126">string</span></span>  | <span data-ttu-id="30a4f-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30a4f-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="30a4f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30a4f-129">Request body</span></span>
<span data-ttu-id="30a4f-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="30a4f-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="30a4f-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="30a4f-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="30a4f-132">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="30a4f-132">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="30a4f-133">Могут быть обновлены перечисленные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="30a4f-133">The following properties can be updated.</span></span>

| <span data-ttu-id="30a4f-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="30a4f-134">Property</span></span>     | <span data-ttu-id="30a4f-135">Тип</span><span class="sxs-lookup"><span data-stu-id="30a4f-135">Type</span></span>   |<span data-ttu-id="30a4f-136">Описание</span><span class="sxs-lookup"><span data-stu-id="30a4f-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30a4f-137">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="30a4f-137">bccRecipients</span></span>|<span data-ttu-id="30a4f-138">Recipient</span><span class="sxs-lookup"><span data-stu-id="30a4f-138">Recipient</span></span>|<span data-ttu-id="30a4f-139">Получатели скрытой копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="30a4f-139">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="30a4f-140">body</span><span class="sxs-lookup"><span data-stu-id="30a4f-140">body</span></span>|<span data-ttu-id="30a4f-141">ItemBody</span><span class="sxs-lookup"><span data-stu-id="30a4f-141">ItemBody</span></span>|<span data-ttu-id="30a4f-142">Текст сообщения.</span><span class="sxs-lookup"><span data-stu-id="30a4f-142">The body of the message.</span></span> <span data-ttu-id="30a4f-143">Можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="30a4f-143">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="30a4f-144">categories</span><span class="sxs-lookup"><span data-stu-id="30a4f-144">categories</span></span>|<span data-ttu-id="30a4f-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="30a4f-145">String collection</span></span>|<span data-ttu-id="30a4f-146">Категории, сопоставленные с сообщением.</span><span class="sxs-lookup"><span data-stu-id="30a4f-146">The categories associated with the message.</span></span>|
|<span data-ttu-id="30a4f-147">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="30a4f-147">ccRecipients</span></span>|<span data-ttu-id="30a4f-148">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="30a4f-148">Recipient collection</span></span>|<span data-ttu-id="30a4f-149">Получатели копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="30a4f-149">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="30a4f-150">flag</span><span class="sxs-lookup"><span data-stu-id="30a4f-150">flag</span></span>|[<span data-ttu-id="30a4f-151">followupFlag</span><span class="sxs-lookup"><span data-stu-id="30a4f-151">followupFlag</span></span>](../resources/followupflag.md)|<span data-ttu-id="30a4f-152">Значение флага, которое указывает статус, дату начала, дату выполнения или дату завершения сообщения.</span><span class="sxs-lookup"><span data-stu-id="30a4f-152">The flag value that indicates the status, start date, due date, or completion date for the message.</span></span>|
|<span data-ttu-id="30a4f-153">from</span><span class="sxs-lookup"><span data-stu-id="30a4f-153">from</span></span>|<span data-ttu-id="30a4f-154">Recipient</span><span class="sxs-lookup"><span data-stu-id="30a4f-154">Recipient</span></span>|<span data-ttu-id="30a4f-155">Владелец почтового ящика и отправитель сообщения.</span><span class="sxs-lookup"><span data-stu-id="30a4f-155">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="30a4f-156">Должно соответствовать фактически используемому почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="30a4f-156">Must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="30a4f-157">importance</span><span class="sxs-lookup"><span data-stu-id="30a4f-157">importance</span></span>|<span data-ttu-id="30a4f-158">String</span><span class="sxs-lookup"><span data-stu-id="30a4f-158">String</span></span>|<span data-ttu-id="30a4f-159">Важность сообщения.</span><span class="sxs-lookup"><span data-stu-id="30a4f-159">The importance of the message.</span></span> <span data-ttu-id="30a4f-160">Допустимые значения: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="30a4f-160">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="30a4f-161">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="30a4f-161">inferenceClassification</span></span> | <span data-ttu-id="30a4f-162">String</span><span class="sxs-lookup"><span data-stu-id="30a4f-162">String</span></span> | <span data-ttu-id="30a4f-163">Классификация сообщения для пользователя на основании подразумеваемой релевантности или важности либо явного переопределения.</span><span class="sxs-lookup"><span data-stu-id="30a4f-163">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override.</span></span> <span data-ttu-id="30a4f-164">Допустимые значения: `focused` или `other`.</span><span class="sxs-lookup"><span data-stu-id="30a4f-164">The possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="30a4f-165">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="30a4f-165">internetMessageId</span></span> |<span data-ttu-id="30a4f-166">String</span><span class="sxs-lookup"><span data-stu-id="30a4f-166">String</span></span> |<span data-ttu-id="30a4f-167">Идентификатор сообщения в формате, установленном документом [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span><span class="sxs-lookup"><span data-stu-id="30a4f-167">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="30a4f-168">Можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="30a4f-168">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="30a4f-169">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="30a4f-169">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="30a4f-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="30a4f-170">Boolean</span></span>|<span data-ttu-id="30a4f-171">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="30a4f-171">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="30a4f-172">isRead</span><span class="sxs-lookup"><span data-stu-id="30a4f-172">isRead</span></span>|<span data-ttu-id="30a4f-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="30a4f-173">Boolean</span></span>|<span data-ttu-id="30a4f-174">Указывает, прочитано ли сообщение.</span><span class="sxs-lookup"><span data-stu-id="30a4f-174">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="30a4f-175">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="30a4f-175">isReadReceiptRequested</span></span>|<span data-ttu-id="30a4f-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="30a4f-176">Boolean</span></span>|<span data-ttu-id="30a4f-177">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="30a4f-177">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="30a4f-178">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="30a4f-178">multiValueExtendedProperties</span></span>|<span data-ttu-id="30a4f-179">Коллекция [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="30a4f-179">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="30a4f-180">Коллекция многозначных расширенных свойств, определенных для сообщения.</span><span class="sxs-lookup"><span data-stu-id="30a4f-180">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="30a4f-181">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="30a4f-181">Nullable.</span></span>|
|<span data-ttu-id="30a4f-182">replyTo</span><span class="sxs-lookup"><span data-stu-id="30a4f-182">replyTo</span></span>|<span data-ttu-id="30a4f-183">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="30a4f-183">Recipient collection</span></span>|<span data-ttu-id="30a4f-184">Электронные адреса, которые необходимо использовать при ответе.</span><span class="sxs-lookup"><span data-stu-id="30a4f-184">The email addresses to use when replying.</span></span> <span data-ttu-id="30a4f-185">Можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="30a4f-185">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="30a4f-186">sender</span><span class="sxs-lookup"><span data-stu-id="30a4f-186">sender</span></span>|<span data-ttu-id="30a4f-187">Recipient</span><span class="sxs-lookup"><span data-stu-id="30a4f-187">Recipient</span></span>|<span data-ttu-id="30a4f-188">Учетная запись, которая фактически используется для создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="30a4f-188">The account that is actually used to generate the message.</span></span> <span data-ttu-id="30a4f-189">Можно изменять при отправке сообщения из [общего почтового ящика](https://docs.microsoft.com/ru-RU/exchange/collaboration/shared-mailboxes/shared-mailboxes) или отправке сообщения в качестве [представителя](https://support.office.com/ru-RU/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="30a4f-189">Updatable when sending a message from a [shared mailbox](https://docs.microsoft.com/ru-RU/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/ru-RU/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="30a4f-190">В любом случае значение должно соответствовать фактически используемому почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="30a4f-190">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="30a4f-191">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="30a4f-191">singleValueExtendedProperties</span></span>|<span data-ttu-id="30a4f-192">Коллекция [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="30a4f-192">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="30a4f-193">Коллекция однозначных расширенных свойств, определенных для сообщения.</span><span class="sxs-lookup"><span data-stu-id="30a4f-193">The collection of single-value extended properties defined for the message.</span></span> <span data-ttu-id="30a4f-194">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="30a4f-194">Nullable.</span></span>|
|<span data-ttu-id="30a4f-195">subject</span><span class="sxs-lookup"><span data-stu-id="30a4f-195">subject</span></span>|<span data-ttu-id="30a4f-196">String</span><span class="sxs-lookup"><span data-stu-id="30a4f-196">String</span></span>|<span data-ttu-id="30a4f-197">Тема сообщения.</span><span class="sxs-lookup"><span data-stu-id="30a4f-197">The subject of the message.</span></span> <span data-ttu-id="30a4f-198">Можно обновить, только если параметр IsDraft имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="30a4f-198">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="30a4f-199">toRecipients</span><span class="sxs-lookup"><span data-stu-id="30a4f-199">toRecipients</span></span>|<span data-ttu-id="30a4f-200">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="30a4f-200">Recipient collection</span></span>|<span data-ttu-id="30a4f-201">Получатели сообщения, указанные в поле "Кому".</span><span class="sxs-lookup"><span data-stu-id="30a4f-201">The To recipients for the message.</span></span>|

<span data-ttu-id="30a4f-202">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="30a4f-202">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="30a4f-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="30a4f-203">Response</span></span>

<span data-ttu-id="30a4f-204">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30a4f-204">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="30a4f-205">Пример</span><span class="sxs-lookup"><span data-stu-id="30a4f-205">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30a4f-206">Запрос</span><span class="sxs-lookup"><span data-stu-id="30a4f-206">Request</span></span>
<span data-ttu-id="30a4f-207">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30a4f-207">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="30a4f-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="30a4f-208">Response</span></span>
<span data-ttu-id="30a4f-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30a4f-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="30a4f-212">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="30a4f-212">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="30a4f-213">C#</span><span class="sxs-lookup"><span data-stu-id="30a4f-213">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="30a4f-214">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30a4f-214">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_message-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="30a4f-215">Дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="30a4f-215">See also</span></span>

- [<span data-ttu-id="30a4f-216">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="30a4f-216">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="30a4f-217">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="30a4f-217">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
