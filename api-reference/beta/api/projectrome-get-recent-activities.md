---
title: Получите последние действия пользователя
description: " API-ИНТЕРФЕЙС. Служба запросов для последних historyItems и затем по запросу этих связанных действий. Действия будут упорядочены в соответствии с самыми последними **lastModified** на **historyItem**. Это означает, что действия без **historyItems** не будут включены в ответе. Разрешение UserActivity.ReadWrite.CreatedByApp будут также применены дополнительные фильтрации в ответ, чтобы возвращаются только действий, созданных приложением. В этом фильтрации на сервере может привести к пустой страницы Если пользователь является особенно active и другие приложения были созданы более последние действия. Для получения действия этого приложения, используйте свойство **nextLink** для разбиения по страницам."
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 5ac5522472404e70f07b5b658e404cd4e77bbf88
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643960"
---
# <a name="get-recent-user-activities"></a><span data-ttu-id="e57c6-109">Получите последние действия пользователя</span><span class="sxs-lookup"><span data-stu-id="e57c6-109">Get recent user activities</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e57c6-110">Получите последние действия для данного пользователя.</span><span class="sxs-lookup"><span data-stu-id="e57c6-110">Get recent activities for a given user.</span></span> <span data-ttu-id="e57c6-111">Эта функция OData имеет некоторые поведения по умолчанию для работы как API «использовался последним».</span><span class="sxs-lookup"><span data-stu-id="e57c6-111">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="e57c6-112">Служба запросов для последних [historyItems](../resources/projectrome-historyitem.md)и затем по запросу этих связанных действий.</span><span class="sxs-lookup"><span data-stu-id="e57c6-112">The service will query for the most recent [historyItems](../resources/projectrome-historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="e57c6-113">Действия будут упорядочены в соответствии с самыми последними **lastModified** на **historyItem**.</span><span class="sxs-lookup"><span data-stu-id="e57c6-113">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="e57c6-114">Это означает, что действия без **historyItems** не будут включены в ответе.</span><span class="sxs-lookup"><span data-stu-id="e57c6-114">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="e57c6-115">Разрешение UserActivity.ReadWrite.CreatedByApp будут также применены дополнительные фильтрации в ответ, чтобы возвращаются только действий, созданных приложением.</span><span class="sxs-lookup"><span data-stu-id="e57c6-115">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="e57c6-116">В этом фильтрации на сервере может привести к пустой страницы Если пользователь является особенно active и другие приложения были созданы более последние действия.</span><span class="sxs-lookup"><span data-stu-id="e57c6-116">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="e57c6-117">Для получения действия этого приложения, используйте свойство **nextLink** для разбиения по страницам.</span><span class="sxs-lookup"><span data-stu-id="e57c6-117">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="e57c6-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e57c6-118">Permissions</span></span>

<span data-ttu-id="e57c6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e57c6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e57c6-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e57c6-121">Permission type</span></span>      | <span data-ttu-id="e57c6-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e57c6-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e57c6-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e57c6-123">Delegated (work or school account)</span></span> | <span data-ttu-id="e57c6-124">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="e57c6-124">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="e57c6-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e57c6-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e57c6-126">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="e57c6-126">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="e57c6-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e57c6-127">Application</span></span> | <span data-ttu-id="e57c6-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e57c6-128">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e57c6-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e57c6-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e57c6-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e57c6-130">Optional query parameters</span></span>

<span data-ttu-id="e57c6-131">Этот метод поддерживает некоторые [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e57c6-131">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="e57c6-132">Поддерживаются следующие параметры запроса:</span><span class="sxs-lookup"><span data-stu-id="e57c6-132">The following query parameters are supported:</span></span>

- <span data-ttu-id="e57c6-133">для свойства **historyItems** навигации разверните $.</span><span class="sxs-lookup"><span data-stu-id="e57c6-133">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="e57c6-134">Чтобы ограничить максимальное число элементов на страницах $top.</span><span class="sxs-lookup"><span data-stu-id="e57c6-134">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="e57c6-135">$filter свойства **lastModifiedDateTime** для **действия** или **historyItems**, если были развернуты.</span><span class="sxs-lookup"><span data-stu-id="e57c6-135">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="e57c6-136">Ниже приведены некоторые примеры поддерживаемых запросов с кодировкой URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="e57c6-136">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="e57c6-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e57c6-137">Request headers</span></span>

|<span data-ttu-id="e57c6-138">Имя</span><span class="sxs-lookup"><span data-stu-id="e57c6-138">Name</span></span> | <span data-ttu-id="e57c6-139">Тип</span><span class="sxs-lookup"><span data-stu-id="e57c6-139">Type</span></span> | <span data-ttu-id="e57c6-140">Описание</span><span class="sxs-lookup"><span data-stu-id="e57c6-140">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="e57c6-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="e57c6-141">Authorization</span></span> | <span data-ttu-id="e57c6-142">строка</span><span class="sxs-lookup"><span data-stu-id="e57c6-142">string</span></span> | <span data-ttu-id="e57c6-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e57c6-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e57c6-145">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e57c6-145">Request body</span></span>

<span data-ttu-id="e57c6-146">Не указывайте текста запроса.</span><span class="sxs-lookup"><span data-stu-id="e57c6-146">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="e57c6-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="e57c6-147">Response</span></span>

<span data-ttu-id="e57c6-148">Успешно завершена, этот метод возвращает `200 OK` код ответа с помощью последние действия пользователя для приложения.</span><span class="sxs-lookup"><span data-stu-id="e57c6-148">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="e57c6-149">Пример</span><span class="sxs-lookup"><span data-stu-id="e57c6-149">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e57c6-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="e57c6-150">Request</span></span>

<span data-ttu-id="e57c6-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e57c6-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="e57c6-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="e57c6-152">Response</span></span>

<span data-ttu-id="e57c6-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e57c6-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.activity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.activity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "https://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": "false",
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
<!--
{
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-get-recent-activities.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
