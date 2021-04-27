---
title: 'пользователь: getMailTips'
description: Получите mailTips одного или более получателей в качестве доступных для пользователя, вписав его.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4fb7e85c4a3590bf4b5688588e4c6cc29326b181
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052623"
---
# <a name="user-getmailtips"></a><span data-ttu-id="50dc7-103">пользователь: getMailTips</span><span class="sxs-lookup"><span data-stu-id="50dc7-103">user: getMailTips</span></span>

<span data-ttu-id="50dc7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50dc7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50dc7-105">Получите mailTips одного или более получателей в качестве [](../resources/user.md)доступных для пользователя, подписав.</span><span class="sxs-lookup"><span data-stu-id="50dc7-105">Get the MailTips of one or more recipients as available to the signed-in [user](../resources/user.md).</span></span>

<span data-ttu-id="50dc7-106">Обратите внимание, что при вызове к действию можно запросить возврат определенных типов mailTips сразу для более чем одного `POST` `getMailTips` получателя.</span><span class="sxs-lookup"><span data-stu-id="50dc7-106">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="50dc7-107">Запрашиваемая mailTips возвращается в [коллекцию mailTips.](../resources/mailtips.md)</span><span class="sxs-lookup"><span data-stu-id="50dc7-107">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="50dc7-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50dc7-108">Permissions</span></span>
<span data-ttu-id="50dc7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50dc7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50dc7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50dc7-111">Permission type</span></span>      | <span data-ttu-id="50dc7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50dc7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50dc7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50dc7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="50dc7-114">Mail.Read, Mail.Read.Shared</span><span class="sxs-lookup"><span data-stu-id="50dc7-114">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="50dc7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50dc7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50dc7-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="50dc7-116">Mail.Read</span></span>    |
|<span data-ttu-id="50dc7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50dc7-117">Application</span></span> | <span data-ttu-id="50dc7-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="50dc7-118">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="50dc7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50dc7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="50dc7-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="50dc7-120">Optional query parameters</span></span>
<span data-ttu-id="50dc7-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="50dc7-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="50dc7-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50dc7-122">Request headers</span></span>
| <span data-ttu-id="50dc7-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50dc7-123">Header</span></span>       | <span data-ttu-id="50dc7-124">Значение</span><span class="sxs-lookup"><span data-stu-id="50dc7-124">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="50dc7-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50dc7-125">Authorization</span></span> | <span data-ttu-id="50dc7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50dc7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="50dc7-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="50dc7-128">Content-Type</span></span>  | <span data-ttu-id="50dc7-129">application/json</span><span class="sxs-lookup"><span data-stu-id="50dc7-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="50dc7-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50dc7-130">Request body</span></span>
<span data-ttu-id="50dc7-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="50dc7-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="50dc7-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="50dc7-132">Property</span></span>     | <span data-ttu-id="50dc7-133">Тип</span><span class="sxs-lookup"><span data-stu-id="50dc7-133">Type</span></span>   |<span data-ttu-id="50dc7-134">Описание</span><span class="sxs-lookup"><span data-stu-id="50dc7-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50dc7-135">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="50dc7-135">EmailAddresses</span></span>|<span data-ttu-id="50dc7-136">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="50dc7-136">String collection</span></span>|<span data-ttu-id="50dc7-137">Коллекция SMTP-адресов получателей для получения MailTips.</span><span class="sxs-lookup"><span data-stu-id="50dc7-137">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="50dc7-138">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="50dc7-138">MailTipsOptions</span></span>|<span data-ttu-id="50dc7-139">String</span><span class="sxs-lookup"><span data-stu-id="50dc7-139">String</span></span>|<span data-ttu-id="50dc7-140">Список флагов, которые представляют запрашиваемую почту.</span><span class="sxs-lookup"><span data-stu-id="50dc7-140">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="50dc7-141">Возможные значения: `automaticReplies` `customMailTip` , , , , , `deliveryRestriction` , , `externalMemberCount` и `mailboxFullStatus` `maxMessageSize` `moderationStatus` `recipientScope` `recipientSuggestions` `totalMemberCount` .</span><span class="sxs-lookup"><span data-stu-id="50dc7-141">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, and `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="50dc7-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="50dc7-142">Response</span></span>

<span data-ttu-id="50dc7-143">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [mailTips](../resources/mailtips.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="50dc7-143">If successful, this method returns a `200 OK` response code and a collection of [mailTips](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="50dc7-144">Пример</span><span class="sxs-lookup"><span data-stu-id="50dc7-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50dc7-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="50dc7-145">Request</span></span>
<span data-ttu-id="50dc7-146">В следующем примере получается MailTips для указанных получателей, для любых параметров автоматического ответа и полного состояния почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="50dc7-146">The following example gets MailTips for the specified recipients, for any automatic reply settings and the mailbox full status.</span></span>


# <a name="http"></a>[<span data-ttu-id="50dc7-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="50dc7-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_getmailtips"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMailTips
Content-Type: application/json

{
    "EmailAddresses": [
        "danas@contoso.onmicrosoft.com", 
        "fannyd@contoso.onmicrosoft.com"
    ],
    "MailTipsOptions": "automaticReplies, mailboxFullStatus"
}
```
# <a name="c"></a>[<span data-ttu-id="50dc7-148">C#</span><span class="sxs-lookup"><span data-stu-id="50dc7-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmailtips-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50dc7-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50dc7-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmailtips-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50dc7-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50dc7-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmailtips-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50dc7-151">Java</span><span class="sxs-lookup"><span data-stu-id="50dc7-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-getmailtips-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="50dc7-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="50dc7-152">Response</span></span>
<span data-ttu-id="50dc7-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="50dc7-153">Here is an example of the response.</span></span> <span data-ttu-id="50dc7-154">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="50dc7-154">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailTips",
  isCollection: true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailTips)",
    "value":[
        {
            "emailAddress":{
                "name":"",
                "address":"danas@contoso.onmicrosoft.com"
            },
            "automaticReplies":{
                "message":"<style type=\"text/css\" style=\"\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n<div dir=\"ltr\">\r\n<div id=\"x_divtagdefaultwrapper\" style=\"font-size:12pt; color:#000000; background-color:#FFFFFF; font-family:Calibri,Arial,Helvetica,sans-serif\">\r\n<p>Hi, I am on vacation right now. I'll get back to you after I return.<br>\r\n</p>\r\n</div>\r\n</div>",
                "messageLanguage":{
                    "locale":"en-US",
                    "displayName":"English (United States)"
                },
                "scheduledStartTime": {
                    "dateTime": "2018-08-07T02:00:00.0000000",
                    "timeZone": "UTC"
                },
                "scheduledEndTime": {
                    "dateTime": "2018-08-09T02:00:00.0000000",
                    "timeZone": "UTC"
                }
            },
            "mailboxFull":false
        },
        {
            "emailAddress":{
                "name":"",
                "address":"fannyd@contoso.onmicrosoft.com"
            },
            "automaticReplies":{
                "message":""
            },
            "mailboxFull":false
        }
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: getMailTips",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
