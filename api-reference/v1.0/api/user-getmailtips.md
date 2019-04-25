---
title: 'Пользователь: подсказки'
description: Получение подСказок одного или нескольких получателей, доступных пользователю, вошедшего в систему.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4c931d6e7f3b7762534d773b647f7db68461a230
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567867"
---
# <a name="user-getmailtips"></a><span data-ttu-id="b1382-103">Пользователь: подсказки</span><span class="sxs-lookup"><span data-stu-id="b1382-103">user: getMailTips</span></span>

<span data-ttu-id="b1382-104">Получение подСказок одного или нескольких получателей, доступных [пользователю](../resources/user.md), вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="b1382-104">Get the MailTips of one or more recipients as available to the signed-in [user](../resources/user.md).</span></span>

<span data-ttu-id="b1382-105">Обратите внимание, что `POST` выполнив вызов `getMailTips` действия, вы можете запросить определенные типы подсказок, которые будут возвращаться сразу для нескольких получателей.</span><span class="sxs-lookup"><span data-stu-id="b1382-105">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="b1382-106">Запрошенные подсказки возвращаются в коллекции [подсказок](../resources/mailtips.md) .</span><span class="sxs-lookup"><span data-stu-id="b1382-106">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1382-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1382-107">Permissions</span></span>
<span data-ttu-id="b1382-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1382-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1382-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1382-110">Permission type</span></span>      | <span data-ttu-id="b1382-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1382-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1382-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1382-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b1382-113">Mail. Read, mail. Read. Shared</span><span class="sxs-lookup"><span data-stu-id="b1382-113">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="b1382-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1382-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1382-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b1382-115">Mail.Read</span></span>    |
|<span data-ttu-id="b1382-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1382-116">Application</span></span> | <span data-ttu-id="b1382-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b1382-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1382-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1382-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b1382-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b1382-119">Optional query parameters</span></span>
<span data-ttu-id="b1382-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b1382-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b1382-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1382-121">Request headers</span></span>
| <span data-ttu-id="b1382-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1382-122">Header</span></span>       | <span data-ttu-id="b1382-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b1382-123">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="b1382-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1382-124">Authorization</span></span> | <span data-ttu-id="b1382-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1382-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b1382-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b1382-127">Content-Type</span></span>  | <span data-ttu-id="b1382-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b1382-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b1382-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1382-129">Request body</span></span>
<span data-ttu-id="b1382-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b1382-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b1382-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1382-131">Property</span></span>     | <span data-ttu-id="b1382-132">Тип</span><span class="sxs-lookup"><span data-stu-id="b1382-132">Type</span></span>   |<span data-ttu-id="b1382-133">Описание</span><span class="sxs-lookup"><span data-stu-id="b1382-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1382-134">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="b1382-134">EmailAddresses</span></span>|<span data-ttu-id="b1382-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b1382-135">String collection</span></span>|<span data-ttu-id="b1382-136">Коллекция SMTP-адресов получателей, для которых требуется получить подсказки.</span><span class="sxs-lookup"><span data-stu-id="b1382-136">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="b1382-137">Маилтипсоптионс</span><span class="sxs-lookup"><span data-stu-id="b1382-137">MailTipsOptions</span></span>|<span data-ttu-id="b1382-138">String</span><span class="sxs-lookup"><span data-stu-id="b1382-138">String</span></span>|<span data-ttu-id="b1382-139">Перечисление флагов, представляющих запрашиваемые подсказки.</span><span class="sxs-lookup"><span data-stu-id="b1382-139">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="b1382-140">Возможные `automaticReplies`значения:, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`и. `totalMemberCount`</span><span class="sxs-lookup"><span data-stu-id="b1382-140">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, and `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="b1382-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1382-141">Response</span></span>

<span data-ttu-id="b1382-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [подсказки](../resources/mailtips.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b1382-142">If successful, this method returns a `200 OK` response code and a collection of [mailTips](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b1382-143">Пример</span><span class="sxs-lookup"><span data-stu-id="b1382-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1382-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1382-144">Request</span></span>
<span data-ttu-id="b1382-145">В следующем примере показано, как получить подсказки для указанных получателей для всех параметров автоматического ответа и полного состояния почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b1382-145">The following example gets MailTips for the specified recipients, for any automatic reply settings and the mailbox full status.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_getmailtips"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMailTips
Content-Type: application/json

{
    "EmailAddresses": [
        "danas@contoso.onmicrosoft.com", 
        "fannyd@contoso.onmicrosoft.com"
    ],
    "MailTipsOptions": "automaticReplies, mailboxFullStatus"
}
```

##### <a name="response"></a><span data-ttu-id="b1382-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1382-146">Response</span></span>
<span data-ttu-id="b1382-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1382-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.mailTips)",
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
<!-- {
  "type": "#page.annotation",
  "description": "user: getMailTips",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
