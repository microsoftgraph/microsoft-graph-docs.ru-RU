---
title: Получение последних действий пользователя
description: " Функцию. Служба будет запрашивать последние Historyitem, а затем извлекать эти связанные действия. Действия сортируются в соответствии с последним значением **LastModified** в **historyItem**. Это означает, что действия без **historyitem** не будут включены в ответ. Разрешение UserActivity. ReadWrite. CreatedByApp также будет применять к отклику дополнительную фильтрацию, чтобы возвращались только действия, созданные приложением. Такая фильтрация на стороне сервера может привести к пустым страницам, если пользователь является особенно активным и другие приложения создали более новые действия. Чтобы получить действия приложения, используйте свойство **nextLink** для разбивки на страницы."
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ''
ms.openlocfilehash: 1aa948b9a71c0855e7bde250b90ee56c2c923579
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454894"
---
# <a name="get-recent-user-activities"></a><span data-ttu-id="aa4ae-109">Получение последних действий пользователя</span><span class="sxs-lookup"><span data-stu-id="aa4ae-109">Get recent user activities</span></span>

<span data-ttu-id="aa4ae-110">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa4ae-110">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa4ae-111">Получение последних действий для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="aa4ae-111">Get recent activities for a given user.</span></span> <span data-ttu-id="aa4ae-112">Эта функция OData имеет некоторые варианты поведения по умолчанию, которые могут работать так же, как и "самый последний использованный" API.</span><span class="sxs-lookup"><span data-stu-id="aa4ae-112">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="aa4ae-113">Служба будет запрашивать последние [historyitem](../resources/projectrome-historyitem.md), а затем извлекать эти связанные действия.</span><span class="sxs-lookup"><span data-stu-id="aa4ae-113">The service will query for the most recent [historyItems](../resources/projectrome-historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="aa4ae-114">Действия сортируются в соответствии с последним значением **LastModified** в **historyItem**.</span><span class="sxs-lookup"><span data-stu-id="aa4ae-114">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="aa4ae-115">Это означает, что действия без **historyitem** не будут включены в ответ.</span><span class="sxs-lookup"><span data-stu-id="aa4ae-115">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="aa4ae-116">Разрешение UserActivity. ReadWrite. CreatedByApp также будет применять к отклику дополнительную фильтрацию, чтобы возвращались только действия, созданные приложением.</span><span class="sxs-lookup"><span data-stu-id="aa4ae-116">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="aa4ae-117">Такая фильтрация на стороне сервера может привести к пустым страницам, если пользователь является особенно активным и другие приложения создали более новые действия.</span><span class="sxs-lookup"><span data-stu-id="aa4ae-117">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="aa4ae-118">Чтобы получить действия приложения, используйте свойство **nextLink** для разбивки на страницы.</span><span class="sxs-lookup"><span data-stu-id="aa4ae-118">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa4ae-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa4ae-119">Permissions</span></span>

<span data-ttu-id="aa4ae-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa4ae-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa4ae-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa4ae-122">Permission type</span></span>      | <span data-ttu-id="aa4ae-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa4ae-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa4ae-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa4ae-124">Delegated (work or school account)</span></span> | <span data-ttu-id="aa4ae-125">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="aa4ae-125">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="aa4ae-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa4ae-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa4ae-127">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="aa4ae-127">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="aa4ae-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa4ae-128">Application</span></span> | <span data-ttu-id="aa4ae-129">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa4ae-129">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa4ae-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa4ae-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aa4ae-131">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aa4ae-131">Optional query parameters</span></span>

<span data-ttu-id="aa4ae-132">Этот метод поддерживает некоторые [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aa4ae-132">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="aa4ae-133">Поддерживаются следующие параметры запросов:</span><span class="sxs-lookup"><span data-stu-id="aa4ae-133">The following query parameters are supported:</span></span>

- <span data-ttu-id="aa4ae-134">$expand для свойства навигации **historyitem** .</span><span class="sxs-lookup"><span data-stu-id="aa4ae-134">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="aa4ae-135">$top, чтобы ограничить максимальное количество элементов на страницах.</span><span class="sxs-lookup"><span data-stu-id="aa4ae-135">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="aa4ae-136">$filter в свойстве **lastModifiedDateTime** для **действий** или **historyitem**, если она развернута.</span><span class="sxs-lookup"><span data-stu-id="aa4ae-136">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="aa4ae-137">Ниже приведено несколько примеров поддерживаемых запросов с кодированием URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="aa4ae-137">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="aa4ae-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa4ae-138">Request headers</span></span>

|<span data-ttu-id="aa4ae-139">Имя</span><span class="sxs-lookup"><span data-stu-id="aa4ae-139">Name</span></span> | <span data-ttu-id="aa4ae-140">Тип</span><span class="sxs-lookup"><span data-stu-id="aa4ae-140">Type</span></span> | <span data-ttu-id="aa4ae-141">Описание</span><span class="sxs-lookup"><span data-stu-id="aa4ae-141">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="aa4ae-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa4ae-142">Authorization</span></span> | <span data-ttu-id="aa4ae-143">string</span><span class="sxs-lookup"><span data-stu-id="aa4ae-143">string</span></span> | <span data-ttu-id="aa4ae-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa4ae-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa4ae-146">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aa4ae-146">Request body</span></span>

<span data-ttu-id="aa4ae-147">Не указывайте текст запроса.</span><span class="sxs-lookup"><span data-stu-id="aa4ae-147">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="aa4ae-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa4ae-148">Response</span></span>

<span data-ttu-id="aa4ae-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика с последними действиями пользователя для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="aa4ae-149">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="aa4ae-150">Пример</span><span class="sxs-lookup"><span data-stu-id="aa4ae-150">Example</span></span>

##### <a name="request"></a><span data-ttu-id="aa4ae-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa4ae-151">Request</span></span>

<span data-ttu-id="aa4ae-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa4ae-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="aa4ae-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa4ae-153">Response</span></span>

<span data-ttu-id="aa4ae-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="aa4ae-154">The following is an example of the response.</span></span>

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
  "suppressions": []
}
-->
