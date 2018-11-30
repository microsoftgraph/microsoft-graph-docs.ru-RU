---
title: Получите последние действия пользователя
description: " API-ИНТЕРФЕЙС. Служба запросов для последних historyItems и затем по запросу этих связанных действий. Действия будут упорядочены в соответствии с самыми последними **lastModified** на **historyItem**. Это означает, что действия без **historyItems** не будут включены в ответе. Разрешение UserActivity.ReadWrite.CreatedByApp будут также применены дополнительные фильтрации в ответ, чтобы возвращаются только действий, созданных приложением. В этом фильтрации на сервере может привести к пустой страницы Если пользователь является особенно active и другие приложения были созданы более последние действия. Для получения действия этого приложения, используйте свойство **nextLink** для разбиения по страницам."
ms.openlocfilehash: 7dbd51e416d62016add020b784b0f7d0ace473cc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082777"
---
# <a name="get-recent-user-activities"></a><span data-ttu-id="71279-109">Получите последние действия пользователя</span><span class="sxs-lookup"><span data-stu-id="71279-109">Get recent user activities</span></span>

> <span data-ttu-id="71279-110">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="71279-110">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71279-111">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71279-111">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="71279-112">Получите последние действия для данного пользователя.</span><span class="sxs-lookup"><span data-stu-id="71279-112">Get recent activities for a given user.</span></span> <span data-ttu-id="71279-113">Эта функция OData имеет некоторые поведения по умолчанию для работы как API «использовался последним».</span><span class="sxs-lookup"><span data-stu-id="71279-113">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="71279-114">Служба запросов для последних [historyItems](../resources/projectrome-historyitem.md)и затем по запросу этих связанных действий.</span><span class="sxs-lookup"><span data-stu-id="71279-114">The service will query for the most recent [historyItems](../resources/projectrome-historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="71279-115">Действия будут упорядочены в соответствии с самыми последними **lastModified** на **historyItem**.</span><span class="sxs-lookup"><span data-stu-id="71279-115">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="71279-116">Это означает, что действия без **historyItems** не будут включены в ответе.</span><span class="sxs-lookup"><span data-stu-id="71279-116">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="71279-117">Разрешение UserActivity.ReadWrite.CreatedByApp будут также применены дополнительные фильтрации в ответ, чтобы возвращаются только действий, созданных приложением.</span><span class="sxs-lookup"><span data-stu-id="71279-117">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="71279-118">В этом фильтрации на сервере может привести к пустой страницы Если пользователь является особенно active и другие приложения были созданы более последние действия.</span><span class="sxs-lookup"><span data-stu-id="71279-118">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="71279-119">Для получения действия этого приложения, используйте свойство **nextLink** для разбиения по страницам.</span><span class="sxs-lookup"><span data-stu-id="71279-119">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="71279-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71279-120">Permissions</span></span>

<span data-ttu-id="71279-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71279-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71279-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71279-123">Permission type</span></span>      | <span data-ttu-id="71279-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71279-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71279-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71279-125">Delegated (work or school account)</span></span> | <span data-ttu-id="71279-126">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="71279-126">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="71279-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71279-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71279-128">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="71279-128">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="71279-129">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71279-129">Application</span></span> | <span data-ttu-id="71279-130">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71279-130">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71279-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71279-131">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71279-132">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="71279-132">Optional query parameters</span></span>

<span data-ttu-id="71279-133">Этот метод поддерживает некоторые [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="71279-133">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="71279-134">Поддерживаются следующие параметры запроса:</span><span class="sxs-lookup"><span data-stu-id="71279-134">The following query parameters are supported:</span></span>

- <span data-ttu-id="71279-135">для свойства **historyItems** навигации разверните $.</span><span class="sxs-lookup"><span data-stu-id="71279-135">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="71279-136">Чтобы ограничить максимальное число элементов на страницах $top.</span><span class="sxs-lookup"><span data-stu-id="71279-136">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="71279-137">$filter свойства **lastModifiedDateTime** для **действия** или **historyItems**, если были развернуты.</span><span class="sxs-lookup"><span data-stu-id="71279-137">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="71279-138">Ниже приведены некоторые примеры поддерживаемых запросов с кодировкой URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="71279-138">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="71279-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71279-139">Request headers</span></span>

|<span data-ttu-id="71279-140">Имя</span><span class="sxs-lookup"><span data-stu-id="71279-140">Name</span></span> | <span data-ttu-id="71279-141">Тип</span><span class="sxs-lookup"><span data-stu-id="71279-141">Type</span></span> | <span data-ttu-id="71279-142">Описание</span><span class="sxs-lookup"><span data-stu-id="71279-142">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="71279-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="71279-143">Authorization</span></span> | <span data-ttu-id="71279-144">string</span><span class="sxs-lookup"><span data-stu-id="71279-144">string</span></span> | <span data-ttu-id="71279-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71279-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71279-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71279-147">Request body</span></span>

<span data-ttu-id="71279-148">Не указывайте текста запроса.</span><span class="sxs-lookup"><span data-stu-id="71279-148">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="71279-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="71279-149">Response</span></span>

<span data-ttu-id="71279-150">Успешно завершена, этот метод возвращает `200 OK` код ответа с помощью последние действия пользователя для приложения.</span><span class="sxs-lookup"><span data-stu-id="71279-150">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="71279-151">Пример</span><span class="sxs-lookup"><span data-stu-id="71279-151">Example</span></span>

##### <a name="request"></a><span data-ttu-id="71279-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="71279-152">Request</span></span>

<span data-ttu-id="71279-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71279-153">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="71279-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="71279-154">Response</span></span>

<span data-ttu-id="71279-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="71279-155">The following is an example of the response.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
