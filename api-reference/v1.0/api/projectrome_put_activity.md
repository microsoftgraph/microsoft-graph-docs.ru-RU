# <a name="create-or-replace-an-activity"></a><span data-ttu-id="27e83-101">Создание или замена активности</span><span class="sxs-lookup"><span data-stu-id="27e83-101">Create or replace an activity</span></span>

<span data-ttu-id="27e83-102">Создание нового или замена существующего факта активности пользователя вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="27e83-102">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="27e83-103">Если вы хотите создать факт активности пользователя и связанные с ним элементы **historyItems** в одном запросе, можно использовать [глубокую вставку](projectrome_put_activity.md#example-2---deep-insert).</span><span class="sxs-lookup"><span data-stu-id="27e83-103">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](projectrome_put_activity.md#example-2---deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="27e83-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27e83-104">Permissions</span></span>

<span data-ttu-id="27e83-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="27e83-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="27e83-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27e83-107">Permission type</span></span>      | <span data-ttu-id="27e83-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27e83-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27e83-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27e83-109">Delegated (work or school account)</span></span> | <span data-ttu-id="27e83-110">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="27e83-110">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="27e83-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27e83-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27e83-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="27e83-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="27e83-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27e83-113">Application</span></span> | <span data-ttu-id="27e83-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27e83-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27e83-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27e83-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

><span data-ttu-id="27e83-116">**Примечание:** AppActivityId в URL-адресе должен быть в URL-безопасном формате (все символы, за исключением незарезервированных символов RFC 2396, должны быть преобразованы в шестнадцатеричное представление), однако исходный appActivityId не должен быть в URL-безопасном формате.</span><span class="sxs-lookup"><span data-stu-id="27e83-116">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="27e83-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27e83-117">Request headers</span></span>

|<span data-ttu-id="27e83-118">Имя</span><span class="sxs-lookup"><span data-stu-id="27e83-118">Name</span></span> | <span data-ttu-id="27e83-119">Тип</span><span class="sxs-lookup"><span data-stu-id="27e83-119">Type</span></span> | <span data-ttu-id="27e83-120">Описание</span><span class="sxs-lookup"><span data-stu-id="27e83-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="27e83-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27e83-121">Authorization</span></span> | <span data-ttu-id="27e83-122">строка</span><span class="sxs-lookup"><span data-stu-id="27e83-122">string</span></span> | <span data-ttu-id="27e83-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27e83-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="27e83-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27e83-125">Request body</span></span>

<span data-ttu-id="27e83-126">В тексте запроса должно быть представление объекта [activity](../resources/projectrome_activity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27e83-126">In the request body, supply a JSON representation of an [educationSchool](../resources/projectrome_activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="27e83-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="27e83-127">Response</span></span>

<span data-ttu-id="27e83-128">При успешном выполнении этот метод возвращает код отклика `201 Created`, если факт активности был создан, или `200 OK`, если факт активности был заменен.</span><span class="sxs-lookup"><span data-stu-id="27e83-128">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="example-1"></a><span data-ttu-id="27e83-129">Пример 1</span><span class="sxs-lookup"><span data-stu-id="27e83-129">Example 1</span></span>

#### <a name="request"></a><span data-ttu-id="27e83-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="27e83-130">Request</span></span>

<span data-ttu-id="27e83-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27e83-131">The following is an example of the request.</span></span>

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
    "activationUrl": "http://www.contoso.com/article?id=12345",
    "contentUrl": "http://www.contoso.com/article?id=12345",
    "fallbackUrl": "http://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "http://schema.org",
        "@type": "Article",
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "visualElements": {
        "attribution": {
            "iconUrl": "http://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false,
        },
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "backgroundColor": "#ff0000",
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "content": {
            "$schema": "http://adaptivecards.io/schemas/adaptive-card.json",
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

#### <a name="response"></a><span data-ttu-id="27e83-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="27e83-132">Response</span></span>

<span data-ttu-id="27e83-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="27e83-133">The following is an example of the response.</span></span>

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
    "activitySourceHost": "http://contoso.com",
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
            "iconUrl": "http://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false
        },
        "backgroundColor": "#ff0000",
        "content": {
            "$schema": "http://adaptivecards.io/schemas/adaptive-card.json",
            "type": "AdaptiveCard",
            "body":
            [{
                "type": "TextBlock",
                "text": "Contoso MainPage"
            }]
        }
    },
    "activationUrl": "http://www.contoso.com/article?id=12345",
    "appDisplayName": "Contoso, Ltd.",
    "userTimezone": "Africa/Casablanca",
    "fallbackUrl": "http://www.contoso.com/article?id=12345",
    "contentUrl": "http://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "http://schema.org",
        "@type": "Article",
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
}
```

## <a name="example-2---deep-insert"></a><span data-ttu-id="27e83-134">Пример 2 — глубокая вставка</span><span class="sxs-lookup"><span data-stu-id="27e83-134">Example 2 - Deep insert</span></span>

#### <a name="request"></a><span data-ttu-id="27e83-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="27e83-135">Request</span></span>

<span data-ttu-id="27e83-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27e83-136">The following is an example of the request.</span></span>

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
    "activationUrl": "http://www.contoso.com/article?id=12345",
    "contentUrl": "http://www.contoso.com/article?id=12345",
    "fallbackUrl": "http://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "http://schema.org",
        "@type": "Article",
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "visualElements": {
        "attribution": {
            "iconUrl": "http://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false,
        },
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "backgroundColor": "#ff0000",
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "content": {
            "$schema": "http://adaptivecards.io/schemas/adaptive-card.json",
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

#### <a name="response"></a><span data-ttu-id="27e83-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="27e83-137">Response</span></span>

<span data-ttu-id="27e83-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="27e83-138">The following is an example of the response.</span></span>

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
    "activitySourceHost": "http://contoso.com",
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
            "iconUrl": "http://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false
        },
        "backgroundColor": "#ff0000",
        "content": {
            "$schema": "http://adaptivecards.io/schemas/adaptive-card.json",
            "type": "AdaptiveCard",
            "body":
            [{
                "type": "TextBlock",
                "text": "Contoso MainPage"
            }]
        }
    },
    "activationUrl": "http://www.contoso.com/article?id=12345",
    "appDisplayName": "Contoso, Ltd.",
    "userTimezone": "Africa/Casablanca",
    "fallbackUrl": "http://www.contoso.com/article?id=12345",
    "contentUrl": "http://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "http://schema.org",
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
