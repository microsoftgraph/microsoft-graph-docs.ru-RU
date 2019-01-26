---
title: Получение действия пользователя
description: Получение действий для определенного пользователя. В отличие от **последние** функции OData будут возвращены действия без личных дел. Разрешение UserActivity.ReadWrite.CreatedByApp будут применяться дополнительных фильтрации в ответ, чтобы возвращаются только действий, созданных приложением. В этом фильтрации на сервере может привести к пустой страницы Если пользователь является особенно active и другие приложения были созданы более последние действия. Для получения действия этого приложения, используйте свойство **nextLink** для разбиения по страницам.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: acca0926e08887143c12bed6517efbc87e41d178
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575732"
---
# <a name="get-user-activities"></a><span data-ttu-id="22d2b-107">Получение действия пользователя</span><span class="sxs-lookup"><span data-stu-id="22d2b-107">Get user activities</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22d2b-108">Получение действий для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="22d2b-108">Get activities for a given user.</span></span> <span data-ttu-id="22d2b-109">В отличие от **последние** функции OData будут возвращены действия без личных дел.</span><span class="sxs-lookup"><span data-stu-id="22d2b-109">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="22d2b-110">Разрешение UserActivity.ReadWrite.CreatedByApp будут применяться дополнительных фильтрации в ответ, чтобы возвращаются только действий, созданных приложением.</span><span class="sxs-lookup"><span data-stu-id="22d2b-110">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="22d2b-111">В этом фильтрации на сервере может привести к пустой страницы Если пользователь является особенно active и другие приложения были созданы более последние действия.</span><span class="sxs-lookup"><span data-stu-id="22d2b-111">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="22d2b-112">Для получения действия этого приложения, используйте свойство **nextLink** для разбиения по страницам.</span><span class="sxs-lookup"><span data-stu-id="22d2b-112">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="22d2b-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22d2b-113">Permissions</span></span>

<span data-ttu-id="22d2b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22d2b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22d2b-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22d2b-116">Permission type</span></span>      | <span data-ttu-id="22d2b-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22d2b-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22d2b-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22d2b-118">Delegated (work or school account)</span></span> | <span data-ttu-id="22d2b-119">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="22d2b-119">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="22d2b-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22d2b-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22d2b-121">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="22d2b-121">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="22d2b-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22d2b-122">Application</span></span> | <span data-ttu-id="22d2b-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22d2b-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22d2b-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22d2b-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22d2b-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="22d2b-125">Optional query parameters</span></span>

<span data-ttu-id="22d2b-126">Этот метод поддерживает некоторые [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="22d2b-126">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="22d2b-127">Поддерживаются следующие параметры запроса:</span><span class="sxs-lookup"><span data-stu-id="22d2b-127">The following query parameters are supported:</span></span>

- <span data-ttu-id="22d2b-128">для свойства **historyItems** навигации разверните $.</span><span class="sxs-lookup"><span data-stu-id="22d2b-128">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="22d2b-129">Чтобы ограничить максимальное число элементов на страницах $top.</span><span class="sxs-lookup"><span data-stu-id="22d2b-129">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="22d2b-130">$filter свойства **lastModifiedDateTime** для **действия** или **historyItems**, если были развернуты.</span><span class="sxs-lookup"><span data-stu-id="22d2b-130">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="22d2b-131">Ниже приведены некоторые примеры поддерживаемых запросов с кодировкой URL-адрес:</span><span class="sxs-lookup"><span data-stu-id="22d2b-131">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="22d2b-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22d2b-132">Request headers</span></span>

|<span data-ttu-id="22d2b-133">Имя</span><span class="sxs-lookup"><span data-stu-id="22d2b-133">Name</span></span> | <span data-ttu-id="22d2b-134">Тип</span><span class="sxs-lookup"><span data-stu-id="22d2b-134">Type</span></span> | <span data-ttu-id="22d2b-135">Описание</span><span class="sxs-lookup"><span data-stu-id="22d2b-135">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="22d2b-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="22d2b-136">Authorization</span></span> | <span data-ttu-id="22d2b-137">string</span><span class="sxs-lookup"><span data-stu-id="22d2b-137">string</span></span> | <span data-ttu-id="22d2b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22d2b-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="22d2b-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22d2b-140">Request body</span></span>

<span data-ttu-id="22d2b-141">Нет текста запроса.</span><span class="sxs-lookup"><span data-stu-id="22d2b-141">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="22d2b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="22d2b-142">Response</span></span>

<span data-ttu-id="22d2b-143">Успешно завершена, этот метод возвращает `200 OK` код ответа с помощью действий пользователя для приложения.</span><span class="sxs-lookup"><span data-stu-id="22d2b-143">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="22d2b-144">Пример</span><span class="sxs-lookup"><span data-stu-id="22d2b-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="22d2b-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="22d2b-145">Request</span></span>

<span data-ttu-id="22d2b-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22d2b-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities
```

##### <a name="response"></a><span data-ttu-id="22d2b-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="22d2b-147">Response</span></span>

<span data-ttu-id="22d2b-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22d2b-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.activity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/activities?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "microsoft.graph.activity",
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
  "description": "Get activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-get-activities.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
