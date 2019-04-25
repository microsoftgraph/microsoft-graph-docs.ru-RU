---
title: Получение последних действий пользователя
description: " Функцию. Служба будет запрашивать последние Historyitem, а затем извлекать эти связанные действия. Действия сортируются в соответствии с последним значением **LastModified** в **historyItem**. Это означает, что действия без **historyitem** не будут включены в ответ. Разрешение UserActivity. ReadWrite. CreatedByApp также будет применять к отклику дополнительную фильтрацию, чтобы возвращались только действия, созданные приложением. Такая фильтрация на стороне сервера может привести к пустым страницам, если пользователь является особенно активным и другие приложения создали более новые действия. Чтобы получить действия приложения, используйте свойство **nextLink** для разбивки на страницы."
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: d7d119f5a80e86a47c8f61756cad99542d0b3b0b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575340"
---
# <a name="get-recent-user-activities"></a><span data-ttu-id="81ebb-109">Получение последних действий пользователя</span><span class="sxs-lookup"><span data-stu-id="81ebb-109">Get recent user activities</span></span>

<span data-ttu-id="81ebb-110">Получение последних действий для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="81ebb-110">Get recent activities for a given user.</span></span> <span data-ttu-id="81ebb-111">Эта функция OData имеет некоторые варианты поведения по умолчанию, которые могут работать так же, как и "самый последний использованный" API.</span><span class="sxs-lookup"><span data-stu-id="81ebb-111">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="81ebb-112">Служба будет запрашивать последние [historyitem](../resources/projectrome-historyitem.md), а затем извлекать эти связанные действия.</span><span class="sxs-lookup"><span data-stu-id="81ebb-112">The service will query for the most recent [historyItems](../resources/projectrome-historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="81ebb-113">Действия сортируются в соответствии с последним значением **LastModified** в **historyItem**.</span><span class="sxs-lookup"><span data-stu-id="81ebb-113">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="81ebb-114">Это означает, что действия без **historyitem** не будут включены в ответ.</span><span class="sxs-lookup"><span data-stu-id="81ebb-114">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="81ebb-115">Разрешение UserActivity. ReadWrite. CreatedByApp также будет применять к отклику дополнительную фильтрацию, чтобы возвращались только действия, созданные приложением.</span><span class="sxs-lookup"><span data-stu-id="81ebb-115">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="81ebb-116">Такая фильтрация на стороне сервера может привести к пустым страницам, если пользователь является особенно активным и другие приложения создали более новые действия.</span><span class="sxs-lookup"><span data-stu-id="81ebb-116">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="81ebb-117">Чтобы получить действия приложения, используйте свойство **nextLink** для разбивки на страницы.</span><span class="sxs-lookup"><span data-stu-id="81ebb-117">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="81ebb-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81ebb-118">Permissions</span></span>

<span data-ttu-id="81ebb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81ebb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81ebb-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81ebb-121">Permission type</span></span>      | <span data-ttu-id="81ebb-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81ebb-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81ebb-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81ebb-123">Delegated (work or school account)</span></span> | <span data-ttu-id="81ebb-124">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="81ebb-124">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="81ebb-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81ebb-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81ebb-126">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="81ebb-126">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="81ebb-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81ebb-127">Application</span></span> | <span data-ttu-id="81ebb-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81ebb-128">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81ebb-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81ebb-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81ebb-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="81ebb-130">Optional query parameters</span></span>

<span data-ttu-id="81ebb-131">Этот метод поддерживает некоторые [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="81ebb-131">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="81ebb-132">Поддерживаются следующие параметры запросов:</span><span class="sxs-lookup"><span data-stu-id="81ebb-132">The following query parameters are supported:</span></span>

- <span data-ttu-id="81ebb-133">$expand для свойства навигации **historyitem** .</span><span class="sxs-lookup"><span data-stu-id="81ebb-133">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="81ebb-134">$Top, чтобы ограничить максимальное количество элементов на страницах.</span><span class="sxs-lookup"><span data-stu-id="81ebb-134">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="81ebb-135">$filter в свойстве **lastModifiedDateTime** для **действий** или **historyitem**, если она развернута.</span><span class="sxs-lookup"><span data-stu-id="81ebb-135">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="81ebb-136">Ниже приведено несколько примеров поддерживаемых запросов с кодированием URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="81ebb-136">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="81ebb-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81ebb-137">Request headers</span></span>

|<span data-ttu-id="81ebb-138">Имя</span><span class="sxs-lookup"><span data-stu-id="81ebb-138">Name</span></span> | <span data-ttu-id="81ebb-139">Тип</span><span class="sxs-lookup"><span data-stu-id="81ebb-139">Type</span></span> | <span data-ttu-id="81ebb-140">Описание</span><span class="sxs-lookup"><span data-stu-id="81ebb-140">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="81ebb-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="81ebb-141">Authorization</span></span> | <span data-ttu-id="81ebb-142">string</span><span class="sxs-lookup"><span data-stu-id="81ebb-142">string</span></span> | <span data-ttu-id="81ebb-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81ebb-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81ebb-145">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81ebb-145">Request body</span></span>

<span data-ttu-id="81ebb-146">Не указывайте текст запроса.</span><span class="sxs-lookup"><span data-stu-id="81ebb-146">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="81ebb-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="81ebb-147">Response</span></span>

<span data-ttu-id="81ebb-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика с последними действиями пользователя для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="81ebb-148">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="81ebb-149">Пример</span><span class="sxs-lookup"><span data-stu-id="81ebb-149">Example</span></span>

##### <a name="request"></a><span data-ttu-id="81ebb-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="81ebb-150">Request</span></span>

<span data-ttu-id="81ebb-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81ebb-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="81ebb-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="81ebb-152">Response</span></span>

<span data-ttu-id="81ebb-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="81ebb-153">The following is an example of the response.</span></span>

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

    "Warning: get_recent_activities/container/visualElements/content/$schema:
      Undocumented property '$schema' [String] was not expected on resource microsoft.graph.Json.",

    "Warning: get_recent_activities/container/visualElements/content/body:
      Undocumented property 'body' [Collection(Object)] was not expected on resource microsoft.graph.Json.",

    "Warning: get_recent_activities/container/visualElements/content/type:
      Undocumented property 'type' [String] was not expected on resource microsoft.graph.Json."

  ],
  "tocPath": ""
}-->
