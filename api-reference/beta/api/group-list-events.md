---
title: Список событий
description: Получение списка, включающего объекты событий.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 32051d6192d9de8e692c063011933a951d4fe4bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809305"
---
# <a name="list-events"></a><span data-ttu-id="c78fe-103">Список событий</span><span class="sxs-lookup"><span data-stu-id="c78fe-103">List events</span></span>

> <span data-ttu-id="c78fe-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c78fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c78fe-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c78fe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c78fe-106">Получение списка объектов [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="c78fe-106">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c78fe-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c78fe-107">Permissions</span></span>
<span data-ttu-id="c78fe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c78fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c78fe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c78fe-110">Permission type</span></span>      | <span data-ttu-id="c78fe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c78fe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c78fe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c78fe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c78fe-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c78fe-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c78fe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c78fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c78fe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c78fe-115">Not supported.</span></span>    |
|<span data-ttu-id="c78fe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c78fe-116">Application</span></span> | <span data-ttu-id="c78fe-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c78fe-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c78fe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c78fe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c78fe-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c78fe-119">Optional query parameters</span></span>
<span data-ttu-id="c78fe-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c78fe-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c78fe-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c78fe-121">Request headers</span></span>
| <span data-ttu-id="c78fe-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c78fe-122">Name</span></span>       | <span data-ttu-id="c78fe-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c78fe-123">Type</span></span> | <span data-ttu-id="c78fe-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c78fe-124">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="c78fe-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c78fe-125">Authorization</span></span>  | <span data-ttu-id="c78fe-126">string</span><span class="sxs-lookup"><span data-stu-id="c78fe-126">string</span></span> | <span data-ttu-id="c78fe-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c78fe-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c78fe-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="c78fe-129">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="c78fe-130">string</span><span class="sxs-lookup"><span data-stu-id="c78fe-130">string</span></span> | <span data-ttu-id="c78fe-131">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="c78fe-131">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="c78fe-132">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c78fe-132">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="c78fe-133">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c78fe-133">Optional.</span></span> |
| <span data-ttu-id="c78fe-134">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="c78fe-134">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="c78fe-135">string</span><span class="sxs-lookup"><span data-stu-id="c78fe-135">string</span></span> | <span data-ttu-id="c78fe-136">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="c78fe-136">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="c78fe-137">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="c78fe-137">Values can be "text" or "html".</span></span> <span data-ttu-id="c78fe-138">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="c78fe-138">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="c78fe-139">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="c78fe-139">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="c78fe-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c78fe-140">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c78fe-141">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c78fe-141">Request body</span></span>
<span data-ttu-id="c78fe-142">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c78fe-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c78fe-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c78fe-143">Response</span></span>
<span data-ttu-id="c78fe-144">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c78fe-144">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c78fe-145">Пример</span><span class="sxs-lookup"><span data-stu-id="c78fe-145">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c78fe-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="c78fe-146">Request</span></span>
<span data-ttu-id="c78fe-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c78fe-147">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/events
```

#### <a name="response"></a><span data-ttu-id="c78fe-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="c78fe-148">Response</span></span>
<span data-ttu-id="c78fe-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c78fe-149">The following is an example of the response.</span></span>
><span data-ttu-id="c78fe-150">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="c78fe-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c78fe-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c78fe-151">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List group events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
