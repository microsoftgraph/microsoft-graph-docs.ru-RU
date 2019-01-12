---
title: 'пользователь: getMailTips'
description: Получите подсказки одного или нескольких получателей как доступные для пользователя, выполнившего вход.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 899524a9db73a202901800804c6061289f32f3fb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958126"
---
# <a name="user-getmailtips"></a><span data-ttu-id="c506d-103">пользователь: getMailTips</span><span class="sxs-lookup"><span data-stu-id="c506d-103">user: getMailTips</span></span>

> <span data-ttu-id="c506d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c506d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c506d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c506d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c506d-106">Получите подсказки одного или нескольких получателей как доступные выполнившего вход [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="c506d-106">Get the MailTips of one or more recipients as available to the signed-in [user](../resources/user.md).</span></span>

<span data-ttu-id="c506d-107">Обратите внимание, что благодаря `POST` звонок, чтобы `getMailTips` действие, можно запросить определенных типов подсказки должно быть возвращено для нескольких получателей за один раз.</span><span class="sxs-lookup"><span data-stu-id="c506d-107">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="c506d-108">Запрошенный подсказок возвращаются в коллекцию [подсказок](../resources/mailtips.md) .</span><span class="sxs-lookup"><span data-stu-id="c506d-108">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="c506d-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c506d-109">Permissions</span></span>
<span data-ttu-id="c506d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c506d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c506d-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c506d-112">Permission type</span></span>      | <span data-ttu-id="c506d-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c506d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c506d-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c506d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c506d-115">Mail.Read Mail.Read.Shared</span><span class="sxs-lookup"><span data-stu-id="c506d-115">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="c506d-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c506d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c506d-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c506d-117">Mail.Read</span></span>    |
|<span data-ttu-id="c506d-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c506d-118">Application</span></span> | <span data-ttu-id="c506d-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c506d-119">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="c506d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c506d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c506d-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c506d-121">Optional query parameters</span></span>
<span data-ttu-id="c506d-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c506d-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c506d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c506d-123">Request headers</span></span>
| <span data-ttu-id="c506d-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c506d-124">Header</span></span>       | <span data-ttu-id="c506d-125">Значение</span><span class="sxs-lookup"><span data-stu-id="c506d-125">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="c506d-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c506d-126">Authorization</span></span> | <span data-ttu-id="c506d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c506d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c506d-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c506d-129">Content-Type</span></span>  | <span data-ttu-id="c506d-130">application/json</span><span class="sxs-lookup"><span data-stu-id="c506d-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c506d-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c506d-131">Request body</span></span>
<span data-ttu-id="c506d-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c506d-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c506d-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="c506d-133">Property</span></span>     | <span data-ttu-id="c506d-134">Тип</span><span class="sxs-lookup"><span data-stu-id="c506d-134">Type</span></span>   |<span data-ttu-id="c506d-135">Описание</span><span class="sxs-lookup"><span data-stu-id="c506d-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c506d-136">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="c506d-136">EmailAddresses</span></span>|<span data-ttu-id="c506d-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c506d-137">String collection</span></span>|<span data-ttu-id="c506d-138">Коллекция SMTP-адреса для получения подсказок для получателей.</span><span class="sxs-lookup"><span data-stu-id="c506d-138">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="c506d-139">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="c506d-139">MailTipsOptions</span></span>|<span data-ttu-id="c506d-140">Строка</span><span class="sxs-lookup"><span data-stu-id="c506d-140">String</span></span>|<span data-ttu-id="c506d-141">Перечисление флаги, который представляет запрошенный подсказок.</span><span class="sxs-lookup"><span data-stu-id="c506d-141">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="c506d-142">Возможные значения: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, и `totalMemberCount`.</span><span class="sxs-lookup"><span data-stu-id="c506d-142">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, and `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="c506d-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c506d-143">Response</span></span>

<span data-ttu-id="c506d-144">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [подсказок](../resources/mailtips.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c506d-144">If successful, this method returns a `200 OK` response code and a collection of [mailTips](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c506d-145">Пример</span><span class="sxs-lookup"><span data-stu-id="c506d-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c506d-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="c506d-146">Request</span></span>
<span data-ttu-id="c506d-147">В следующем примере получается подсказки для заданных получателей для все параметры автоматического ответа, а также состояние полный почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="c506d-147">The following example gets MailTips for the specified recipients, for any automatic reply settings and the mailbox full status.</span></span>

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

##### <a name="response"></a><span data-ttu-id="c506d-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="c506d-148">Response</span></span>
<span data-ttu-id="c506d-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c506d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "user: getMailTips",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
