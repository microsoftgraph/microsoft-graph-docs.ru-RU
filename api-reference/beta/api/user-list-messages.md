---
title: Список сообщений
description: 'Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные"). '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: fae97e9188f4069829cf066539fb9425efc3788b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270086"
---
# <a name="list-messages"></a><span data-ttu-id="fef18-103">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="fef18-103">List messages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fef18-104">Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные").</span><span class="sxs-lookup"><span data-stu-id="fef18-104">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span> 

<span data-ttu-id="fef18-105">В зависимости от размера страницы и данных почтового ящика получение сообщений из почтового ящика может повлечь множество запросов.</span><span class="sxs-lookup"><span data-stu-id="fef18-105">Depending on the page size and mailbox data, getting messages from a mailbox can incur multiple requests.</span></span> <span data-ttu-id="fef18-106">По умолчанию страница содержит 10 сообщений.</span><span class="sxs-lookup"><span data-stu-id="fef18-106">The default page size is 10 messages.</span></span> <span data-ttu-id="fef18-107">Для получения следующей странице с сообщениями, просто примените весь URL-адрес, возвращаемый в `@odata.nextLink`, для другого запроса на получение сообщений.</span><span class="sxs-lookup"><span data-stu-id="fef18-107">To get the next page of messages, simply apply the entire URL returned in `@odata.nextLink` to the next get-messages request.</span></span> <span data-ttu-id="fef18-108">Этот URL-адрес включает любые параметры запроса, которые указаны в первоначальном запросе.</span><span class="sxs-lookup"><span data-stu-id="fef18-108">This URL includes any query parameters you may have specified in the initial request.</span></span> 

<span data-ttu-id="fef18-109">Не извлекайте значение `$skip` из URL-адреса `@odata.nextLink` для операций с ответами.</span><span class="sxs-lookup"><span data-stu-id="fef18-109">Do not try to extract the `$skip` value from the `@odata.nextLink` URL to manipulate responses.</span></span> <span data-ttu-id="fef18-110">Данный API использует значение `$skip` для учета всех элементов, просмотренных в почтовом ящике пользователя, и возврата элементов типа сообщение на странице.</span><span class="sxs-lookup"><span data-stu-id="fef18-110">This API uses the `$skip` value to keep count of all the items it has gone through in the user's mailbox to return a page of message-type items.</span></span> <span data-ttu-id="fef18-111">Таким образом, существует возможность, что даже в первоначальном ответе, значение `$skip` будет больше, чем размер страницы.</span><span class="sxs-lookup"><span data-stu-id="fef18-111">It's therefore possible that even in the initial response, the `$skip` value is larger than the page size.</span></span> <span data-ttu-id="fef18-112">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="fef18-112">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="fef18-113">Вы можете фильтровать сообщения и получать только те сообщения, которые содержат [упоминание](../resources/mention.md) пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="fef18-113">You can filter on the messages and get only those that include a [mention](../resources/mention.md) of the signed-in user.</span></span>

<span data-ttu-id="fef18-114">Обратите внимание, что по `GET /me/messages` умолчанию операция не возвращает свойство **упоминания** .</span><span class="sxs-lookup"><span data-stu-id="fef18-114">Note that by default, the `GET /me/messages` operation does not return the **mentions** property.</span></span> <span data-ttu-id="fef18-115">Используйте параметр `$expand` запроса для [получения сведений о каждом упоминании в сообщении](../api/message-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="fef18-115">Use the `$expand` query parameter to [find details of each mention in a message](../api/message-get.md#request-2).</span></span>

<span data-ttu-id="fef18-116">Существует два сценария, когда приложение может получить сообщения из папки почты другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="fef18-116">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="fef18-117">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="fef18-117">If the app has application permissions, or,</span></span>
* <span data-ttu-id="fef18-118">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="fef18-118">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="fef18-119">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="fef18-119">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="fef18-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fef18-120">Permissions</span></span>
<span data-ttu-id="fef18-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fef18-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fef18-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fef18-123">Permission type</span></span>      | <span data-ttu-id="fef18-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fef18-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fef18-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fef18-125">Delegated (work or school account)</span></span> | <span data-ttu-id="fef18-126">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fef18-126">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fef18-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fef18-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fef18-128">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fef18-128">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fef18-129">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fef18-129">Application</span></span> | <span data-ttu-id="fef18-130">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fef18-130">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fef18-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fef18-131">HTTP request</span></span>

<span data-ttu-id="fef18-132">Для получения всех сообщений в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="fef18-132">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="fef18-133">Для получения сообщений из определенной папки в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="fef18-133">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

<span data-ttu-id="fef18-134">Для получения всех сообщений в почтовом ящике пользователя, содержащих **упоминание** пользователя:</span><span class="sxs-lookup"><span data-stu-id="fef18-134">To get all the messages in the user's mailbox that include a **mention** of the user:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=mentionsPreview/isMentioned eq true
GET /users/{id | userPrincipalName}/messages?$filter=mentionsPreview/isMentioned eq true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fef18-135">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fef18-135">Optional query parameters</span></span>
<span data-ttu-id="fef18-136">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fef18-136">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="fef18-137">Вы можете использовать параметр `$filter` запроса для свойства **ментионспревиев** , чтобы получить такие сообщения, которые упоминают пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="fef18-137">You can use the `$filter` query parameter on the **mentionsPreview** property to get those messages that mention the signed-in user.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fef18-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fef18-138">Request headers</span></span>
| <span data-ttu-id="fef18-139">Имя</span><span class="sxs-lookup"><span data-stu-id="fef18-139">Name</span></span>       | <span data-ttu-id="fef18-140">Тип</span><span class="sxs-lookup"><span data-stu-id="fef18-140">Type</span></span> | <span data-ttu-id="fef18-141">Описание</span><span class="sxs-lookup"><span data-stu-id="fef18-141">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fef18-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="fef18-142">Authorization</span></span>  | <span data-ttu-id="fef18-143">string</span><span class="sxs-lookup"><span data-stu-id="fef18-143">string</span></span>  | <span data-ttu-id="fef18-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fef18-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fef18-146">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="fef18-146">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="fef18-147">string</span><span class="sxs-lookup"><span data-stu-id="fef18-147">string</span></span> | <span data-ttu-id="fef18-148">Формат возвращаемых свойств **body** и **uniqueBody**.</span><span class="sxs-lookup"><span data-stu-id="fef18-148">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="fef18-149">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="fef18-149">Values can be "text" or "html".</span></span> <span data-ttu-id="fef18-150">Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="fef18-150">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="fef18-151">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="fef18-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fef18-152">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fef18-152">Request body</span></span>
<span data-ttu-id="fef18-153">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fef18-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fef18-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="fef18-154">Response</span></span>

<span data-ttu-id="fef18-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fef18-155">If successful, this method returns a `200 OK` response code and collection of [message](../resources/message.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fef18-156">Пример</span><span class="sxs-lookup"><span data-stu-id="fef18-156">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="fef18-157">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="fef18-157">Request 1</span></span>
<span data-ttu-id="fef18-158">В первом примере возвращаются значения по умолчанию: первые 10 сообщений в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="fef18-158">The first example gets the default, top 10 messages in the signed-in user's mailbox.</span></span> <span data-ttu-id="fef18-159">`$select` используется для получения подмножества свойств каждого сообщения в ответе.</span><span class="sxs-lookup"><span data-stu-id="fef18-159">It uses `$select` to return a subset of the properties of each message in the response.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$select=sender,subject
```
##### <a name="response-1"></a><span data-ttu-id="fef18-160">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="fef18-160">Response 1</span></span>
<span data-ttu-id="fef18-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fef18-161">Here is an example of the response.</span></span> <span data-ttu-id="fef18-162">Чтобы получить следующую страницу с сообщениями, примените URL-адрес, возвращенный в `@odata.nextLink`, для последующего запроса GET.</span><span class="sxs-lookup"><span data-stu-id="fef18-162">To get the next page of messages, apply the URL returned in `@odata.nextLink` to a subsequent GET request.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="fef18-163">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="fef18-163">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fef18-164">C#</span><span class="sxs-lookup"><span data-stu-id="fef18-164">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_messages-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fef18-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="fef18-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_messages-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fef18-166">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fef18-166">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_messages-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


##### <a name="request-2"></a><span data-ttu-id="fef18-167">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="fef18-167">Request 2</span></span>
<span data-ttu-id="fef18-168">В следующем примере выполняется фильтрация всех сообщений в почтовом ящике вошедшего пользователя для тех, которые упоминают пользователя.</span><span class="sxs-lookup"><span data-stu-id="fef18-168">The next example filters all messages in the signed-in user's mailbox for those that mention the user.</span></span> <span data-ttu-id="fef18-169">Он также используется `$select` для возврата подмножества свойств каждого сообщения в ответе.</span><span class="sxs-lookup"><span data-stu-id="fef18-169">It also uses `$select` to return a subset of the properties of each message in the response.</span></span> 

<span data-ttu-id="fef18-170">В этом примере также используются URL-кодировка для пробелов в строке параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="fef18-170">The example also incorporates URL encoding for the space characters in the query parameter string.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages_with_mentions"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=MentionsPreview/IsMentioned%20eq%20true&$select=Subject,Sender,ReceivedDateTime,MentionsPreview
```
##### <a name="response-2"></a><span data-ttu-id="fef18-171">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="fef18-171">Response 2</span></span>
<span data-ttu-id="fef18-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fef18-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="fef18-175">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="fef18-175">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fef18-176">C#</span><span class="sxs-lookup"><span data-stu-id="fef18-176">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_messages_with_mentions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fef18-177">Javascript</span><span class="sxs-lookup"><span data-stu-id="fef18-177">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_messages_with_mentions-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fef18-178">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fef18-178">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_messages_with_mentions-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-3"></a><span data-ttu-id="fef18-179">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="fef18-179">Request 3</span></span>
<span data-ttu-id="fef18-180">В третьем примере показано, как использовать `Prefer: outlook.body-content-type="text"` заголовок для получения свойств **Body** и **uniqueBody** каждого сообщения в текстовом формате.</span><span class="sxs-lookup"><span data-stu-id="fef18-180">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** properties of each message in text format.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
##### <a name="response-3"></a><span data-ttu-id="fef18-181">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="fef18-181">Response 3</span></span>
<span data-ttu-id="fef18-182">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fef18-182">Here is an example of the response.</span></span> 

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="fef18-183">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="fef18-183">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fef18-184">C#</span><span class="sxs-lookup"><span data-stu-id="fef18-184">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_messages_in_text-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fef18-185">Javascript</span><span class="sxs-lookup"><span data-stu-id="fef18-185">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_messages_in_text-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fef18-186">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fef18-186">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_messages_in_text-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/user-list-messages.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-list-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-list-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-list-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
