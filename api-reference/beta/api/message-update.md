---
title: Обновление сообщения
description: Обновление свойств объекта сообщения.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5a42e9d6a10e79a4ae801cca464c912dc6fade7b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29644051"
---
# <a name="update-message"></a><span data-ttu-id="b13a3-103">Обновление сообщения</span><span class="sxs-lookup"><span data-stu-id="b13a3-103">Update message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b13a3-104">Обновляет свойства объекта message.</span><span class="sxs-lookup"><span data-stu-id="b13a3-104">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b13a3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b13a3-105">Permissions</span></span>
<span data-ttu-id="b13a3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b13a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b13a3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b13a3-108">Permission type</span></span>      | <span data-ttu-id="b13a3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b13a3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b13a3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b13a3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b13a3-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b13a3-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b13a3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b13a3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b13a3-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b13a3-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b13a3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b13a3-114">Application</span></span> | <span data-ttu-id="b13a3-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b13a3-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b13a3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b13a3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b13a3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b13a3-117">Request headers</span></span>
| <span data-ttu-id="b13a3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b13a3-118">Name</span></span>       | <span data-ttu-id="b13a3-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b13a3-119">Type</span></span> | <span data-ttu-id="b13a3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b13a3-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b13a3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b13a3-121">Authorization</span></span>  | <span data-ttu-id="b13a3-122">строка</span><span class="sxs-lookup"><span data-stu-id="b13a3-122">string</span></span>  | <span data-ttu-id="b13a3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b13a3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b13a3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b13a3-125">Content-Type</span></span> | <span data-ttu-id="b13a3-126">строка</span><span class="sxs-lookup"><span data-stu-id="b13a3-126">string</span></span>  | <span data-ttu-id="b13a3-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b13a3-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="b13a3-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b13a3-129">Request body</span></span>
<span data-ttu-id="b13a3-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="b13a3-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b13a3-131">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="b13a3-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b13a3-132">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b13a3-132">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="b13a3-133">Следующие свойства могут быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="b13a3-133">The following properties can be updated.</span></span>

| <span data-ttu-id="b13a3-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="b13a3-134">Property</span></span>     | <span data-ttu-id="b13a3-135">Тип</span><span class="sxs-lookup"><span data-stu-id="b13a3-135">Type</span></span>   |<span data-ttu-id="b13a3-136">Описание</span><span class="sxs-lookup"><span data-stu-id="b13a3-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b13a3-137">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="b13a3-137">bccRecipients</span></span>|<span data-ttu-id="b13a3-138">Recipient</span><span class="sxs-lookup"><span data-stu-id="b13a3-138">Recipient</span></span>|<span data-ttu-id="b13a3-139">Получателей скрытой копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="b13a3-139">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="b13a3-140">Основной текст</span><span class="sxs-lookup"><span data-stu-id="b13a3-140">body</span></span>|<span data-ttu-id="b13a3-141">ItemBody</span><span class="sxs-lookup"><span data-stu-id="b13a3-141">ItemBody</span></span>|<span data-ttu-id="b13a3-142">Текст сообщения.</span><span class="sxs-lookup"><span data-stu-id="b13a3-142">The body of the message.</span></span> <span data-ttu-id="b13a3-143">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="b13a3-143">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="b13a3-144">categories</span><span class="sxs-lookup"><span data-stu-id="b13a3-144">categories</span></span>|<span data-ttu-id="b13a3-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b13a3-145">String collection</span></span>|<span data-ttu-id="b13a3-146">Категории, связанные с сообщением.</span><span class="sxs-lookup"><span data-stu-id="b13a3-146">The categories associated with the message.</span></span>|
|<span data-ttu-id="b13a3-147">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="b13a3-147">ccRecipients</span></span>|<span data-ttu-id="b13a3-148">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="b13a3-148">Recipient collection</span></span>|<span data-ttu-id="b13a3-149">Получателей копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="b13a3-149">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="b13a3-150">from</span><span class="sxs-lookup"><span data-stu-id="b13a3-150">from</span></span>|<span data-ttu-id="b13a3-151">Recipient</span><span class="sxs-lookup"><span data-stu-id="b13a3-151">Recipient</span></span>|<span data-ttu-id="b13a3-152">Владелец почтового ящика и отправитель сообщения.</span><span class="sxs-lookup"><span data-stu-id="b13a3-152">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="b13a3-153">Должно соответствовать фактический почтового ящика, используемого.</span><span class="sxs-lookup"><span data-stu-id="b13a3-153">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="b13a3-154">importance</span><span class="sxs-lookup"><span data-stu-id="b13a3-154">importance</span></span>|<span data-ttu-id="b13a3-155">String</span><span class="sxs-lookup"><span data-stu-id="b13a3-155">String</span></span>|<span data-ttu-id="b13a3-p107">Важность сообщения. Возможные значения: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="b13a3-p107">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="b13a3-158">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="b13a3-158">inferenceClassification</span></span> | <span data-ttu-id="b13a3-159">String</span><span class="sxs-lookup"><span data-stu-id="b13a3-159">String</span></span> | <span data-ttu-id="b13a3-p108">Классификация сообщения для пользователя на основании подразумеваемой релевантности или важности либо явного переопределения. Возможные значения: `focused` или `other`.</span><span class="sxs-lookup"><span data-stu-id="b13a3-p108">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="b13a3-162">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="b13a3-162">internetMessageId</span></span> |<span data-ttu-id="b13a3-163">String</span><span class="sxs-lookup"><span data-stu-id="b13a3-163">String</span></span> |<span data-ttu-id="b13a3-164">Идентификатор сообщения в формате, установленном документом [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span><span class="sxs-lookup"><span data-stu-id="b13a3-164">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="b13a3-165">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="b13a3-165">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="b13a3-166">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="b13a3-166">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="b13a3-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="b13a3-167">Boolean</span></span>|<span data-ttu-id="b13a3-168">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="b13a3-168">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="b13a3-169">isRead</span><span class="sxs-lookup"><span data-stu-id="b13a3-169">isRead</span></span>|<span data-ttu-id="b13a3-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="b13a3-170">Boolean</span></span>|<span data-ttu-id="b13a3-171">Указывает, прочитано ли сообщение.</span><span class="sxs-lookup"><span data-stu-id="b13a3-171">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="b13a3-172">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="b13a3-172">isReadReceiptRequested</span></span>|<span data-ttu-id="b13a3-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="b13a3-173">Boolean</span></span>|<span data-ttu-id="b13a3-174">Указывает, запрашивается ли уведомление о прочтении сообщения.</span><span class="sxs-lookup"><span data-stu-id="b13a3-174">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="b13a3-175">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b13a3-175">multiValueExtendedProperties</span></span>|<span data-ttu-id="b13a3-176">Коллекция [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="b13a3-176">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="b13a3-177">Коллекция многозначных расширенных свойств, определенных для сообщения.</span><span class="sxs-lookup"><span data-stu-id="b13a3-177">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="b13a3-178">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b13a3-178">Nullable.</span></span>|
|<span data-ttu-id="b13a3-179">replyTo</span><span class="sxs-lookup"><span data-stu-id="b13a3-179">replyTo</span></span>|<span data-ttu-id="b13a3-180">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="b13a3-180">Recipient collection</span></span>|<span data-ttu-id="b13a3-181">Электронные адреса, которые необходимо использовать при ответе.</span><span class="sxs-lookup"><span data-stu-id="b13a3-181">The email addresses to use when replying.</span></span> <span data-ttu-id="b13a3-182">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="b13a3-182">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="b13a3-183">sender</span><span class="sxs-lookup"><span data-stu-id="b13a3-183">sender</span></span>|<span data-ttu-id="b13a3-184">Recipient</span><span class="sxs-lookup"><span data-stu-id="b13a3-184">Recipient</span></span>|<span data-ttu-id="b13a3-185">Учетная запись, которая фактически используется для создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="b13a3-185">The account that is actually used to generate the message.</span></span> <span data-ttu-id="b13a3-186">Обновляемые при отправке сообщения из [общего почтового ящика](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)или отправка сообщения [Делегирование](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="b13a3-186">Updatable when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="b13a3-187">В любом случае значение должно соответствовать фактически используемому почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="b13a3-187">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="b13a3-188">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b13a3-188">singleValueExtendedProperties</span></span>|<span data-ttu-id="b13a3-189">Коллекция [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="b13a3-189">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="b13a3-190">Коллекция однозначных расширенных свойств, определенных для сообщения.</span><span class="sxs-lookup"><span data-stu-id="b13a3-190">The collection of single-value extended properties defined for the message.</span></span> <span data-ttu-id="b13a3-191">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b13a3-191">Nullable.</span></span>|
|<span data-ttu-id="b13a3-192">subject</span><span class="sxs-lookup"><span data-stu-id="b13a3-192">subject</span></span>|<span data-ttu-id="b13a3-193">String</span><span class="sxs-lookup"><span data-stu-id="b13a3-193">String</span></span>|<span data-ttu-id="b13a3-194">Тема сообщения.</span><span class="sxs-lookup"><span data-stu-id="b13a3-194">The subject of the message.</span></span> <span data-ttu-id="b13a3-195">Обновляемые только если isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="b13a3-195">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="b13a3-196">toRecipients</span><span class="sxs-lookup"><span data-stu-id="b13a3-196">toRecipients</span></span>|<span data-ttu-id="b13a3-197">Коллекция объектов Recipient</span><span class="sxs-lookup"><span data-stu-id="b13a3-197">Recipient collection</span></span>|<span data-ttu-id="b13a3-198">Кому получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="b13a3-198">The To recipients for the message.</span></span> |

<span data-ttu-id="b13a3-199">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **message**.</span><span class="sxs-lookup"><span data-stu-id="b13a3-199">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="b13a3-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="b13a3-200">Response</span></span>

<span data-ttu-id="b13a3-201">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b13a3-201">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b13a3-202">Пример</span><span class="sxs-lookup"><span data-stu-id="b13a3-202">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b13a3-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="b13a3-203">Request</span></span>
<span data-ttu-id="b13a3-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b13a3-204">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="b13a3-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="b13a3-205">Response</span></span>
<span data-ttu-id="b13a3-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b13a3-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="b13a3-209">См. также</span><span class="sxs-lookup"><span data-stu-id="b13a3-209">See also</span></span>

- [<span data-ttu-id="b13a3-210">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="b13a3-210">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b13a3-211">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="b13a3-211">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="b13a3-212">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="b13a3-212">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
    "Error: /api-reference/beta/api/message-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
