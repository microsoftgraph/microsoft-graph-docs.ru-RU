---
title: Получение действий пользователей
description: Получение действий для определенного пользователя. В отличие от **последней** функции OData, будут возвращены действия без журналов. Разрешение UserActivity. ReadWrite. CreatedByApp будет применять к отклику дополнительную фильтрацию, чтобы возвращались только действия, созданные приложением. Такая фильтрация на стороне сервера может привести к пустым страницам, если пользователь является особенно активным и другие приложения создали более новые действия. Чтобы получить действия приложения, используйте свойство **nextLink** для разбивки на страницы.
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: apiPageType
ms.openlocfilehash: 1a3dad16f96f8b16618a1916bcccf6cf67eb95ff
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35975888"
---
# <a name="get-user-activities"></a><span data-ttu-id="7f5e8-107">Получение действий пользователей</span><span class="sxs-lookup"><span data-stu-id="7f5e8-107">Get user activities</span></span>

<span data-ttu-id="7f5e8-108">Получение действий для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="7f5e8-108">Get activities for a given user.</span></span> <span data-ttu-id="7f5e8-109">В отличие от **последней** функции OData, будут возвращены действия без журналов.</span><span class="sxs-lookup"><span data-stu-id="7f5e8-109">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="7f5e8-110">Разрешение UserActivity. ReadWrite. CreatedByApp будет применять к отклику дополнительную фильтрацию, чтобы возвращались только действия, созданные приложением.</span><span class="sxs-lookup"><span data-stu-id="7f5e8-110">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="7f5e8-111">Такая фильтрация на стороне сервера может привести к пустым страницам, если пользователь является особенно активным и другие приложения создали более новые действия.</span><span class="sxs-lookup"><span data-stu-id="7f5e8-111">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="7f5e8-112">Чтобы получить действия приложения, используйте свойство **nextLink** для разбивки на страницы.</span><span class="sxs-lookup"><span data-stu-id="7f5e8-112">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f5e8-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f5e8-113">Permissions</span></span>

<span data-ttu-id="7f5e8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f5e8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f5e8-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f5e8-116">Permission type</span></span>      | <span data-ttu-id="7f5e8-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f5e8-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f5e8-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f5e8-118">Delegated (work or school account)</span></span> | <span data-ttu-id="7f5e8-119">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="7f5e8-119">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="7f5e8-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f5e8-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f5e8-121">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="7f5e8-121">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="7f5e8-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f5e8-122">Application</span></span> | <span data-ttu-id="7f5e8-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f5e8-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f5e8-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f5e8-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f5e8-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7f5e8-125">Optional query parameters</span></span>

<span data-ttu-id="7f5e8-126">Этот метод поддерживает некоторые [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7f5e8-126">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="7f5e8-127">Поддерживаются следующие параметры запросов:</span><span class="sxs-lookup"><span data-stu-id="7f5e8-127">The following query parameters are supported:</span></span>

- <span data-ttu-id="7f5e8-128">$expand для свойства навигации **historyitem** .</span><span class="sxs-lookup"><span data-stu-id="7f5e8-128">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="7f5e8-129">$top, чтобы ограничить максимальное количество элементов на страницах.</span><span class="sxs-lookup"><span data-stu-id="7f5e8-129">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="7f5e8-130">$filter в свойстве **lastModifiedDateTime** для действий или **historyitem**, если она развернута.</span><span class="sxs-lookup"><span data-stu-id="7f5e8-130">$filter on the **lastModifiedDateTime** property for either activities or **historyItems**, if expanded.</span></span>

<span data-ttu-id="7f5e8-131">Ниже приведено несколько примеров поддерживаемых запросов с кодированием URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="7f5e8-131">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="7f5e8-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f5e8-132">Request headers</span></span>

|<span data-ttu-id="7f5e8-133">Имя</span><span class="sxs-lookup"><span data-stu-id="7f5e8-133">Name</span></span> | <span data-ttu-id="7f5e8-134">Тип</span><span class="sxs-lookup"><span data-stu-id="7f5e8-134">Type</span></span> | <span data-ttu-id="7f5e8-135">Описание</span><span class="sxs-lookup"><span data-stu-id="7f5e8-135">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="7f5e8-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f5e8-136">Authorization</span></span> | <span data-ttu-id="7f5e8-137">string</span><span class="sxs-lookup"><span data-stu-id="7f5e8-137">string</span></span> | <span data-ttu-id="7f5e8-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f5e8-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f5e8-140">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7f5e8-140">Request body</span></span>

<span data-ttu-id="7f5e8-141">Текст запроса отсутствует.</span><span class="sxs-lookup"><span data-stu-id="7f5e8-141">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="7f5e8-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f5e8-142">Response</span></span>

<span data-ttu-id="7f5e8-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика с действиями пользователя для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="7f5e8-143">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="7f5e8-144">Пример</span><span class="sxs-lookup"><span data-stu-id="7f5e8-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7f5e8-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f5e8-145">Request</span></span>

<span data-ttu-id="7f5e8-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f5e8-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities
```

##### <a name="response"></a><span data-ttu-id="7f5e8-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f5e8-147">Response</span></span>

<span data-ttu-id="7f5e8-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7f5e8-148">The following is an example of the response.</span></span>

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
  "description": "Get activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
