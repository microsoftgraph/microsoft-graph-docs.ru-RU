---
title: 'user: getMailTips'
description: Получите сообщения о том, что один или несколько получателей доступны во вписаемом пользователю.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cbbeffff7949096693969b03d6f3aa7bbf5bfe44
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131679"
---
# <a name="user-getmailtips"></a><span data-ttu-id="70ca4-103">user: getMailTips</span><span class="sxs-lookup"><span data-stu-id="70ca4-103">user: getMailTips</span></span>

<span data-ttu-id="70ca4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70ca4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70ca4-105">Получите в качестве доступных для пользователя, выписав в качестве адресатов, соответствующие одному или более [получателям.](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="70ca4-105">Get the MailTips of one or more recipients as available to the signed-in [user](../resources/user.md).</span></span>

<span data-ttu-id="70ca4-106">Обратите внимание, что, вызовите действие, вы можете запросить определенные типы сообщений, которые будут возвращаться для более чем одного получателя `POST` `getMailTips` за один раз.</span><span class="sxs-lookup"><span data-stu-id="70ca4-106">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="70ca4-107">Запрашиваемая электронная почта возвращается в [коллекции.](../resources/mailtips.md)</span><span class="sxs-lookup"><span data-stu-id="70ca4-107">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="70ca4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70ca4-108">Permissions</span></span>
<span data-ttu-id="70ca4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70ca4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70ca4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70ca4-111">Permission type</span></span>      | <span data-ttu-id="70ca4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70ca4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70ca4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70ca4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="70ca4-114">Mail.Read, Mail.Read.Shared</span><span class="sxs-lookup"><span data-stu-id="70ca4-114">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="70ca4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70ca4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70ca4-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="70ca4-116">Mail.Read</span></span>    |
|<span data-ttu-id="70ca4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70ca4-117">Application</span></span> | <span data-ttu-id="70ca4-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="70ca4-118">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="70ca4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70ca4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="70ca4-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="70ca4-120">Optional query parameters</span></span>
<span data-ttu-id="70ca4-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="70ca4-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="70ca4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70ca4-122">Request headers</span></span>
| <span data-ttu-id="70ca4-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70ca4-123">Header</span></span>       | <span data-ttu-id="70ca4-124">Значение</span><span class="sxs-lookup"><span data-stu-id="70ca4-124">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="70ca4-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70ca4-125">Authorization</span></span> | <span data-ttu-id="70ca4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70ca4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="70ca4-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70ca4-128">Content-Type</span></span>  | <span data-ttu-id="70ca4-129">application/json</span><span class="sxs-lookup"><span data-stu-id="70ca4-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="70ca4-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70ca4-130">Request body</span></span>
<span data-ttu-id="70ca4-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="70ca4-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="70ca4-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="70ca4-132">Property</span></span>     | <span data-ttu-id="70ca4-133">Тип</span><span class="sxs-lookup"><span data-stu-id="70ca4-133">Type</span></span>   |<span data-ttu-id="70ca4-134">Описание</span><span class="sxs-lookup"><span data-stu-id="70ca4-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70ca4-135">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="70ca4-135">EmailAddresses</span></span>|<span data-ttu-id="70ca4-136">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="70ca4-136">String collection</span></span>|<span data-ttu-id="70ca4-137">Коллекция SMTP-адресов получателей для получения сообщений.</span><span class="sxs-lookup"><span data-stu-id="70ca4-137">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="70ca4-138">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="70ca4-138">MailTipsOptions</span></span>|<span data-ttu-id="70ca4-139">Строка</span><span class="sxs-lookup"><span data-stu-id="70ca4-139">String</span></span>|<span data-ttu-id="70ca4-140">Список флагов, которые представляют запрашиваемую почту.</span><span class="sxs-lookup"><span data-stu-id="70ca4-140">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="70ca4-141">Возможные значения: `automaticReplies` , , , , , , , и `customMailTip` `deliveryRestriction` `externalMemberCount` `mailboxFullStatus` `maxMessageSize` `moderationStatus` `recipientScope` `recipientSuggestions` `totalMemberCount` .</span><span class="sxs-lookup"><span data-stu-id="70ca4-141">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, and `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="70ca4-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="70ca4-142">Response</span></span>

<span data-ttu-id="70ca4-143">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [mailTips](../resources/mailtips.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70ca4-143">If successful, this method returns a `200 OK` response code and a collection of [mailTips](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="70ca4-144">Пример</span><span class="sxs-lookup"><span data-stu-id="70ca4-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70ca4-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="70ca4-145">Request</span></span>
<span data-ttu-id="70ca4-146">В следующем примере по мере настройки автоматического ответа и полного состояния почтового ящика для указанных получателей возвращается сообщение о всех параметрах автоматического ответа.</span><span class="sxs-lookup"><span data-stu-id="70ca4-146">The following example gets MailTips for the specified recipients, for any automatic reply settings and the mailbox full status.</span></span>


# <a name="http"></a>[<span data-ttu-id="70ca4-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="70ca4-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="70ca4-148">C#</span><span class="sxs-lookup"><span data-stu-id="70ca4-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmailtips-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70ca4-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70ca4-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmailtips-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70ca4-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70ca4-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmailtips-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70ca4-151">Java</span><span class="sxs-lookup"><span data-stu-id="70ca4-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-getmailtips-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="70ca4-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="70ca4-152">Response</span></span>
<span data-ttu-id="70ca4-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70ca4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
