---
title: Список сообщений
description: Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные").
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 67e201d14cdae4ada4ccca8160822ace5793c099
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509061"
---
# <a name="list-messages"></a><span data-ttu-id="691f1-103">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="691f1-103">List messages</span></span>

<span data-ttu-id="691f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="691f1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="691f1-105">Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные").</span><span class="sxs-lookup"><span data-stu-id="691f1-105">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="691f1-106">В зависимости от размера страницы и данных почтового ящика получение сообщений из почтового ящика может повлечь множество запросов.</span><span class="sxs-lookup"><span data-stu-id="691f1-106">Depending on the page size and mailbox data, getting messages from a mailbox can incur multiple requests.</span></span> <span data-ttu-id="691f1-107">По умолчанию страница содержит 10 сообщений.</span><span class="sxs-lookup"><span data-stu-id="691f1-107">The default page size is 10 messages.</span></span> <span data-ttu-id="691f1-108">Для получения следующей странице с сообщениями, просто примените весь URL-адрес, возвращаемый в `@odata.nextLink`, для другого запроса на получение сообщений.</span><span class="sxs-lookup"><span data-stu-id="691f1-108">To get the next page of messages, simply apply the entire URL returned in `@odata.nextLink` to the next get-messages request.</span></span> <span data-ttu-id="691f1-109">Этот URL-адрес включает любые параметры запроса, которые указаны в первоначальном запросе.</span><span class="sxs-lookup"><span data-stu-id="691f1-109">This URL includes any query parameters you may have specified in the initial request.</span></span> 

<span data-ttu-id="691f1-110">Не извлекайте значение `$skip` из URL-адреса `@odata.nextLink` для операций с ответами.</span><span class="sxs-lookup"><span data-stu-id="691f1-110">Do not try to extract the `$skip` value from the `@odata.nextLink` URL to manipulate responses.</span></span> <span data-ttu-id="691f1-111">Данный API использует значение `$skip` для учета всех элементов, просмотренных в почтовом ящике пользователя, и возврата элементов типа сообщение на странице.</span><span class="sxs-lookup"><span data-stu-id="691f1-111">This API uses the `$skip` value to keep count of all the items it has gone through in the user's mailbox to return a page of message-type items.</span></span> <span data-ttu-id="691f1-112">Таким образом, существует возможность, что даже в первоначальном ответе, значение `$skip` будет больше, чем размер страницы.</span><span class="sxs-lookup"><span data-stu-id="691f1-112">It's therefore possible that even in the initial response, the `$skip` value is larger than the page size.</span></span> <span data-ttu-id="691f1-113">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="691f1-113">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="691f1-114">В настоящее время эта операция возвращает текст сообщения только в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="691f1-114">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="691f1-115">Существует два сценария, когда приложение может получить сообщения из папки почты другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="691f1-115">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="691f1-116">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="691f1-116">If the app has application permissions, or,</span></span>
* <span data-ttu-id="691f1-117">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="691f1-117">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="691f1-118">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="691f1-118">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

## <a name="permissions"></a><span data-ttu-id="691f1-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="691f1-119">Permissions</span></span>
<span data-ttu-id="691f1-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="691f1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="691f1-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="691f1-122">Permission type</span></span>      | <span data-ttu-id="691f1-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="691f1-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="691f1-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="691f1-124">Delegated (work or school account)</span></span> | <span data-ttu-id="691f1-125">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="691f1-125">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="691f1-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="691f1-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="691f1-127">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="691f1-127">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="691f1-128">Для приложения</span><span class="sxs-lookup"><span data-stu-id="691f1-128">Application</span></span> | <span data-ttu-id="691f1-129">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="691f1-129">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="691f1-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="691f1-130">HTTP request</span></span>

<span data-ttu-id="691f1-131">Для получения всех сообщений в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="691f1-131">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="691f1-132">Для получения сообщений из определенной папки в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="691f1-132">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="691f1-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="691f1-133">Optional query parameters</span></span>
<span data-ttu-id="691f1-134">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="691f1-134">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

### <a name="using-filter-and-orderby-in-the-same-query"></a><span data-ttu-id="691f1-135">Использование операторов filter и orderby в одном запросе</span><span class="sxs-lookup"><span data-stu-id="691f1-135">Using filter and orderby in the same query</span></span>
<span data-ttu-id="691f1-136">При использовании операторов `$filter` и `$orderby` в одном запросе на получение сообщений необходимо указать свойства, соблюдая указанные ниже условия.</span><span class="sxs-lookup"><span data-stu-id="691f1-136">When using `$filter` and `$orderby` in the same query to get messages, make sure to specify properties in the following ways:</span></span>

1. <span data-ttu-id="691f1-137">Свойства, используемые в операторе `$orderby`, также должны использоваться в операторе `$filter`.</span><span class="sxs-lookup"><span data-stu-id="691f1-137">Properties that appear in `$orderby` must also appear in `$filter`.</span></span> 
2. <span data-ttu-id="691f1-138">Свойства, используемые в операторе `$orderby`, представлены в том же порядке, что и для оператора `$filter`.</span><span class="sxs-lookup"><span data-stu-id="691f1-138">Properties that appear in `$orderby` are in the same order as in `$filter`.</span></span>
3. <span data-ttu-id="691f1-139">Свойства, присутствующие в операторе `$orderby`, представлены в операторе `$filter` раньше всех остальных свойств.</span><span class="sxs-lookup"><span data-stu-id="691f1-139">Properties that are present in `$orderby` appear in `$filter` before any properties that aren't.</span></span>

<span data-ttu-id="691f1-140">В противном случае возникнет следующая ошибка:</span><span class="sxs-lookup"><span data-stu-id="691f1-140">Failing to do this results in the following error:</span></span>

- <span data-ttu-id="691f1-141">Код ошибки: `InefficientFilter`</span><span class="sxs-lookup"><span data-stu-id="691f1-141">Error code: `InefficientFilter`</span></span>
- <span data-ttu-id="691f1-142">Сообщение об ошибке: `The restriction or sort order is too complex for this operation.`</span><span class="sxs-lookup"><span data-stu-id="691f1-142">Error message: `The restriction or sort order is too complex for this operation.`</span></span>

## <a name="request-headers"></a><span data-ttu-id="691f1-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="691f1-143">Request headers</span></span>
| <span data-ttu-id="691f1-144">Имя</span><span class="sxs-lookup"><span data-stu-id="691f1-144">Name</span></span>       | <span data-ttu-id="691f1-145">Тип</span><span class="sxs-lookup"><span data-stu-id="691f1-145">Type</span></span> | <span data-ttu-id="691f1-146">Описание</span><span class="sxs-lookup"><span data-stu-id="691f1-146">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="691f1-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="691f1-147">Authorization</span></span>  | <span data-ttu-id="691f1-148">string</span><span class="sxs-lookup"><span data-stu-id="691f1-148">string</span></span>  | <span data-ttu-id="691f1-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="691f1-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="691f1-151">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="691f1-151">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="691f1-152">string</span><span class="sxs-lookup"><span data-stu-id="691f1-152">string</span></span> | <span data-ttu-id="691f1-153">Формат возвращаемых свойств **body** и **uniqueBody**.</span><span class="sxs-lookup"><span data-stu-id="691f1-153">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="691f1-154">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="691f1-154">Values can be "text" or "html".</span></span> <span data-ttu-id="691f1-155">Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="691f1-155">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="691f1-156">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="691f1-156">Optional.</span></span> |


## <a name="request-body"></a><span data-ttu-id="691f1-157">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="691f1-157">Request body</span></span>
<span data-ttu-id="691f1-158">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="691f1-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="691f1-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="691f1-159">Response</span></span>

<span data-ttu-id="691f1-160">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="691f1-160">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="691f1-161">Пример</span><span class="sxs-lookup"><span data-stu-id="691f1-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="691f1-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="691f1-162">Request</span></span>
<span data-ttu-id="691f1-163">Данный пример получает по умолчанию 10 верхних сообщений в почтовом ящике выполнившего вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="691f1-163">This example gets the default, top 10 messages in the signed-in user's mailbox.</span></span> <span data-ttu-id="691f1-164">`$select` используется для получения подмножества свойств каждого сообщения в ответе.</span><span class="sxs-lookup"><span data-stu-id="691f1-164">It uses `$select` to return a subset of the properties of each message in the response.</span></span>

# <a name="http"></a>[<span data-ttu-id="691f1-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="691f1-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$select=sender,subject
```
# <a name="c"></a>[<span data-ttu-id="691f1-166">C#</span><span class="sxs-lookup"><span data-stu-id="691f1-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="691f1-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="691f1-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="691f1-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="691f1-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="691f1-169">Java</span><span class="sxs-lookup"><span data-stu-id="691f1-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="691f1-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="691f1-170">Response</span></span>
<span data-ttu-id="691f1-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="691f1-171">Here is an example of the response.</span></span> <span data-ttu-id="691f1-172">Чтобы получить следующую страницу с сообщениями, примените URL-адрес, возвращенный в `@odata.nextLink`, для последующего запроса GET.</span><span class="sxs-lookup"><span data-stu-id="691f1-172">To get the next page of messages, apply the URL returned in `@odata.nextLink` to a subsequent GET request.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages(sender,subject)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$select=sender%2csubject&$skip=14",
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
            "@odata.type": "#microsoft.graph.eventMessage",
            "@odata.etag": "W/\"DAAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dft\"",
            "id": "AAMkAGUAAAq5UMVAAA=",
            "subject": "Accepted: Review strategy for Q3",
            "sender": {
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "/O=EXCHANGELABS/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=A17A02BCF30C4937A87B14273385667C-ADELEV"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.eventMessage",
            "@odata.etag": "W/\"DAAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4DfF\"",
            "id": "AAMkAGUAAAq5UMUAAA=",
            "subject": "Accepted: Review strategy for Q3",
            "sender": {
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "/O=EXCHANGELABS/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=A17A02BCF30C4937A87B14273385667C-ADELEV"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.eventMessage",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
