---
title: Получение действий пользователей
description: Получение действий для определенного пользователя. В отличие от **последней** функции OData, будут возвращены действия без журналов. Разрешение UserActivity. ReadWrite. CreatedByApp будет применять к отклику дополнительную фильтрацию, чтобы возвращались только действия, созданные приложением. Такая фильтрация на стороне сервера может привести к пустым страницам, если пользователь является особенно активным и другие приложения создали более новые действия. Чтобы получить действия приложения, используйте свойство **nextLink** для разбивки на страницы.
localization_priority: Normal
ms.prod: project-rome
author: ailae
doc_type: apiPageType
ms.openlocfilehash: 61221581354c5742c85a6cc2bcf931afd67a5481
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051720"
---
# <a name="get-user-activities"></a><span data-ttu-id="81c65-107">Получение действий пользователей</span><span class="sxs-lookup"><span data-stu-id="81c65-107">Get user activities</span></span>

<span data-ttu-id="81c65-108">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81c65-108">Namespace: microsoft.graph</span></span>

<span data-ttu-id="81c65-109">Получение действий для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="81c65-109">Get activities for a given user.</span></span> <span data-ttu-id="81c65-110">В отличие от **последней** функции OData, будут возвращены действия без журналов.</span><span class="sxs-lookup"><span data-stu-id="81c65-110">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="81c65-111">Разрешение UserActivity. ReadWrite. CreatedByApp будет применять к отклику дополнительную фильтрацию, чтобы возвращались только действия, созданные приложением.</span><span class="sxs-lookup"><span data-stu-id="81c65-111">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="81c65-112">Такая фильтрация на стороне сервера может привести к пустым страницам, если пользователь является особенно активным и другие приложения создали более новые действия.</span><span class="sxs-lookup"><span data-stu-id="81c65-112">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="81c65-113">Чтобы получить действия приложения, используйте свойство **nextLink** для разбивки на страницы.</span><span class="sxs-lookup"><span data-stu-id="81c65-113">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="81c65-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81c65-114">Permissions</span></span>

<span data-ttu-id="81c65-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81c65-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81c65-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81c65-117">Permission type</span></span>      | <span data-ttu-id="81c65-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81c65-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81c65-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81c65-119">Delegated (work or school account)</span></span> | <span data-ttu-id="81c65-120">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="81c65-120">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="81c65-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81c65-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81c65-122">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="81c65-122">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="81c65-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81c65-123">Application</span></span> | <span data-ttu-id="81c65-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81c65-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81c65-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81c65-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81c65-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="81c65-126">Optional query parameters</span></span>

<span data-ttu-id="81c65-127">Этот метод поддерживает некоторые [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="81c65-127">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="81c65-128">Поддерживаются следующие параметры запросов:</span><span class="sxs-lookup"><span data-stu-id="81c65-128">The following query parameters are supported:</span></span>

- <span data-ttu-id="81c65-129">$expand для свойства навигации **historyitem** .</span><span class="sxs-lookup"><span data-stu-id="81c65-129">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="81c65-130">$top, чтобы ограничить максимальное количество элементов на страницах.</span><span class="sxs-lookup"><span data-stu-id="81c65-130">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="81c65-131">$filter в свойстве **lastModifiedDateTime** для действий или **historyitem**, если она развернута.</span><span class="sxs-lookup"><span data-stu-id="81c65-131">$filter on the **lastModifiedDateTime** property for either activities or **historyItems**, if expanded.</span></span>

<span data-ttu-id="81c65-132">Ниже приведено несколько примеров поддерживаемых запросов с кодированием URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="81c65-132">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="81c65-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81c65-133">Request headers</span></span>

|<span data-ttu-id="81c65-134">Имя</span><span class="sxs-lookup"><span data-stu-id="81c65-134">Name</span></span> | <span data-ttu-id="81c65-135">Тип</span><span class="sxs-lookup"><span data-stu-id="81c65-135">Type</span></span> | <span data-ttu-id="81c65-136">Описание</span><span class="sxs-lookup"><span data-stu-id="81c65-136">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="81c65-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="81c65-137">Authorization</span></span> | <span data-ttu-id="81c65-138">string</span><span class="sxs-lookup"><span data-stu-id="81c65-138">string</span></span> | <span data-ttu-id="81c65-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81c65-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81c65-141">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="81c65-141">Request body</span></span>

<span data-ttu-id="81c65-142">Текст запроса отсутствует.</span><span class="sxs-lookup"><span data-stu-id="81c65-142">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="81c65-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="81c65-143">Response</span></span>

<span data-ttu-id="81c65-144">В случае успешного выполнения этот метод возвращает `200 OK` код отклика с действиями пользователя для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="81c65-144">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="81c65-145">Пример</span><span class="sxs-lookup"><span data-stu-id="81c65-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="81c65-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="81c65-146">Request</span></span>

<span data-ttu-id="81c65-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81c65-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities
```

##### <a name="response"></a><span data-ttu-id="81c65-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="81c65-148">Response</span></span>

<span data-ttu-id="81c65-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="81c65-149">The following is an example of the response.</span></span>

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

