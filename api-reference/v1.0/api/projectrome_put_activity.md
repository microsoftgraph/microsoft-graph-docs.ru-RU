# <a name="create-or-replace-an-activity"></a><span data-ttu-id="c0a1c-101">Создание или замена действия</span><span class="sxs-lookup"><span data-stu-id="c0a1c-101">Create or replace an activity</span></span>

<span data-ttu-id="c0a1c-102">Создание новой или заменить существующий активности пользователей для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="c0a1c-102">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="c0a1c-103">Если вы хотите создать действие пользователя и его связанных с ними **historyItems** в один запрос, можно использовать [глубоко вставки](projectrome_put_activity.md#example-2---deep-insert).</span><span class="sxs-lookup"><span data-stu-id="c0a1c-103">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](projectrome_put_activity.md#example-2---deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="c0a1c-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0a1c-104">Permissions</span></span>

<span data-ttu-id="c0a1c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c0a1c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="c0a1c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0a1c-107">Permission type</span></span>      | <span data-ttu-id="c0a1c-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0a1c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0a1c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0a1c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c0a1c-110">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="c0a1c-110">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="c0a1c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0a1c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0a1c-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="c0a1c-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="c0a1c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0a1c-113">Application</span></span> | <span data-ttu-id="c0a1c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0a1c-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0a1c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0a1c-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

><span data-ttu-id="c0a1c-116">**Примечание:** AppActivityId в URL-адрес должен быть URL-безопасными (все символы, за исключением RFC 2396 незарезервированные символы должны быть преобразованы в их шестнадцатеричное представление), но исходного appActivityId не должен быть безопасно URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="c0a1c-116">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0a1c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0a1c-117">Request headers</span></span>

|<span data-ttu-id="c0a1c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c0a1c-118">Name</span></span> | <span data-ttu-id="c0a1c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c0a1c-119">Type</span></span> | <span data-ttu-id="c0a1c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c0a1c-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="c0a1c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0a1c-121">Authorization</span></span> | <span data-ttu-id="c0a1c-122">string</span><span class="sxs-lookup"><span data-stu-id="c0a1c-122">string</span></span> | <span data-ttu-id="c0a1c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0a1c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0a1c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0a1c-125">Request body</span></span>

<span data-ttu-id="c0a1c-126">В тексте запроса укажите представление JSON объекта [активности](../resources/projectrome_activity.md) .</span><span class="sxs-lookup"><span data-stu-id="c0a1c-126">In the request body, supply a JSON representation of an [activity](../resources/projectrome_activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c0a1c-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0a1c-127">Response</span></span>

<span data-ttu-id="c0a1c-128">Успешно завершена, этот метод возвращает `201 Created` код ответа, если действие было создано или `200 OK` при замене действия.</span><span class="sxs-lookup"><span data-stu-id="c0a1c-128">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="example-1"></a><span data-ttu-id="c0a1c-129">Пример 1</span><span class="sxs-lookup"><span data-stu-id="c0a1c-129">Example 1</span></span>

#### <a name="request"></a><span data-ttu-id="c0a1c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0a1c-130">Request</span></span>

<span data-ttu-id="c0a1c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0a1c-131">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
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
            "addImageQuery": false,
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

#### <a name="response"></a><span data-ttu-id="c0a1c-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0a1c-132">Response</span></span>

<span data-ttu-id="c0a1c-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c0a1c-133">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/v1.0/me/activities/14332800362997268276

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

## <a name="example-2---deep-insert"></a><span data-ttu-id="c0a1c-134">В примере 2 - глубокой insert</span><span class="sxs-lookup"><span data-stu-id="c0a1c-134">Example 2 - Deep insert</span></span>

#### <a name="request"></a><span data-ttu-id="c0a1c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0a1c-135">Request</span></span>

<span data-ttu-id="c0a1c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0a1c-136">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
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
            "addImageQuery": false,
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

#### <a name="response"></a><span data-ttu-id="c0a1c-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0a1c-137">Response</span></span>

<span data-ttu-id="c0a1c-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c0a1c-138">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/v1.0/me/activities/14332800362997268276

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
