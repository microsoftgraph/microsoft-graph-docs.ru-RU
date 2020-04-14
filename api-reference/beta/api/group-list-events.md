---
title: Список событий
description: Получение списка, включающего объекты событий.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b748151247dbca6c85ad1b0f089676315a9e7be6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43396972"
---
# <a name="list-events"></a><span data-ttu-id="22f11-103">Перечисление событий</span><span class="sxs-lookup"><span data-stu-id="22f11-103">List events</span></span>

<span data-ttu-id="22f11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22f11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22f11-105">Получение списка объектов [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="22f11-105">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="22f11-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22f11-106">Permissions</span></span>
<span data-ttu-id="22f11-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22f11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22f11-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22f11-109">Permission type</span></span>      | <span data-ttu-id="22f11-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22f11-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22f11-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22f11-111">Delegated (work or school account)</span></span> | <span data-ttu-id="22f11-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22f11-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="22f11-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22f11-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22f11-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22f11-114">Not supported.</span></span>    |
|<span data-ttu-id="22f11-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22f11-115">Application</span></span> | <span data-ttu-id="22f11-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22f11-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22f11-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22f11-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22f11-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="22f11-118">Optional query parameters</span></span>
<span data-ttu-id="22f11-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="22f11-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22f11-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22f11-120">Request headers</span></span>
| <span data-ttu-id="22f11-121">Имя</span><span class="sxs-lookup"><span data-stu-id="22f11-121">Name</span></span>       | <span data-ttu-id="22f11-122">Тип</span><span class="sxs-lookup"><span data-stu-id="22f11-122">Type</span></span> | <span data-ttu-id="22f11-123">Описание</span><span class="sxs-lookup"><span data-stu-id="22f11-123">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="22f11-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="22f11-124">Authorization</span></span>  | <span data-ttu-id="22f11-125">string</span><span class="sxs-lookup"><span data-stu-id="22f11-125">string</span></span> | <span data-ttu-id="22f11-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22f11-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="22f11-128">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="22f11-128">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="22f11-129">string</span><span class="sxs-lookup"><span data-stu-id="22f11-129">string</span></span> | <span data-ttu-id="22f11-130">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="22f11-130">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="22f11-131">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="22f11-131">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="22f11-132">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="22f11-132">Optional.</span></span> |
| <span data-ttu-id="22f11-133">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="22f11-133">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="22f11-134">string</span><span class="sxs-lookup"><span data-stu-id="22f11-134">string</span></span> | <span data-ttu-id="22f11-135">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="22f11-135">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="22f11-136">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="22f11-136">Values can be "text" or "html".</span></span> <span data-ttu-id="22f11-137">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="22f11-137">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="22f11-138">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="22f11-138">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="22f11-139">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="22f11-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22f11-140">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="22f11-140">Request body</span></span>
<span data-ttu-id="22f11-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22f11-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22f11-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="22f11-142">Response</span></span>
<span data-ttu-id="22f11-143">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="22f11-143">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22f11-144">Пример</span><span class="sxs-lookup"><span data-stu-id="22f11-144">Example</span></span>
#### <a name="request"></a><span data-ttu-id="22f11-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="22f11-145">Request</span></span>
<span data-ttu-id="22f11-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22f11-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="22f11-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="22f11-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/events
```
# <a name="c"></a>[<span data-ttu-id="22f11-148">C#</span><span class="sxs-lookup"><span data-stu-id="22f11-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22f11-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22f11-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22f11-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22f11-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="22f11-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="22f11-151">Response</span></span>
<span data-ttu-id="22f11-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22f11-152">The following is an example of the response.</span></span>
><span data-ttu-id="22f11-153">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="22f11-153">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="22f11-154">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22f11-154">All the properties will be returned from an actual call.</span></span>
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
