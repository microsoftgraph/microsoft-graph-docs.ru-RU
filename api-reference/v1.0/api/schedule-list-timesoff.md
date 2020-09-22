---
title: Список Тимесофф
description: Получение списка Тимесофф в этом расписании.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4ac7eac13ef82da7d962e2a5306b37212870db0c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051265"
---
# <a name="list-timesoff"></a><span data-ttu-id="48adc-103">Список Тимесофф</span><span class="sxs-lookup"><span data-stu-id="48adc-103">List timesOff</span></span>

<span data-ttu-id="48adc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48adc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="48adc-105">Получение списка экземпляров [тимеофф](../resources/timeoff.md) по [расписанию](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="48adc-105">Get the list of [timeOff](../resources/timeoff.md) instances in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="48adc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48adc-106">Permissions</span></span>

<span data-ttu-id="48adc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48adc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48adc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48adc-109">Permission type</span></span>      | <span data-ttu-id="48adc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48adc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48adc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48adc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="48adc-112">Schedule. Read. ALL, Group. Read. ALL, Schedule. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="48adc-112">Schedule.Read.All, Group.Read.All,Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="48adc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48adc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48adc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48adc-114">Not supported.</span></span>    |
|<span data-ttu-id="48adc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48adc-115">Application</span></span> | <span data-ttu-id="48adc-116">Schedule. Read. ALL, Schedule. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="48adc-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="48adc-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="48adc-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="48adc-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="48adc-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="48adc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48adc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff
```
## <a name="optional-query-parameters"></a><span data-ttu-id="48adc-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="48adc-120">Optional query parameters</span></span>
<span data-ttu-id="48adc-121">Этот метод поддерживает `$filter` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="48adc-121">This method supports the `$filter` [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48adc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48adc-122">Request headers</span></span>

| <span data-ttu-id="48adc-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48adc-123">Header</span></span>       | <span data-ttu-id="48adc-124">Значение</span><span class="sxs-lookup"><span data-stu-id="48adc-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="48adc-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48adc-125">Authorization</span></span>  | <span data-ttu-id="48adc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48adc-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="48adc-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48adc-128">Request body</span></span>
<span data-ttu-id="48adc-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48adc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48adc-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="48adc-130">Response</span></span>

<span data-ttu-id="48adc-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [тимеофф](../resources/timeoff.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48adc-131">If successful, this method returns a `200 OK` response code and a collection of [timeOff](../resources/timeoff.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48adc-132">Пример</span><span class="sxs-lookup"><span data-stu-id="48adc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="48adc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="48adc-133">Request</span></span>

<span data-ttu-id="48adc-134">Ниже приведен пример запроса, который получает все объекты **тимеофф** с общей версией и черновой версией в диапазоне от 11 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="48adc-134">The following is an example of a request that gets all **timeOff** objects that have a shared version and a draft version between March 11 - March 18, 2019.</span></span>


# <a name="http"></a>[<span data-ttu-id="48adc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="48adc-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-timesoff"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timesOff?$filter=sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z
```
# <a name="c"></a>[<span data-ttu-id="48adc-136">C#</span><span class="sxs-lookup"><span data-stu-id="48adc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-timesoff-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48adc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48adc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-timesoff-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48adc-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48adc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-timesoff-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="48adc-139">Java</span><span class="sxs-lookup"><span data-stu-id="48adc-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-list-timesoff-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="48adc-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="48adc-140">Response</span></span>

<span data-ttu-id="48adc-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="48adc-141">The following is an example of the response.</span></span> 

><span data-ttu-id="48adc-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48adc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

