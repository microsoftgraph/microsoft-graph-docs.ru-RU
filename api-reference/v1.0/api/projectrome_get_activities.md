# <a name="get-user-activities"></a><span data-ttu-id="c081c-101">Получение действий пользователя</span><span class="sxs-lookup"><span data-stu-id="c081c-101">Get user activities</span></span>

<span data-ttu-id="c081c-102">Получение действий для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="c081c-102">Get activities for a given user.</span></span> <span data-ttu-id="c081c-103">В отличие от функции OData **recent** (последние), действия без истории будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="c081c-103">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="c081c-104">Разрешение UserActivity.ReadWrite.CreatedByApp применит дополнительные фильтры к ответу, чтобы возвращались только действия, созданные вашим приложением.</span><span class="sxs-lookup"><span data-stu-id="c081c-104">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="c081c-105">Такая фильтрация на стороне сервера может привести к возникновению пустых страниц, если пользователь особенно активен, и другие приложения зафиксировали более свежие факты активности.</span><span class="sxs-lookup"><span data-stu-id="c081c-105">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="c081c-106">Для получения действий в вашем приложении, используйте свойство **nextLink** для разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="c081c-106">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="c081c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c081c-107">Permissions</span></span>

<span data-ttu-id="c081c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c081c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c081c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c081c-110">Permission type</span></span>      | <span data-ttu-id="c081c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c081c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c081c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c081c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c081c-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="c081c-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="c081c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c081c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c081c-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="c081c-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="c081c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c081c-116">Application</span></span> | <span data-ttu-id="c081c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c081c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c081c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c081c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c081c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c081c-119">Optional query parameters</span></span>

<span data-ttu-id="c081c-120">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c081c-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span> <span data-ttu-id="c081c-121">Поддерживаются следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="c081c-121">The following query parameters are supported:</span></span>

- <span data-ttu-id="c081c-122">$expand — для свойства навигации **historyItems**.</span><span class="sxs-lookup"><span data-stu-id="c081c-122">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="c081c-123">$top — для ограничения максимального числа элементов на страницах.</span><span class="sxs-lookup"><span data-stu-id="c081c-123">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="c081c-124">$filter для свойства **lastModifiedDateTime** — для действий или элементов истории (**historyItems**), если они были развернуты.</span><span class="sxs-lookup"><span data-stu-id="c081c-124">$filter on the **lastModifiedDateTime** property for either activities or **historyItems**, if expanded.</span></span>

<span data-ttu-id="c081c-125">Ниже приведены некоторые примеры поддерживаемых запросов с кодировкой URL-адреса:</span><span class="sxs-lookup"><span data-stu-id="c081c-125">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="c081c-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c081c-126">Request headers</span></span>

|<span data-ttu-id="c081c-127">Имя</span><span class="sxs-lookup"><span data-stu-id="c081c-127">Name</span></span> | <span data-ttu-id="c081c-128">Тип</span><span class="sxs-lookup"><span data-stu-id="c081c-128">Type</span></span> | <span data-ttu-id="c081c-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c081c-129">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="c081c-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c081c-130">Authorization</span></span> | <span data-ttu-id="c081c-131">строка</span><span class="sxs-lookup"><span data-stu-id="c081c-131">string</span></span> | <span data-ttu-id="c081c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c081c-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c081c-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c081c-134">Request body</span></span>

<span data-ttu-id="c081c-135">Нет текста запроса.</span><span class="sxs-lookup"><span data-stu-id="c081c-135">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="c081c-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="c081c-136">Response</span></span>

<span data-ttu-id="c081c-137">При успешном выполнении этот метод возвращает код отклика `200 OK` с действиями пользователя в приложении.</span><span class="sxs-lookup"><span data-stu-id="c081c-137">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="c081c-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c081c-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c081c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c081c-139">Request</span></span>

<span data-ttu-id="c081c-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c081c-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities
```

##### <a name="response"></a><span data-ttu-id="c081c-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="c081c-141">Response</span></span>

<span data-ttu-id="c081c-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c081c-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.activity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/activities?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.userActivity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "http://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": false,
              },
            "displayText": "Contoso How-To: How to Tie a Reef Knot",
            "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
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
            "author": "John Doe",
            "name": "How to Tie a Reef Knot"
        },
        "expirationDateTime": "2018-03-28T18:34:29.607Z",
        "status": "updated"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
