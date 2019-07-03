---
title: Список Тимесофф
description: Получение списка Тимесофф в этом расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f1f91490eb08d6ebebbed7187c3c4bf5bb05df0f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450354"
---
# <a name="list-timesoff"></a><span data-ttu-id="8f6a8-103">Список Тимесофф</span><span class="sxs-lookup"><span data-stu-id="8f6a8-103">List timesOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f6a8-104">Получение списка экземпляров [тимеофф](../resources/timeoff.md) по расписанию. [](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="8f6a8-104">Get the list of [timeOff](../resources/timeoff.md) instances in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8f6a8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f6a8-105">Permissions</span></span>

<span data-ttu-id="8f6a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f6a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f6a8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f6a8-108">Permission type</span></span>      | <span data-ttu-id="8f6a8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f6a8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f6a8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f6a8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8f6a8-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f6a8-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8f6a8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f6a8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f6a8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-113">Not supported.</span></span>    |
|<span data-ttu-id="8f6a8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f6a8-114">Application</span></span> | <span data-ttu-id="8f6a8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-115">Not supported.</span></span> |

> <span data-ttu-id="8f6a8-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8f6a8-117">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8f6a8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f6a8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8f6a8-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8f6a8-119">Optional query parameters</span></span>
<span data-ttu-id="8f6a8-120">Этот метод поддерживает $filter [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-120">This method supports the $filter [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f6a8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f6a8-121">Request headers</span></span>

| <span data-ttu-id="8f6a8-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f6a8-122">Header</span></span>       | <span data-ttu-id="8f6a8-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8f6a8-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8f6a8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f6a8-124">Authorization</span></span>  | <span data-ttu-id="8f6a8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8f6a8-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f6a8-127">Content-Type</span></span>  | <span data-ttu-id="8f6a8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8f6a8-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8f6a8-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8f6a8-129">Request body</span></span>
<span data-ttu-id="8f6a8-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f6a8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f6a8-131">Response</span></span>

<span data-ttu-id="8f6a8-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [тимеофф](../resources/timeoff.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-132">If successful, this method returns a `200 OK` response code and a collection of [timeOff](../resources/timeoff.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f6a8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8f6a8-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8f6a8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f6a8-134">Request</span></span>

<span data-ttu-id="8f6a8-135">Ниже приведен пример запроса, который получает все объекты **тимеофф** с общей версией и черновой версией в диапазоне от 11 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-135">The following is an example of a request that gets all **timeOff** objects that have a shared version and a draft version between March 11 - March 18, 2019.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8f6a8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f6a8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-timesoff"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff?$filter=sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f6a8-137">C#</span><span class="sxs-lookup"><span data-stu-id="8f6a8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-timesoff-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f6a8-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="8f6a8-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-timesoff-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f6a8-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8f6a8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-timesoff-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8f6a8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f6a8-140">Response</span></span>

<span data-ttu-id="8f6a8-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-141">The following is an example of the response.</span></span> 

><span data-ttu-id="8f6a8-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f6a8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOff",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "value": [
    {
      "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
      "createdDateTime": "2019-03-14T05:35:57.755Z",
      "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
      "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
          "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
          "displayName": "John Doe"
        }
      },
      "sharedTimeOff": {
        "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
        "startDateTime": "2019-03-11T07:00:00Z",
        "endDateTime": "2019-03-12T07:00:00Z",
        "theme": "white"
      },
      "draftTimeOff": {
        "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
        "startDateTime": "2019-03-11T07:00:00Z",
        "endDateTime": "2019-03-12T07:00:00Z",
        "theme": "pink"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the list of timesOff in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
