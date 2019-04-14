---
title: Список сообщений
description: Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные").
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: dd3a5cbf3e5f4ee87b74602187c230f6be92940a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799911"
---
# <a name="list-messages"></a><span data-ttu-id="d1a37-103">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="d1a37-103">List messages</span></span>

<span data-ttu-id="d1a37-104">Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные").</span><span class="sxs-lookup"><span data-stu-id="d1a37-104">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="d1a37-105">В зависимости от размера страницы и данных почтового ящика получение сообщений из почтового ящика может повлечь множество запросов.</span><span class="sxs-lookup"><span data-stu-id="d1a37-105">Depending on the page size and mailbox data, getting messages from a mailbox can incur multiple requests.</span></span> <span data-ttu-id="d1a37-106">По умолчанию страница содержит 10 сообщений.</span><span class="sxs-lookup"><span data-stu-id="d1a37-106">The default page size for this request is 10 messages.</span></span> <span data-ttu-id="d1a37-107">Для получения следующей странице с сообщениями, просто примените весь URL-адрес, возвращаемый в `@odata.nextLink`, для другого запроса на получение сообщений.</span><span class="sxs-lookup"><span data-stu-id="d1a37-107">To get the next page of messages, simply apply the entire URL returned in `@odata.nextLink` to the next get-messages request.</span></span> <span data-ttu-id="d1a37-108">Этот URL-адрес включает любые параметры запроса, которые указаны в первоначальном запросе.</span><span class="sxs-lookup"><span data-stu-id="d1a37-108">This URL includes any query parameters you may have specified in the initial request.</span></span> 

<span data-ttu-id="d1a37-109">Не извлекайте значение `$skip` из URL-адреса `@odata.nextLink` для операций с ответами.</span><span class="sxs-lookup"><span data-stu-id="d1a37-109">Do not try to extract the `$skip` value from the `@odata.nextLink` URL to manipulate responses.</span></span> <span data-ttu-id="d1a37-110">Данный API использует значение `$skip` для учета всех элементов, просмотренных в почтовом ящике пользователя, и возврата элементов типа сообщение на странице.</span><span class="sxs-lookup"><span data-stu-id="d1a37-110">This API uses the `$skip` value to keep count of all the items it has gone through in the user's mailbox to return a page of message-type items.</span></span> <span data-ttu-id="d1a37-111">Таким образом, существует возможность, что даже в первоначальном ответе, значение `$skip` будет больше, чем размер страницы.</span><span class="sxs-lookup"><span data-stu-id="d1a37-111">It's therefore possible that even in the initial response, the `$skip` value is larger than the page size.</span></span> <span data-ttu-id="d1a37-112">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="d1a37-112">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="d1a37-113">В настоящее время эта операция возвращает текст сообщения только в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="d1a37-113">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="d1a37-114">Существует два сценария, когда приложение может получить сообщения из папки почты другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="d1a37-114">There are two scenarios where an app can get events in another user's calendar:</span></span>

* <span data-ttu-id="d1a37-115">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="d1a37-115">If the app has application permissions, or,</span></span>
* <span data-ttu-id="d1a37-116">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="d1a37-116">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="d1a37-117">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="d1a37-117">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

## <a name="permissions"></a><span data-ttu-id="d1a37-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1a37-118">Permissions</span></span>
<span data-ttu-id="d1a37-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1a37-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1a37-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1a37-121">Permission type</span></span>      | <span data-ttu-id="d1a37-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1a37-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1a37-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1a37-123">Delegated (work or school account)</span></span> | <span data-ttu-id="d1a37-124">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1a37-124">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d1a37-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1a37-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1a37-126">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1a37-126">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d1a37-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1a37-127">Application</span></span> | <span data-ttu-id="d1a37-128">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1a37-128">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1a37-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1a37-129">HTTP request</span></span>

<span data-ttu-id="d1a37-130">Для получения всех сообщений в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="d1a37-130">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="d1a37-131">Для получения сообщений из определенной папки в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="d1a37-131">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1a37-132">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d1a37-132">Optional query parameters</span></span>
<span data-ttu-id="d1a37-133">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d1a37-133">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d1a37-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1a37-134">Request headers</span></span>
| <span data-ttu-id="d1a37-135">Имя</span><span class="sxs-lookup"><span data-stu-id="d1a37-135">Name</span></span>       | <span data-ttu-id="d1a37-136">Тип</span><span class="sxs-lookup"><span data-stu-id="d1a37-136">Type</span></span> | <span data-ttu-id="d1a37-137">Описание</span><span class="sxs-lookup"><span data-stu-id="d1a37-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d1a37-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1a37-138">Authorization</span></span>  | <span data-ttu-id="d1a37-139">string</span><span class="sxs-lookup"><span data-stu-id="d1a37-139">string</span></span>  | <span data-ttu-id="d1a37-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1a37-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d1a37-142">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="d1a37-142">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="d1a37-143">string</span><span class="sxs-lookup"><span data-stu-id="d1a37-143">string</span></span> | <span data-ttu-id="d1a37-144">Формат возвращаемых свойств **body** и **uniqueBody**.</span><span class="sxs-lookup"><span data-stu-id="d1a37-144">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="d1a37-145">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="d1a37-145">Values can be "text" or "html".</span></span> <span data-ttu-id="d1a37-146">Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="d1a37-146">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="d1a37-147">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d1a37-147">Optional.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d1a37-148">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1a37-148">Request body</span></span>
<span data-ttu-id="d1a37-149">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d1a37-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1a37-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1a37-150">Response</span></span>

<span data-ttu-id="d1a37-151">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d1a37-151">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1a37-152">Пример</span><span class="sxs-lookup"><span data-stu-id="d1a37-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1a37-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1a37-153">Request</span></span>
<span data-ttu-id="d1a37-154">Данный пример получает по умолчанию 10 верхних сообщений в почтовом ящике выполнившего вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="d1a37-154">This example gets the default, top 10 messages in the signed-in user's mailbox.</span></span> <span data-ttu-id="d1a37-155">`$select` используется для получения подмножества свойств каждого сообщения в ответе.</span><span class="sxs-lookup"><span data-stu-id="d1a37-155">It uses `$select` to return a subset of the properties of each message in the response.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=sender,subject
```
##### <a name="response"></a><span data-ttu-id="d1a37-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="d1a37-156">Response</span></span>
<span data-ttu-id="d1a37-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d1a37-157">Here is an example of the response.</span></span> <span data-ttu-id="d1a37-158">Чтобы получить следующую страницу с сообщениями, примените URL-адрес, возвращенный в `@odata.nextLink`, для последующего запроса GET.</span><span class="sxs-lookup"><span data-stu-id="d1a37-158">To get the next page of messages, apply the URL returned in `@odata.nextLink` to a subsequent GET request.</span></span>

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
  "tocPath": ""
}-->
