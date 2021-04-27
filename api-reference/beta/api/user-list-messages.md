---
title: Список сообщений
description: 'Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные"). '
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: outlook
ms.openlocfilehash: 24083f158863077d6dcb6b2af55a2a16db1e83e7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052616"
---
# <a name="list-messages"></a><span data-ttu-id="bcc3d-103">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="bcc3d-103">List messages</span></span>

<span data-ttu-id="bcc3d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcc3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcc3d-105">Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные").</span><span class="sxs-lookup"><span data-stu-id="bcc3d-105">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span> 

<span data-ttu-id="bcc3d-106">В зависимости от размера страницы и данных почтового ящика получение сообщений из почтового ящика может повлечь множество запросов.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-106">Depending on the page size and mailbox data, getting messages from a mailbox can incur multiple requests.</span></span> <span data-ttu-id="bcc3d-107">По умолчанию страница содержит 10 сообщений.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-107">The default page size is 10 messages.</span></span> <span data-ttu-id="bcc3d-108">Используйте параметр `$top`, чтобы настроить размер страницы в диапазоне от 1 до 1000.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-108">Use `$top` to customize the page size, within the range of 1 and 1000.</span></span>

<span data-ttu-id="bcc3d-109">Чтобы сократить время отклика, используйте параметр `$select` для указания точных свойств, которые вам нужны. См. [пример 1](#example-1-list-all-messages) ниже.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-109">To improve the operation response time, use `$select` to specify the exact properties you need; see [example 1](#example-1-list-all-messages) below.</span></span> <span data-ttu-id="bcc3d-110">Настройте значения для `$select` и `$top`, особенно при необходимости использовании большего размера страницы, так как возврат страницы с сотнями сообщений, каждое из которых содержит полные полезные данные отклика, может привести к [истечению времени ожидания шлюза](/graph/errors#http-status-codes) (HTTP 504).</span><span class="sxs-lookup"><span data-stu-id="bcc3d-110">Fine-tune the values for `$select` and `$top`, especially when you must use a larger page size, as returning a page with hundreds of messages each with a full response payload may trigger the [gateway timeout](/graph/errors#http-status-codes) (HTTP 504).</span></span>

<span data-ttu-id="bcc3d-111">Для получения следующей странице с сообщениями, просто примените весь URL-адрес, возвращаемый в `@odata.nextLink`, для другого запроса на получение сообщений.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-111">To get the next page of messages, simply apply the entire URL returned in `@odata.nextLink` to the next get-messages request.</span></span> <span data-ttu-id="bcc3d-112">Этот URL-адрес включает любые параметры запроса, которые указаны в первоначальном запросе.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-112">This URL includes any query parameters you may have specified in the initial request.</span></span> 

<span data-ttu-id="bcc3d-113">Не извлекайте значение `$skip` из URL-адреса `@odata.nextLink` для операций с ответами.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-113">Do not try to extract the `$skip` value from the `@odata.nextLink` URL to manipulate responses.</span></span> <span data-ttu-id="bcc3d-114">Данный API использует значение `$skip` для учета всех элементов, просмотренных в почтовом ящике пользователя, и возврата элементов типа сообщение на странице.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-114">This API uses the `$skip` value to keep count of all the items it has gone through in the user's mailbox to return a page of message-type items.</span></span> <span data-ttu-id="bcc3d-115">Таким образом, существует возможность, что даже в первоначальном ответе, значение `$skip` будет больше, чем размер страницы.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-115">It's therefore possible that even in the initial response, the `$skip` value is larger than the page size.</span></span> <span data-ttu-id="bcc3d-116">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="bcc3d-116">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="bcc3d-117">Вы можете фильтровать сообщения и получать только те, которые включают [упоминание](../resources/mention.md) пользователя, включаемого в него.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-117">You can filter on the messages and get only those that include a [mention](../resources/mention.md) of the signed-in user.</span></span> <span data-ttu-id="bcc3d-118">См. [пример](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-118">See an [example](#request-2) below.</span></span> <span data-ttu-id="bcc3d-119">По умолчанию операция не возвращает свойство `GET /me/messages` **упоминаний.**</span><span class="sxs-lookup"><span data-stu-id="bcc3d-119">By default, the `GET /me/messages` operation does not return the **mentions** property.</span></span> <span data-ttu-id="bcc3d-120">Используйте параметр `$expand` запроса, [чтобы найти сведения о каждом упоминаемом сообщении.](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message)</span><span class="sxs-lookup"><span data-stu-id="bcc3d-120">Use the `$expand` query parameter to [find details of each mention in a message](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message).</span></span>

<span data-ttu-id="bcc3d-121">Существует два сценария, когда приложение может получить сообщения из папки почты другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="bcc3d-121">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="bcc3d-122">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="bcc3d-122">If the app has application permissions, or,</span></span>
* <span data-ttu-id="bcc3d-123">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-123">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="bcc3d-124">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="bcc3d-124">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

> <span data-ttu-id="bcc3d-125">**Примечание** Необходимо учитывать [известную проблему](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams) с включением сообщений чата Microsoft Teams в ответ операции.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-125">**Note** Be aware of the [known issue](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams) that this operation includes Microsoft Teams chat messages in its response.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="bcc3d-126">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bcc3d-126">Permissions</span></span>
<span data-ttu-id="bcc3d-p107">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcc3d-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcc3d-129">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcc3d-129">Permission type</span></span>      | <span data-ttu-id="bcc3d-130">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcc3d-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcc3d-131">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcc3d-131">Delegated (work or school account)</span></span> | <span data-ttu-id="bcc3d-132">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcc3d-132">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bcc3d-133">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcc3d-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcc3d-134">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcc3d-134">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bcc3d-135">Приложение</span><span class="sxs-lookup"><span data-stu-id="bcc3d-135">Application</span></span> | <span data-ttu-id="bcc3d-136">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcc3d-136">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcc3d-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcc3d-137">HTTP request</span></span>

<span data-ttu-id="bcc3d-138">Для получения всех сообщений в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="bcc3d-138">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="bcc3d-139">Для получения сообщений из определенной папки в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="bcc3d-139">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

<span data-ttu-id="bcc3d-140">Чтобы получить все сообщения в почтовом ящике пользователя с **упоминанием** пользователя:</span><span class="sxs-lookup"><span data-stu-id="bcc3d-140">To get all the messages in the user's mailbox that include a **mention** of the user:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=mentionsPreview/isMentioned eq true
GET /users/{id | userPrincipalName}/messages?$filter=mentionsPreview/isMentioned eq true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bcc3d-141">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bcc3d-141">Optional query parameters</span></span>
<span data-ttu-id="bcc3d-142">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-142">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="bcc3d-143">Параметр запроса `$filter` в свойстве **mentionsPreview** можно использовать для получения сообщений, в которых упоминается пользователь, вписав его.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-143">You can use the `$filter` query parameter on the **mentionsPreview** property to get those messages that mention the signed-in user.</span></span>

### <a name="using-filter-and-orderby-in-the-same-query"></a><span data-ttu-id="bcc3d-144">Использование операторов filter и orderby в одном запросе</span><span class="sxs-lookup"><span data-stu-id="bcc3d-144">Using filter and orderby in the same query</span></span>
<span data-ttu-id="bcc3d-145">При использовании операторов `$filter` и `$orderby` в одном запросе на получение сообщений необходимо указать свойства, соблюдая указанные ниже условия.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-145">When using `$filter` and `$orderby` in the same query to get messages, make sure to specify properties in the following ways:</span></span>

1. <span data-ttu-id="bcc3d-146">Свойства, используемые в операторе `$orderby`, также должны использоваться в операторе `$filter`.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-146">Properties that appear in `$orderby` must also appear in `$filter`.</span></span> 
2. <span data-ttu-id="bcc3d-147">Свойства, используемые в операторе `$orderby`, представлены в том же порядке, что и для оператора `$filter`.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-147">Properties that appear in `$orderby` are in the same order as in `$filter`.</span></span>
3. <span data-ttu-id="bcc3d-148">Свойства, присутствующие в операторе `$orderby`, представлены в операторе `$filter` раньше всех остальных свойств.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-148">Properties that are present in `$orderby` appear in `$filter` before any properties that aren't.</span></span>

<span data-ttu-id="bcc3d-149">В противном случае возникнет следующая ошибка:</span><span class="sxs-lookup"><span data-stu-id="bcc3d-149">Failing to do this results in the following error:</span></span>

- <span data-ttu-id="bcc3d-150">Код ошибки: `InefficientFilter`</span><span class="sxs-lookup"><span data-stu-id="bcc3d-150">Error code: `InefficientFilter`</span></span>
- <span data-ttu-id="bcc3d-151">Сообщение об ошибке: `The restriction or sort order is too complex for this operation.`</span><span class="sxs-lookup"><span data-stu-id="bcc3d-151">Error message: `The restriction or sort order is too complex for this operation.`</span></span>

## <a name="request-headers"></a><span data-ttu-id="bcc3d-152">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcc3d-152">Request headers</span></span>
| <span data-ttu-id="bcc3d-153">Имя</span><span class="sxs-lookup"><span data-stu-id="bcc3d-153">Name</span></span>       | <span data-ttu-id="bcc3d-154">Тип</span><span class="sxs-lookup"><span data-stu-id="bcc3d-154">Type</span></span> | <span data-ttu-id="bcc3d-155">Описание</span><span class="sxs-lookup"><span data-stu-id="bcc3d-155">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bcc3d-156">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcc3d-156">Authorization</span></span>  | <span data-ttu-id="bcc3d-157">string</span><span class="sxs-lookup"><span data-stu-id="bcc3d-157">string</span></span>  | <span data-ttu-id="bcc3d-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-p108">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bcc3d-160">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="bcc3d-160">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="bcc3d-161">string</span><span class="sxs-lookup"><span data-stu-id="bcc3d-161">string</span></span> | <span data-ttu-id="bcc3d-162">Формат возвращаемых свойств **body** и **uniqueBody**.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-162">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="bcc3d-163">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="bcc3d-163">Values can be "text" or "html".</span></span> <span data-ttu-id="bcc3d-164">Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-164">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="bcc3d-165">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-165">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bcc3d-166">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bcc3d-166">Request body</span></span>
<span data-ttu-id="bcc3d-167">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-167">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcc3d-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcc3d-168">Response</span></span>

<span data-ttu-id="bcc3d-169">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` сообщений в тексте [](../resources/message.md) отклика.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-169">If successful, this method returns a `200 OK` response code and collection of [message](../resources/message.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bcc3d-170">Примеры</span><span class="sxs-lookup"><span data-stu-id="bcc3d-170">Examples</span></span>
### <a name="example-1-list-all-messages"></a><span data-ttu-id="bcc3d-171">Пример 1. Перечисление всех сообщений</span><span class="sxs-lookup"><span data-stu-id="bcc3d-171">Example 1: List all messages</span></span>
#### <a name="request"></a><span data-ttu-id="bcc3d-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcc3d-172">Request</span></span>
<span data-ttu-id="bcc3d-173">В первом примере получается по умолчанию, топ-10 сообщений в почтовом ящике подписанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-173">The first example gets the default, top 10 messages in the signed-in user's mailbox.</span></span> <span data-ttu-id="bcc3d-174">`$select` используется для получения подмножества свойств каждого сообщения в ответе.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-174">It uses `$select` to return a subset of the properties of each message in the response.</span></span> 

# <a name="http"></a>[<span data-ttu-id="bcc3d-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcc3d-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$select=sender,subject
```
# <a name="c"></a>[<span data-ttu-id="bcc3d-176">C#</span><span class="sxs-lookup"><span data-stu-id="bcc3d-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bcc3d-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcc3d-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bcc3d-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcc3d-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bcc3d-179">Java</span><span class="sxs-lookup"><span data-stu-id="bcc3d-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="bcc3d-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcc3d-180">Response</span></span>
<span data-ttu-id="bcc3d-181">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-181">Here is an example of the response.</span></span> <span data-ttu-id="bcc3d-182">Чтобы получить следующую страницу с сообщениями, примените URL-адрес, возвращенный в `@odata.nextLink`, для последующего запроса GET.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-182">To get the next page of messages, apply the URL returned in `@odata.nextLink` to a subsequent GET request.</span></span>

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
    }
  ]
}
```

### <a name="example-2-use-filter-to-get-all-messages-satisfying-a-specific-condition"></a><span data-ttu-id="bcc3d-183">Пример 2. Использование $filter для получения всех сообщений, удовлетворяющих определенному условию</span><span class="sxs-lookup"><span data-stu-id="bcc3d-183">Example 2: Use $filter to get all messages satisfying a specific condition</span></span>
#### <a name="request"></a><span data-ttu-id="bcc3d-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcc3d-184">Request</span></span>
<span data-ttu-id="bcc3d-185">В следующем примере фильтруются все сообщения в почтовом ящике подписанного пользователя для тех, кто упоминает пользователя.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-185">The next example filters all messages in the signed-in user's mailbox for those that mention the user.</span></span> <span data-ttu-id="bcc3d-186">Он также `$select` использует для возврата подмножество свойств каждого сообщения в ответе.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-186">It also uses `$select` to return a subset of the properties of each message in the response.</span></span> 

<span data-ttu-id="bcc3d-187">В примере также включается кодить URL-адрес для символов пространства в строке параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-187">The example also incorporates URL encoding for the space characters in the query parameter string.</span></span>

# <a name="http"></a>[<span data-ttu-id="bcc3d-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcc3d-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_with_mentions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$filter=MentionsPreview/IsMentioned%20eq%20true&$select=Subject,Sender,ReceivedDateTime,MentionsPreview
```
# <a name="c"></a>[<span data-ttu-id="bcc3d-189">C#</span><span class="sxs-lookup"><span data-stu-id="bcc3d-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bcc3d-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcc3d-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bcc3d-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcc3d-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bcc3d-192">Java</span><span class="sxs-lookup"><span data-stu-id="bcc3d-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-with-mentions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="bcc3d-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcc3d-193">Response</span></span>
<span data-ttu-id="bcc3d-194">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-194">Here is an example of the response.</span></span> <span data-ttu-id="bcc3d-195">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-195">Note: The response object shown here might be shortened for readability.</span></span>
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
          "name":"Adele Vance",
          "address":"AdeleV@contoso.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    }
  ]
}
```

### <a name="example-3-use-prefer-header-to-get-the-message-body-and-uniquebody-is-text-format"></a><span data-ttu-id="bcc3d-196">Пример 3. Используйте предпочитаемую заголовка, чтобы получить тело сообщения, а uniqueBody — текстовый формат</span><span class="sxs-lookup"><span data-stu-id="bcc3d-196">Example 3: Use prefer header to get the message body and uniqueBody is text format</span></span>
#### <a name="request"></a><span data-ttu-id="bcc3d-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcc3d-197">Request</span></span>
<span data-ttu-id="bcc3d-198">В третьем примере показано, как использовать заголовка для получения тела и уникальных свойств каждого сообщения в `Prefer: outlook.body-content-type="text"` текстовом  формате. </span><span class="sxs-lookup"><span data-stu-id="bcc3d-198">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** properties of each message in text format.</span></span>

# <a name="http"></a>[<span data-ttu-id="bcc3d-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcc3d-199">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[<span data-ttu-id="bcc3d-200">C#</span><span class="sxs-lookup"><span data-stu-id="bcc3d-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bcc3d-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcc3d-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bcc3d-202">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcc3d-202">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bcc3d-203">Java</span><span class="sxs-lookup"><span data-stu-id="bcc3d-203">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="bcc3d-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcc3d-204">Response</span></span>
<span data-ttu-id="bcc3d-205">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bcc3d-205">Here is an example of the response.</span></span> 

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
