---
title: Список сообщений
description: 'Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные"). '
localization_priority: Normal
doc_type: apiPageType
author: svpsiva
ms.prod: outlook
ms.openlocfilehash: 1e1eb885803d90fca401a6cd4dee6ef3d6a865e0
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844419"
---
# <a name="list-messages"></a><span data-ttu-id="cfcc0-103">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="cfcc0-103">List messages</span></span>

<span data-ttu-id="cfcc0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfcc0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfcc0-105">Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные").</span><span class="sxs-lookup"><span data-stu-id="cfcc0-105">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span> 

<span data-ttu-id="cfcc0-106">В зависимости от размера страницы и данных почтового ящика получение сообщений из почтового ящика может повлечь множество запросов.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-106">Depending on the page size and mailbox data, getting messages from a mailbox can incur multiple requests.</span></span> <span data-ttu-id="cfcc0-107">По умолчанию страница содержит 10 сообщений.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-107">The default page size is 10 messages.</span></span> <span data-ttu-id="cfcc0-108">Для получения следующей странице с сообщениями, просто примените весь URL-адрес, возвращаемый в `@odata.nextLink`, для другого запроса на получение сообщений.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-108">To get the next page of messages, simply apply the entire URL returned in `@odata.nextLink` to the next get-messages request.</span></span> <span data-ttu-id="cfcc0-109">Этот URL-адрес включает любые параметры запроса, которые указаны в первоначальном запросе.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-109">This URL includes any query parameters you may have specified in the initial request.</span></span> 

<span data-ttu-id="cfcc0-110">Не извлекайте значение `$skip` из URL-адреса `@odata.nextLink` для операций с ответами.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-110">Do not try to extract the `$skip` value from the `@odata.nextLink` URL to manipulate responses.</span></span> <span data-ttu-id="cfcc0-111">Данный API использует значение `$skip` для учета всех элементов, просмотренных в почтовом ящике пользователя, и возврата элементов типа сообщение на странице.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-111">This API uses the `$skip` value to keep count of all the items it has gone through in the user's mailbox to return a page of message-type items.</span></span> <span data-ttu-id="cfcc0-112">Таким образом, существует возможность, что даже в первоначальном ответе, значение `$skip` будет больше, чем размер страницы.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-112">It's therefore possible that even in the initial response, the `$skip` value is larger than the page size.</span></span> <span data-ttu-id="cfcc0-113">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="cfcc0-113">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="cfcc0-114">Вы можете отфильтровать сообщения и получить [](../resources/mention.md) только те сообщения, которые содержат упоминание во включенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-114">You can filter on the messages and get only those that include a [mention](../resources/mention.md) of the signed-in user.</span></span> <span data-ttu-id="cfcc0-115">См. [пример](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-115">See an [example](#request-2) below.</span></span> <span data-ttu-id="cfcc0-116">По умолчанию операция не возвращает свойство `GET /me/messages` **mentions.**</span><span class="sxs-lookup"><span data-stu-id="cfcc0-116">By default, the `GET /me/messages` operation does not return the **mentions** property.</span></span> <span data-ttu-id="cfcc0-117">Используйте параметр `$expand` запроса, [чтобы найти сведения о каждом упоминаемом в сообщении.](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message)</span><span class="sxs-lookup"><span data-stu-id="cfcc0-117">Use the `$expand` query parameter to [find details of each mention in a message](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message).</span></span>

<span data-ttu-id="cfcc0-118">Существует два сценария, когда приложение может получить сообщения из папки почты другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="cfcc0-118">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="cfcc0-119">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="cfcc0-119">If the app has application permissions, or,</span></span>
* <span data-ttu-id="cfcc0-120">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-120">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="cfcc0-121">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="cfcc0-121">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

> <span data-ttu-id="cfcc0-122">**Примечание** Необходимо учитывать [известную проблему](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams) с включением сообщений чата Microsoft Teams в ответ операции.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-122">**Note** Be aware of the [known issue](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams) that this operation includes Microsoft Teams chat messages in its response.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="cfcc0-123">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cfcc0-123">Permissions</span></span>
<span data-ttu-id="cfcc0-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfcc0-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfcc0-126">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cfcc0-126">Permission type</span></span>      | <span data-ttu-id="cfcc0-127">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cfcc0-127">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfcc0-128">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cfcc0-128">Delegated (work or school account)</span></span> | <span data-ttu-id="cfcc0-129">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfcc0-129">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="cfcc0-130">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cfcc0-130">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfcc0-131">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfcc0-131">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="cfcc0-132">Приложение</span><span class="sxs-lookup"><span data-stu-id="cfcc0-132">Application</span></span> | <span data-ttu-id="cfcc0-133">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfcc0-133">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfcc0-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cfcc0-134">HTTP request</span></span>

<span data-ttu-id="cfcc0-135">Для получения всех сообщений в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="cfcc0-135">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="cfcc0-136">Для получения сообщений из определенной папки в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="cfcc0-136">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

<span data-ttu-id="cfcc0-137">Чтобы получить все сообщения в почтовом ящике  пользователя, которые содержат упоминание пользователя:</span><span class="sxs-lookup"><span data-stu-id="cfcc0-137">To get all the messages in the user's mailbox that include a **mention** of the user:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=mentionsPreview/isMentioned eq true
GET /users/{id | userPrincipalName}/messages?$filter=mentionsPreview/isMentioned eq true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cfcc0-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cfcc0-138">Optional query parameters</span></span>
<span data-ttu-id="cfcc0-139">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-139">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="cfcc0-140">Вы можете использовать параметр `$filter` запроса в свойстве **mentionsPreview,** чтобы получить сообщения, в которых упоминается во время выполнения действия пользователя.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-140">You can use the `$filter` query parameter on the **mentionsPreview** property to get those messages that mention the signed-in user.</span></span>

### <a name="using-filter-and-orderby-in-the-same-query"></a><span data-ttu-id="cfcc0-141">Использование операторов filter и orderby в одном запросе</span><span class="sxs-lookup"><span data-stu-id="cfcc0-141">Using filter and orderby in the same query</span></span>
<span data-ttu-id="cfcc0-142">При использовании операторов `$filter` и `$orderby` в одном запросе на получение сообщений необходимо указать свойства, соблюдая указанные ниже условия.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-142">When using `$filter` and `$orderby` in the same query to get messages, make sure to specify properties in the following ways:</span></span>

1. <span data-ttu-id="cfcc0-143">Свойства, используемые в операторе `$orderby`, также должны использоваться в операторе `$filter`.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-143">Properties that appear in `$orderby` must also appear in `$filter`.</span></span> 
2. <span data-ttu-id="cfcc0-144">Свойства, используемые в операторе `$orderby`, представлены в том же порядке, что и для оператора `$filter`.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-144">Properties that appear in `$orderby` are in the same order as in `$filter`.</span></span>
3. <span data-ttu-id="cfcc0-145">Свойства, присутствующие в операторе `$orderby`, представлены в операторе `$filter` раньше всех остальных свойств.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-145">Properties that are present in `$orderby` appear in `$filter` before any properties that aren't.</span></span>

<span data-ttu-id="cfcc0-146">В противном случае возникнет следующая ошибка:</span><span class="sxs-lookup"><span data-stu-id="cfcc0-146">Failing to do this results in the following error:</span></span>

- <span data-ttu-id="cfcc0-147">Код ошибки: `InefficientFilter`</span><span class="sxs-lookup"><span data-stu-id="cfcc0-147">Error code: `InefficientFilter`</span></span>
- <span data-ttu-id="cfcc0-148">Сообщение об ошибке: `The restriction or sort order is too complex for this operation.`</span><span class="sxs-lookup"><span data-stu-id="cfcc0-148">Error message: `The restriction or sort order is too complex for this operation.`</span></span>

## <a name="request-headers"></a><span data-ttu-id="cfcc0-149">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cfcc0-149">Request headers</span></span>
| <span data-ttu-id="cfcc0-150">Имя</span><span class="sxs-lookup"><span data-stu-id="cfcc0-150">Name</span></span>       | <span data-ttu-id="cfcc0-151">Тип</span><span class="sxs-lookup"><span data-stu-id="cfcc0-151">Type</span></span> | <span data-ttu-id="cfcc0-152">Описание</span><span class="sxs-lookup"><span data-stu-id="cfcc0-152">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cfcc0-153">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfcc0-153">Authorization</span></span>  | <span data-ttu-id="cfcc0-154">string</span><span class="sxs-lookup"><span data-stu-id="cfcc0-154">string</span></span>  | <span data-ttu-id="cfcc0-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cfcc0-157">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="cfcc0-157">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="cfcc0-158">string</span><span class="sxs-lookup"><span data-stu-id="cfcc0-158">string</span></span> | <span data-ttu-id="cfcc0-159">Формат возвращаемых свойств **body** и **uniqueBody**.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-159">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="cfcc0-160">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="cfcc0-160">Values can be "text" or "html".</span></span> <span data-ttu-id="cfcc0-161">Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-161">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="cfcc0-162">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-162">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfcc0-163">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cfcc0-163">Request body</span></span>
<span data-ttu-id="cfcc0-164">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfcc0-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfcc0-165">Response</span></span>

<span data-ttu-id="cfcc0-166">В случае успеха этот метод возвращает код отклика и коллекцию `200 OK` объектов [сообщений](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-166">If successful, this method returns a `200 OK` response code and collection of [message](../resources/message.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfcc0-167">Пример</span><span class="sxs-lookup"><span data-stu-id="cfcc0-167">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="cfcc0-168">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="cfcc0-168">Request 1</span></span>
<span data-ttu-id="cfcc0-169">В первом примере по умолчанию возвращается 10 сообщений в почтовом ящике пользователя, выписав его.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-169">The first example gets the default, top 10 messages in the signed-in user's mailbox.</span></span> <span data-ttu-id="cfcc0-170">`$select` используется для получения подмножества свойств каждого сообщения в ответе.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-170">It uses `$select` to return a subset of the properties of each message in the response.</span></span> 

# <a name="http"></a>[<span data-ttu-id="cfcc0-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfcc0-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$select=sender,subject
```
# <a name="c"></a>[<span data-ttu-id="cfcc0-172">C#</span><span class="sxs-lookup"><span data-stu-id="cfcc0-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfcc0-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfcc0-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfcc0-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfcc0-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfcc0-175">Java</span><span class="sxs-lookup"><span data-stu-id="cfcc0-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="cfcc0-176">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="cfcc0-176">Response 1</span></span>
<span data-ttu-id="cfcc0-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-177">Here is an example of the response.</span></span> <span data-ttu-id="cfcc0-178">Чтобы получить следующую страницу с сообщениями, примените URL-адрес, возвращенный в `@odata.nextLink`, для последующего запроса GET.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-178">To get the next page of messages, apply the URL returned in `@odata.nextLink` to a subsequent GET request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages(sender,subject)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/messages?$select=sender%2csubject&$skip=14",
    "value": [
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAwR4Hg\"",
            "id": "AAMkAGUAAAwTW09AAA=",
            "subject": "You have late tasks!",
            "sender": {
                "emailAddress": {
                    "name": "Microsoft Planner",
                    "address": "noreply@Planner.Office365.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4D1e\"",
            "id": "AAMkAGUAAAq5QKlAAA=",
            "subject": "You have late tasks!",
            "sender": {
                "emailAddress": {
                    "name": "Microsoft Planner",
                    "address": "noreply@Planner.Office365.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4D0v\"",
            "id": "AAMkAGUAAAq5QKkAAA=",
            "subject": "Your Azure AD Identity Protection Weekly Digest",
            "sender": {
                "emailAddress": {
                    "name": "Microsoft Azure",
                    "address": "azure-noreply@microsoft.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4DsN\"",
            "id": "AAMkAGUAAAq5QKjAAA=",
            "subject": "Use attached file",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dq9\"",
            "id": "AAMkAGUAAAq5QKiAAA=",
            "subject": "Original invitation",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dq1\"",
            "id": "AAMkAGUAAAq5QKhAAA=",
            "subject": "Koala image",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dqp\"",
            "id": "AAMkAGUAAAq5QKgAAA=",
            "subject": "Sales invoice template",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.eventMessageRequest",
            "@odata.etag": "W/\"CwAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dfa\"",
            "id": "AAMkAGUAAAq5T8tAAA=",
            "subject": "Review strategy for Q3",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        }
    ]
}
```


##### <a name="request-2"></a><span data-ttu-id="cfcc0-179">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="cfcc0-179">Request 2</span></span>
<span data-ttu-id="cfcc0-180">В следующем примере фильтруются все сообщения в почтовом ящике пользователя, выписав его.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-180">The next example filters all messages in the signed-in user's mailbox for those that mention the user.</span></span> <span data-ttu-id="cfcc0-181">Он также использует для возврата подмножество свойств каждого `$select` сообщения в ответе.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-181">It also uses `$select` to return a subset of the properties of each message in the response.</span></span> 

<span data-ttu-id="cfcc0-182">В пример также включена кодивка URL-адресов для пробелов в строке параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-182">The example also incorporates URL encoding for the space characters in the query parameter string.</span></span>

# <a name="http"></a>[<span data-ttu-id="cfcc0-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfcc0-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_with_mentions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$filter=MentionsPreview/IsMentioned%20eq%20true&$select=Subject,Sender,ReceivedDateTime,MentionsPreview
```
# <a name="c"></a>[<span data-ttu-id="cfcc0-184">C#</span><span class="sxs-lookup"><span data-stu-id="cfcc0-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfcc0-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfcc0-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfcc0-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfcc0-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfcc0-187">Java</span><span class="sxs-lookup"><span data-stu-id="cfcc0-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-with-mentions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="cfcc0-188">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="cfcc0-188">Response 2</span></span>
<span data-ttu-id="cfcc0-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 987

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages(subject,sender,receivedDateTime,mentionsPreview)",
  "value":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAATI\"",
      "id":"AQMkADJmMTUAAAgVZAAAA",
      "receivedDateTime":"2016-07-21T07:40:21Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Randi Welch",
          "address":"randiw@contoso.onmicrosoft.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    },
    {
      "@odata.id":"https://graph.microsoft.com/beta/Users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/Messages('AQMkADJmMTUAAAjwVAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAEGj\"",
      "id":"AQMkADJmMTUAAAjwVAAAA",
      "receivedDateTime":"2016-07-21T07:40:20Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Randi Welch",
          "address":"randiw@contoso.onmicrosoft.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    }
  ]
}
```

##### <a name="request-3"></a><span data-ttu-id="cfcc0-192">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="cfcc0-192">Request 3</span></span>
<span data-ttu-id="cfcc0-193">В третьем примере показано, как использовать заголовщик для получения текста и свойств `Prefer: outlook.body-content-type="text"` **uniqueBody** каждого сообщения  в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-193">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** properties of each message in text format.</span></span>

# <a name="http"></a>[<span data-ttu-id="cfcc0-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfcc0-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[<span data-ttu-id="cfcc0-195">C#</span><span class="sxs-lookup"><span data-stu-id="cfcc0-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfcc0-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfcc0-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfcc0-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfcc0-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfcc0-198">Java</span><span class="sxs-lookup"><span data-stu-id="cfcc0-198">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-3"></a><span data-ttu-id="cfcc0-199">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="cfcc0-199">Response 3</span></span>
<span data-ttu-id="cfcc0-200">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cfcc0-200">Here is an example of the response.</span></span> 

<!--
Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.
-->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2704

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)",
    "value":[
        {
            "@odata.type":"#microsoft.graph.eventMessageRequest",
            "@odata.etag":"W/\"CwAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj5\"",
            "id":"AAMkAGIAAAoZCfIAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            }
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
            "id":"AAMkAGIAAAoZCfHAAA=",
            "subject":"Welcome to our group!",
            "bodyPreview":"Welcome to our group, Dana! Hope you will enjoy working with us !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nTh",
            "body":{
                "contentType":"text",
                "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nThanks!\r\n\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\nThanks!\r\n"
            }
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAAAAjr\"",
            "id":"AQMkAGIAAAIJTQAAAA==",
            "subject":"Welcome aboard!",
            "bodyPreview":"Welcome to the Support group!",
            "body":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
