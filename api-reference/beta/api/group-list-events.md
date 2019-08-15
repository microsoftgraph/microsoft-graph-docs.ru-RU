---
title: Список событий
description: Получение списка, включающего объекты событий.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: bd8b99367c66e5879a40aade9a893b1108ae350d
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420209"
---
# <a name="list-events"></a><span data-ttu-id="19f5b-103">Список событий</span><span class="sxs-lookup"><span data-stu-id="19f5b-103">List events</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19f5b-104">Получение списка объектов [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="19f5b-104">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="19f5b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19f5b-105">Permissions</span></span>
<span data-ttu-id="19f5b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19f5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19f5b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19f5b-108">Permission type</span></span>      | <span data-ttu-id="19f5b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19f5b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19f5b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19f5b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="19f5b-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19f5b-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="19f5b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19f5b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19f5b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19f5b-113">Not supported.</span></span>    |
|<span data-ttu-id="19f5b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19f5b-114">Application</span></span> | <span data-ttu-id="19f5b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19f5b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19f5b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19f5b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19f5b-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="19f5b-117">Optional query parameters</span></span>
<span data-ttu-id="19f5b-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="19f5b-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19f5b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19f5b-119">Request headers</span></span>
| <span data-ttu-id="19f5b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="19f5b-120">Name</span></span>       | <span data-ttu-id="19f5b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="19f5b-121">Type</span></span> | <span data-ttu-id="19f5b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="19f5b-122">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="19f5b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="19f5b-123">Authorization</span></span>  | <span data-ttu-id="19f5b-124">string</span><span class="sxs-lookup"><span data-stu-id="19f5b-124">string</span></span> | <span data-ttu-id="19f5b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19f5b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="19f5b-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="19f5b-127">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="19f5b-128">string</span><span class="sxs-lookup"><span data-stu-id="19f5b-128">string</span></span> | <span data-ttu-id="19f5b-129">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="19f5b-129">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="19f5b-130">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="19f5b-130">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="19f5b-131">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="19f5b-131">Optional.</span></span> |
| <span data-ttu-id="19f5b-132">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="19f5b-132">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="19f5b-133">string</span><span class="sxs-lookup"><span data-stu-id="19f5b-133">string</span></span> | <span data-ttu-id="19f5b-134">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="19f5b-134">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="19f5b-135">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="19f5b-135">Values can be "text" or "html".</span></span> <span data-ttu-id="19f5b-136">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="19f5b-136">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="19f5b-137">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="19f5b-137">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="19f5b-138">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="19f5b-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19f5b-139">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="19f5b-139">Request body</span></span>
<span data-ttu-id="19f5b-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="19f5b-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19f5b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="19f5b-141">Response</span></span>
<span data-ttu-id="19f5b-142">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="19f5b-142">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19f5b-143">Пример</span><span class="sxs-lookup"><span data-stu-id="19f5b-143">Example</span></span>
#### <a name="request"></a><span data-ttu-id="19f5b-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="19f5b-144">Request</span></span>
<span data-ttu-id="19f5b-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19f5b-145">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="19f5b-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="19f5b-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/events
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="19f5b-147">C#</span><span class="sxs-lookup"><span data-stu-id="19f5b-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19f5b-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19f5b-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19f5b-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="19f5b-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="19f5b-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="19f5b-150">Response</span></span>
<span data-ttu-id="19f5b-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="19f5b-151">The following is an example of the response.</span></span>
><span data-ttu-id="19f5b-152">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="19f5b-152">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="19f5b-153">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19f5b-153">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "",
        "time": "2016-10-19T10:37:00Z"
      },
      "uid": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List group events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
