---
title: Создание или замена действия
description: Создание новой или заменить существующий активности пользователей для вашего приложения. Если вы хотите создать действие пользователя и его связанных с ними **historyItems** в один запрос, можно использовать глубокой вставки.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 99c1abc800464a6b3c4113ba825a8455f6cdea40
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642284"
---
# <a name="create-or-replace-an-activity"></a><span data-ttu-id="e9026-104">Создание или замена действия</span><span class="sxs-lookup"><span data-stu-id="e9026-104">Create or replace an activity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9026-105">Создание новой или заменить существующий активности пользователей для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="e9026-105">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="e9026-106">Если вы хотите создать действие пользователя и его связанных с ними **historyItems** в один запрос, можно использовать [глубоко вставки](projectrome-put-activity.md#example-2---deep-insert).</span><span class="sxs-lookup"><span data-stu-id="e9026-106">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](projectrome-put-activity.md#example-2---deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9026-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9026-107">Permissions</span></span>

<span data-ttu-id="e9026-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9026-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e9026-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9026-110">Permission type</span></span>      | <span data-ttu-id="e9026-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9026-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9026-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9026-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e9026-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="e9026-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="e9026-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9026-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9026-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="e9026-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="e9026-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9026-116">Application</span></span> | <span data-ttu-id="e9026-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9026-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9026-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9026-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

><span data-ttu-id="e9026-119">**Примечание:** AppActivityId в URL-адрес должен быть URL-безопасными (все символы, за исключением RFC 2396 незарезервированные символы должны быть преобразованы в их шестнадцатеричное представление), но исходного appActivityId не должен быть безопасно URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="e9026-119">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9026-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9026-120">Request headers</span></span>

|<span data-ttu-id="e9026-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e9026-121">Name</span></span> | <span data-ttu-id="e9026-122">Тип</span><span class="sxs-lookup"><span data-stu-id="e9026-122">Type</span></span> | <span data-ttu-id="e9026-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e9026-123">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="e9026-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9026-124">Authorization</span></span> | <span data-ttu-id="e9026-125">строка</span><span class="sxs-lookup"><span data-stu-id="e9026-125">string</span></span> | <span data-ttu-id="e9026-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9026-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9026-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e9026-128">Request body</span></span>

<span data-ttu-id="e9026-129">В тексте запроса укажите представление JSON объекта [активности](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="e9026-129">In the request body, supply a JSON representation of an [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e9026-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9026-130">Response</span></span>

<span data-ttu-id="e9026-131">Успешно завершена, этот метод возвращает `201 Created` код ответа, если действие было создано или `200 OK` при замене действия.</span><span class="sxs-lookup"><span data-stu-id="e9026-131">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="example-1"></a><span data-ttu-id="e9026-132">Пример 1</span><span class="sxs-lookup"><span data-stu-id="e9026-132">Example 1</span></span>

#### <a name="request"></a><span data-ttu-id="e9026-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9026-133">Request</span></span>

<span data-ttu-id="e9026-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9026-134">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="e9026-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9026-135">Response</span></span>

<span data-ttu-id="e9026-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e9026-136">The following is an example of the response.</span></span>

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
            "addImageQuery": "false"
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

## <a name="example-2---deep-insert"></a><span data-ttu-id="e9026-137">В примере 2 - глубокой insert</span><span class="sxs-lookup"><span data-stu-id="e9026-137">Example 2 - Deep insert</span></span>

#### <a name="request"></a><span data-ttu-id="e9026-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9026-138">Request</span></span>

<span data-ttu-id="e9026-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9026-139">The following is an example of the request.</span></span>

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
    },
    "historyItems":[
        {
            "userTimezone": "Africa/Casablanca",
            "startedDateTime": "2018-02-26T20:54:04.345Z",
            "lastActiveDateTime": "2018-02-26T20:54:24.345Z"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="e9026-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9026-140">Response</span></span>

<span data-ttu-id="e9026-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e9026-141">The following is an example of the response.</span></span>

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
            "addImageQuery": "false"
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
<!--
{
  "type": "#page.annotation",
  "description": "Upsert activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-put-activity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
