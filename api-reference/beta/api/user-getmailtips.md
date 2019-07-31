---
title: 'Пользователь: подсказки'
description: Получение подсказок одного или нескольких получателей, доступных пользователю, вошедшего в систему.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9c623429eda707f639e4d6e039542b3dcbe77c9f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987728"
---
# <a name="user-getmailtips"></a><span data-ttu-id="7104e-103">Пользователь: подсказки</span><span class="sxs-lookup"><span data-stu-id="7104e-103">user: getMailTips</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7104e-104">Получение подсказок одного или нескольких получателей, доступных [пользователю](../resources/user.md), вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="7104e-104">Get the MailTips of one or more recipients as available to the signed-in [user](../resources/user.md).</span></span>

<span data-ttu-id="7104e-105">Обратите внимание, что `POST` выполнив вызов `getMailTips` действия, вы можете запросить определенные типы подсказок, которые будут возвращаться сразу для нескольких получателей.</span><span class="sxs-lookup"><span data-stu-id="7104e-105">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="7104e-106">Запрошенные подсказки возвращаются в коллекции [подсказок](../resources/mailtips.md) .</span><span class="sxs-lookup"><span data-stu-id="7104e-106">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="7104e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7104e-107">Permissions</span></span>
<span data-ttu-id="7104e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7104e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7104e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7104e-110">Permission type</span></span>      | <span data-ttu-id="7104e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7104e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7104e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7104e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7104e-113">Mail. Read, mail. Read. Shared</span><span class="sxs-lookup"><span data-stu-id="7104e-113">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="7104e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7104e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7104e-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7104e-115">Mail.Read</span></span>    |
|<span data-ttu-id="7104e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7104e-116">Application</span></span> | <span data-ttu-id="7104e-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7104e-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="7104e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7104e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7104e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7104e-119">Optional query parameters</span></span>
<span data-ttu-id="7104e-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7104e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7104e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7104e-121">Request headers</span></span>
| <span data-ttu-id="7104e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7104e-122">Header</span></span>       | <span data-ttu-id="7104e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7104e-123">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="7104e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7104e-124">Authorization</span></span> | <span data-ttu-id="7104e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7104e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7104e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7104e-127">Content-Type</span></span>  | <span data-ttu-id="7104e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7104e-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7104e-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7104e-129">Request body</span></span>
<span data-ttu-id="7104e-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7104e-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7104e-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="7104e-131">Property</span></span>     | <span data-ttu-id="7104e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="7104e-132">Type</span></span>   |<span data-ttu-id="7104e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="7104e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7104e-134">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="7104e-134">EmailAddresses</span></span>|<span data-ttu-id="7104e-135">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7104e-135">String collection</span></span>|<span data-ttu-id="7104e-136">Коллекция SMTP-адресов получателей, для которых требуется получить подсказки.</span><span class="sxs-lookup"><span data-stu-id="7104e-136">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="7104e-137">Маилтипсоптионс</span><span class="sxs-lookup"><span data-stu-id="7104e-137">MailTipsOptions</span></span>|<span data-ttu-id="7104e-138">String</span><span class="sxs-lookup"><span data-stu-id="7104e-138">String</span></span>|<span data-ttu-id="7104e-139">Перечисление флагов, представляющих запрашиваемые подсказки.</span><span class="sxs-lookup"><span data-stu-id="7104e-139">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="7104e-140">Возможные `automaticReplies`значения:, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`и. `totalMemberCount`</span><span class="sxs-lookup"><span data-stu-id="7104e-140">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, and `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="7104e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="7104e-141">Response</span></span>

<span data-ttu-id="7104e-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [подсказки](../resources/mailtips.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7104e-142">If successful, this method returns a `200 OK` response code and a collection of [mailTips](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7104e-143">Пример</span><span class="sxs-lookup"><span data-stu-id="7104e-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7104e-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="7104e-144">Request</span></span>
<span data-ttu-id="7104e-145">В следующем примере показано, как получить подсказки для указанных получателей для всех параметров автоматического ответа и полного состояния почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="7104e-145">The following example gets MailTips for the specified recipients, for any automatic reply settings and the mailbox full status.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7104e-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="7104e-146">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7104e-147">C#</span><span class="sxs-lookup"><span data-stu-id="7104e-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmailtips-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7104e-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="7104e-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmailtips-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7104e-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7104e-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmailtips-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7104e-150">Java</span><span class="sxs-lookup"><span data-stu-id="7104e-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-getmailtips-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7104e-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="7104e-151">Response</span></span>
<span data-ttu-id="7104e-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7104e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
