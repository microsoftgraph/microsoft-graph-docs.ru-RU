---
title: Создание или замена действия
description: Создание новой или заменить существующий активности пользователей для вашего приложения. Если вы хотите создать действие пользователя и его связанных с ними **historyItems** в один запрос, можно использовать глубокой вставки.
ms.openlocfilehash: 1a749f0c4303551ab9915c89d84e6757c61bd0a2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079542"
---
# <a name="create-or-replace-an-activity"></a><span data-ttu-id="5cb46-104">Создание или замена действия</span><span class="sxs-lookup"><span data-stu-id="5cb46-104">Create or replace an activity</span></span>

> <span data-ttu-id="5cb46-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5cb46-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5cb46-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cb46-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5cb46-107">Создание новой или заменить существующий активности пользователей для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="5cb46-107">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="5cb46-108">Если вы хотите создать действие пользователя и его связанных с ними **historyItems** в один запрос, можно использовать [глубоко вставки](projectrome-put-activity.md#example-2---deep-insert).</span><span class="sxs-lookup"><span data-stu-id="5cb46-108">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](projectrome-put-activity.md#example-2---deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="5cb46-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5cb46-109">Permissions</span></span>

<span data-ttu-id="5cb46-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cb46-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5cb46-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5cb46-112">Permission type</span></span>      | <span data-ttu-id="5cb46-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5cb46-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5cb46-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5cb46-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5cb46-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="5cb46-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="5cb46-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5cb46-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cb46-117">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="5cb46-117">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="5cb46-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5cb46-118">Application</span></span> | <span data-ttu-id="5cb46-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cb46-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5cb46-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5cb46-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

><span data-ttu-id="5cb46-121">**Примечание:** AppActivityId в URL-адрес должен быть URL-безопасными (все символы, за исключением RFC 2396 незарезервированные символы должны быть преобразованы в их шестнадцатеричное представление), но исходного appActivityId не должен быть безопасно URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="5cb46-121">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5cb46-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5cb46-122">Request headers</span></span>

|<span data-ttu-id="5cb46-123">Имя</span><span class="sxs-lookup"><span data-stu-id="5cb46-123">Name</span></span> | <span data-ttu-id="5cb46-124">Тип</span><span class="sxs-lookup"><span data-stu-id="5cb46-124">Type</span></span> | <span data-ttu-id="5cb46-125">Описание</span><span class="sxs-lookup"><span data-stu-id="5cb46-125">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="5cb46-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cb46-126">Authorization</span></span> | <span data-ttu-id="5cb46-127">string</span><span class="sxs-lookup"><span data-stu-id="5cb46-127">string</span></span> | <span data-ttu-id="5cb46-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5cb46-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cb46-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5cb46-130">Request body</span></span>

<span data-ttu-id="5cb46-131">В тексте запроса укажите представление JSON объекта [активности](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="5cb46-131">In the request body, supply a JSON representation of an [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5cb46-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="5cb46-132">Response</span></span>

<span data-ttu-id="5cb46-133">Успешно завершена, этот метод возвращает `201 Created` код ответа, если действие было создано или `200 OK` при замене действия.</span><span class="sxs-lookup"><span data-stu-id="5cb46-133">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="example-1"></a><span data-ttu-id="5cb46-134">Пример 1</span><span class="sxs-lookup"><span data-stu-id="5cb46-134">Example 1</span></span>

#### <a name="request"></a><span data-ttu-id="5cb46-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="5cb46-135">Request</span></span>

<span data-ttu-id="5cb46-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5cb46-136">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/beta/me/activities/%2Farticle%3F12345
Content-type: application/json
Content-length: 364

{
    "appActivityId": "/article?12345",
    "activitySourceHost": "https://www.contoso.com",
    "userTimezone": "Africa/Casablanca",
    "appDisplayName": "Contoso, Ltd.",
    "activationUrl": "https://www.contoso.com/article?id=12345",
    "contentUrl": "https://www.contoso.com/article?id=12345",
    "fallbackUrl": "https://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "https://schema.org",
        "@type": "Article",
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "visualElements": {
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": "false"
        },
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "backgroundColor": "#ff0000",
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "content": {
            "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
            "type": "AdaptiveCard",
            "body":
            [{
                "type": "TextBlock",
                "text": "Contoso MainPage"
            }]
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="5cb46-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="5cb46-137">Response</span></span>

<span data-ttu-id="5cb46-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5cb46-138">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/beta/me/activities/14332800362997268276

{
    "activitySourceHost": "https://contoso.com",
    "createdDateTime": "2017-06-09T20:54:43.969Z",
    "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
    "id": "14332800362997268276",
    "appActivityId": "/article?12345",
    "status":"updated",
    "expirationDateTime": "2017-02-26T20:20:48.114Z",
    "id": "14332800362997268276",
    "visualElements": {
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false
        },
        "backgroundColor": "#ff0000",
        "content": {
            "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
            "type": "AdaptiveCard",
            "body":
            [{
                "type": "TextBlock",
                "text": "Contoso MainPage"
            }]
        }
    },
    "activationUrl": "https://www.contoso.com/article?id=12345",
    "appDisplayName": "Contoso, Ltd.",
    "userTimezone": "Africa/Casablanca",
    "fallbackUrl": "https://www.contoso.com/article?id=12345",
    "contentUrl": "https://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "https://schema.org",
        "@type": "Article",
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
}
```

## <a name="example-2---deep-insert"></a><span data-ttu-id="5cb46-139">В примере 2 - глубокой insert</span><span class="sxs-lookup"><span data-stu-id="5cb46-139">Example 2 - Deep insert</span></span>

#### <a name="request"></a><span data-ttu-id="5cb46-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="5cb46-140">Request</span></span>

<span data-ttu-id="5cb46-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5cb46-141">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/beta/me/activities/%2Farticle%3F12345
Content-type: application/json
Content-length: 364

{
    "appActivityId": "/article?12345",
    "activitySourceHost": "https://www.contoso.com",
    "userTimezone": "Africa/Casablanca",
    "appDisplayName": "Contoso, Ltd.",
    "activationUrl": "https://www.contoso.com/article?id=12345",
    "contentUrl": "https://www.contoso.com/article?id=12345",
    "fallbackUrl": "https://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "https://schema.org",
        "@type": "Article",
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "visualElements": {
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": "false",
        },
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "backgroundColor": "#ff0000",
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "content": {
            "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
            "type": "AdaptiveCard",
            "body":
            [{
                "type": "TextBlock",
                "text": "Contoso MainPage"
            }]
        }
    },
    "historyItems":[
        {
            "userTimezone": "Africa/Casablanca",
            "startedDateTime": "2018-02-26T20:54:04.345Z",
            "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="5cb46-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="5cb46-142">Response</span></span>

<span data-ttu-id="5cb46-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5cb46-143">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/beta/me/activities/14332800362997268276

{
    "activitySourceHost": "https://contoso.com",
    "createdDateTime": "2017-06-09T20:54:43.969Z",
    "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
    "id": "14332800362997268276",
    "appActivityId": "/article?12345",
    "status":"updated",
    "expirationDateTime": "2017-02-26T20:20:48.114Z",
    "id": "14332800362997268276",
    "visualElements": {
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false
        },
        "backgroundColor": "#ff0000",
        "content": {
            "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
            "type": "AdaptiveCard",
            "body":
            [{
                "type": "TextBlock",
                "text": "Contoso MainPage"
            }]
        }
    },
    "activationUrl": "https://www.contoso.com/article?id=12345",
    "appDisplayName": "Contoso, Ltd.",
    "userTimezone": "Africa/Casablanca",
    "fallbackUrl": "https://www.contoso.com/article?id=12345",
    "contentUrl": "https://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "https://schema.org",
        "@type": "Article",
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "historyItems":[
        {
            "status": "updated",
            "userTimezone": "Africa/Casablanca",
            "createdDateTime": "2018-04-12T21:42:42.495Z",
            "lastModifiedDateTime": "2018-04-12T21:42:42.495Z",
            "id": "61fc8f36-919f-4b73-89d4-1cb7b159d912",
            "startedDateTime": "2018-02-26T20:54:04.345Z",
            "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
            "expirationDateTime": "2018-05-12T21:42:42.495Z",
            "activeDurationSeconds": 20
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upsert activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
