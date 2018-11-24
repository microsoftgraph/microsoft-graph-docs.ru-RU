# <a name="get-recent-user-activities"></a><span data-ttu-id="dd642-101">Получите последние действия пользователя</span><span class="sxs-lookup"><span data-stu-id="dd642-101">Get recent user activities</span></span>

<span data-ttu-id="dd642-102">Получите последние действия для данного пользователя.</span><span class="sxs-lookup"><span data-stu-id="dd642-102">Get recent activities for a given user.</span></span> <span data-ttu-id="dd642-103">Эта функция OData имеет некоторые поведения по умолчанию для работы как API «использовался последним».</span><span class="sxs-lookup"><span data-stu-id="dd642-103">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="dd642-104">Служба запросов для последних [historyItems](../resources/projectrome_historyitem.md)и затем по запросу этих связанных действий.</span><span class="sxs-lookup"><span data-stu-id="dd642-104">The service will query for the most recent [historyItems](../resources/projectrome_historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="dd642-105">Действия будут упорядочены в соответствии с самыми последними **lastModified** на **historyItem**.</span><span class="sxs-lookup"><span data-stu-id="dd642-105">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="dd642-106">Это означает, что действия без **historyItems** не будут включены в ответе.</span><span class="sxs-lookup"><span data-stu-id="dd642-106">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="dd642-107">Разрешение UserActivity.ReadWrite.CreatedByApp будут также применены дополнительные фильтрации в ответ, чтобы возвращаются только действий, созданных приложением.</span><span class="sxs-lookup"><span data-stu-id="dd642-107">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="dd642-108">В этом фильтрации на сервере может привести к пустой страницы Если пользователь является особенно active и другие приложения были созданы более последние действия.</span><span class="sxs-lookup"><span data-stu-id="dd642-108">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="dd642-109">Для получения действия этого приложения, используйте свойство **nextLink** для разбиения по страницам.</span><span class="sxs-lookup"><span data-stu-id="dd642-109">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd642-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd642-110">Permissions</span></span>

<span data-ttu-id="dd642-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dd642-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dd642-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd642-113">Permission type</span></span>      | <span data-ttu-id="dd642-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd642-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd642-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd642-115">Delegated (work or school account)</span></span> | <span data-ttu-id="dd642-116">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="dd642-116">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="dd642-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd642-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd642-118">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="dd642-118">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="dd642-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd642-119">Application</span></span> | <span data-ttu-id="dd642-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd642-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd642-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd642-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dd642-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dd642-122">Optional query parameters</span></span>

<span data-ttu-id="dd642-123">Этот метод поддерживает некоторые [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dd642-123">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="dd642-124">Поддерживаются следующие параметры запроса:</span><span class="sxs-lookup"><span data-stu-id="dd642-124">The following query parameters are supported:</span></span>

- <span data-ttu-id="dd642-125">для свойства **historyItems** навигации разверните $.</span><span class="sxs-lookup"><span data-stu-id="dd642-125">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="dd642-126">Чтобы ограничить максимальное число элементов на страницах $top.</span><span class="sxs-lookup"><span data-stu-id="dd642-126">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="dd642-127">$filter свойства **lastModifiedDateTime** для **действия** или **historyItems**, если были развернуты.</span><span class="sxs-lookup"><span data-stu-id="dd642-127">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="dd642-128">Ниже приведены некоторые примеры поддерживаемых запросов с кодировкой URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="dd642-128">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="dd642-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd642-129">Request headers</span></span>

|<span data-ttu-id="dd642-130">Имя</span><span class="sxs-lookup"><span data-stu-id="dd642-130">Name</span></span> | <span data-ttu-id="dd642-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dd642-131">Type</span></span> | <span data-ttu-id="dd642-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dd642-132">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="dd642-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd642-133">Authorization</span></span> | <span data-ttu-id="dd642-134">string</span><span class="sxs-lookup"><span data-stu-id="dd642-134">string</span></span> | <span data-ttu-id="dd642-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd642-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd642-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd642-137">Request body</span></span>

<span data-ttu-id="dd642-138">Не указывайте текста запроса.</span><span class="sxs-lookup"><span data-stu-id="dd642-138">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="dd642-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd642-139">Response</span></span>

<span data-ttu-id="dd642-140">Успешно завершена, этот метод возвращает `200 OK` код ответа с помощью последние действия пользователя для приложения.</span><span class="sxs-lookup"><span data-stu-id="dd642-140">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="dd642-141">Пример</span><span class="sxs-lookup"><span data-stu-id="dd642-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dd642-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd642-142">Request</span></span>

<span data-ttu-id="dd642-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd642-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="dd642-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd642-144">Response</span></span>

<span data-ttu-id="dd642-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dd642-145">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userActivity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.userActivity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "https://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": false,
              },
            "displayText": "Contoso How-To: How to Tie a Reef Knot",
            "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
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
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: get_recent_activities/container/contentInfo:
      Property 'contentInfo' is of type Custom but has no custom members.",

    "Warning: get_recent_activities/container/visualElements:
      Schema validation failed on property 'visualElements' ['microsoft.graph.visualInfo']",

    "Warning: get_recent_activities/container/visualElements/content:
      Schema validation failed on property 'content' ['microsoft.graph.Json']",

    "Warning: get_recent_activities/container/visualElements/content/$schema:
      Undocumented property '$schema' [String] was not expected on resource microsoft.graph.Json.",

    "Warning: get_recent_activities/container/visualElements/content/body:
      Undocumented property 'body' [Collection(Object)] was not expected on resource microsoft.graph.Json.",

    "Warning: get_recent_activities/container/visualElements/content/type:
      Undocumented property 'type' [String] was not expected on resource microsoft.graph.Json."

  ],
  "tocPath": ""
}-->
