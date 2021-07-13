---
title: Получать последние действия пользователя
description: " API. Служба запрашивает последние historyItems и затем вытягивает связанные действия. Действия будут сортироваться в соответствии с последним **lastModified** на **historyItem**. Это означает, что действия без **historyItems** не будут включены в ответ. Разрешение UserActivity.ReadWrite.CreatedByApp также применяет дополнительную фильтрацию к ответу, чтобы возвращались только действия, созданные вашим приложением. Это фильтрация на стороне сервера может привести к пустым страницам, если пользователь особенно активен, а другие приложения создали более последние действия. Чтобы получить действия приложения, используйте свойство **nextLink** для пагинации."
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ailae
ms.openlocfilehash: 27361d56e62e1ea255c2a0e9e3b6d3e0b45ee44e
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401507"
---
# <a name="get-recent-user-activities"></a><span data-ttu-id="f0657-109">Получать последние действия пользователя</span><span class="sxs-lookup"><span data-stu-id="f0657-109">Get recent user activities</span></span>

<span data-ttu-id="f0657-110">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0657-110">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0657-111">Получите последние действия для данного пользователя.</span><span class="sxs-lookup"><span data-stu-id="f0657-111">Get recent activities for a given user.</span></span> <span data-ttu-id="f0657-112">Эта функция OData имеет некоторые действия по умолчанию, включаемые, чтобы заставить ее работать как API "последнего времени".</span><span class="sxs-lookup"><span data-stu-id="f0657-112">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="f0657-113">Служба запрашивает последние [historyItems,](../resources/projectrome-historyitem.md)а затем вытягивает связанные действия.</span><span class="sxs-lookup"><span data-stu-id="f0657-113">The service will query for the most recent [historyItems](../resources/projectrome-historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="f0657-114">Действия будут сортироваться в соответствии с последним **lastModified** на **historyItem**.</span><span class="sxs-lookup"><span data-stu-id="f0657-114">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="f0657-115">Это означает, что действия без **historyItems** не будут включены в ответ.</span><span class="sxs-lookup"><span data-stu-id="f0657-115">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="f0657-116">Разрешение UserActivity.ReadWrite.CreatedByApp также применяет дополнительную фильтрацию к ответу, чтобы возвращались только действия, созданные вашим приложением.</span><span class="sxs-lookup"><span data-stu-id="f0657-116">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="f0657-117">Это фильтрация на стороне сервера может привести к пустым страницам, если пользователь особенно активен, а другие приложения создали более последние действия.</span><span class="sxs-lookup"><span data-stu-id="f0657-117">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="f0657-118">Чтобы получить действия приложения, используйте свойство **nextLink** для пагинации.</span><span class="sxs-lookup"><span data-stu-id="f0657-118">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0657-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0657-119">Permissions</span></span>

<span data-ttu-id="f0657-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0657-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0657-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0657-122">Permission type</span></span>      | <span data-ttu-id="f0657-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0657-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0657-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0657-124">Delegated (work or school account)</span></span> | <span data-ttu-id="f0657-125">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="f0657-125">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="f0657-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0657-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0657-127">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="f0657-127">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="f0657-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0657-128">Application</span></span> | <span data-ttu-id="f0657-129">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0657-129">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0657-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0657-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0657-131">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f0657-131">Optional query parameters</span></span>

<span data-ttu-id="f0657-132">Этот метод поддерживает некоторые [параметры запроса OData для](/graph/query-parameters) настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f0657-132">This method supports some [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="f0657-133">Поддерживаются следующие параметры запроса:</span><span class="sxs-lookup"><span data-stu-id="f0657-133">The following query parameters are supported:</span></span>

- <span data-ttu-id="f0657-134">$expand для свойства **навигации historyItems.**</span><span class="sxs-lookup"><span data-stu-id="f0657-134">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="f0657-135">$top ограничить максимальное количество элементов на страницах.</span><span class="sxs-lookup"><span data-stu-id="f0657-135">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="f0657-136">$filter в **свойстве lastModifiedDateTime** для  действий или **historyItems,** если они расширены.</span><span class="sxs-lookup"><span data-stu-id="f0657-136">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="f0657-137">Ниже приводится несколько примеров поддерживаемых запросов с кодией URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="f0657-137">The following are some examples of supported queries with URL encoding.</span></span>

```http
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="f0657-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0657-138">Request headers</span></span>

|<span data-ttu-id="f0657-139">Имя</span><span class="sxs-lookup"><span data-stu-id="f0657-139">Name</span></span> | <span data-ttu-id="f0657-140">Тип</span><span class="sxs-lookup"><span data-stu-id="f0657-140">Type</span></span> | <span data-ttu-id="f0657-141">Описание</span><span class="sxs-lookup"><span data-stu-id="f0657-141">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="f0657-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0657-142">Authorization</span></span> | <span data-ttu-id="f0657-143">string</span><span class="sxs-lookup"><span data-stu-id="f0657-143">string</span></span> | <span data-ttu-id="f0657-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0657-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0657-146">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0657-146">Request body</span></span>

<span data-ttu-id="f0657-147">Не укажите тело запроса.</span><span class="sxs-lookup"><span data-stu-id="f0657-147">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="f0657-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0657-148">Response</span></span>

<span data-ttu-id="f0657-149">В случае успешной работы этот метод возвращает код ответа с последними действиями пользователя `200 OK` для приложения.</span><span class="sxs-lookup"><span data-stu-id="f0657-149">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="f0657-150">Пример</span><span class="sxs-lookup"><span data-stu-id="f0657-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0657-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0657-151">Request</span></span>

<span data-ttu-id="f0657-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0657-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities/recent
```

### <a name="response"></a><span data-ttu-id="f0657-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0657-153">Response</span></span>

<span data-ttu-id="f0657-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f0657-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.activity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(userActivity)",
   "@odata.nextLink":"https://graph.microsoft.com/beta/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
   "value":[
      {
         "@odata.type":"#microsoft.graph.activity",
         "activitySourceHost":"https://www.contoso.com",
         "createdDateTime":"2018-02-26T18:34:29.592Z",
         "lastModifiedDateTime":"2018-02-26T18:34:29.607Z",
         "id":"5347642601316252694",
         "appActivityId":"/article?12345",
         "visualElements":{
            "attribution":{
               "iconUrl":"https://www.contoso.com/icon",
               "alternateText":"Contoso, Ltd.",
               "addImageQuery":"false"
            },
            "displayText":"Contoso How-To: How to Tie a Reef Knot",
            "description":"How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
            "backgroundColor":"#ff0000",
            "content":{
               "$schema":"https://adaptivecards.io/schemas/adaptive-card.json",
               "type":"AdaptiveCard",
               "body":[
                  {
                     "type":"TextBlock",
                     "text":"Contoso MainPage"
                  }
               ]
            }
         },
         "activationUrl":"https://www.contoso.com/article?id=12345",
         "appDisplayName":"Contoso, Ltd.",
         "userTimezone":"Africa/Casablanca",
         "fallbackUrl":"https://www.contoso.com/article?id=12345",
         "contentUrl":"https://www.contoso.com/article?id=12345",
         "contentInfo":{
            "@context":"https://schema.org",
            "@type":"Article",
            "author":"John Doe",
            "name":"How to Tie a Reef Knot"
         },
         "expirationDateTime":"2018-03-28T18:34:29.607Z",
         "status":"updated"
      }
   ]
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
