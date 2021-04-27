---
title: Перечисление смен
description: Получите список сдвигов в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0565f3e0d5e81bf7bc8cc3c9f153935a01bf90e6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050887"
---
# <a name="list-shifts"></a><span data-ttu-id="fef43-103">Перечисление смен</span><span class="sxs-lookup"><span data-stu-id="fef43-103">List shifts</span></span>

<span data-ttu-id="fef43-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fef43-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="fef43-105">Получите список [экземпляров смены](../resources/shift.md) в [расписании.](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="fef43-105">Get the list of [shift](../resources/shift.md) instances in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fef43-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fef43-106">Permissions</span></span>

<span data-ttu-id="fef43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fef43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fef43-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fef43-109">Permission type</span></span>      | <span data-ttu-id="fef43-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fef43-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fef43-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fef43-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fef43-112">Schedule.Read.All, Group.Read.All,Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fef43-112">Schedule.Read.All, Group.Read.All,Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fef43-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fef43-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fef43-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fef43-114">Not supported.</span></span>    |
|<span data-ttu-id="fef43-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="fef43-115">Application</span></span> | <span data-ttu-id="fef43-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fef43-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fef43-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fef43-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fef43-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fef43-118">Optional query parameters</span></span>
<span data-ttu-id="fef43-119">Этот метод поддерживает параметр запроса $filter [OData,](/graph/query-parameters) чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="fef43-119">This method supports the $filter [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fef43-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fef43-120">Request headers</span></span>

| <span data-ttu-id="fef43-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fef43-121">Header</span></span>       | <span data-ttu-id="fef43-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fef43-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fef43-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fef43-123">Authorization</span></span>  | <span data-ttu-id="fef43-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fef43-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fef43-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fef43-126">Request body</span></span>
<span data-ttu-id="fef43-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fef43-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fef43-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fef43-128">Response</span></span>

<span data-ttu-id="fef43-129">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [переноса](../resources/shift.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fef43-129">If successful, this method returns a `200 OK` response code and a collection of [shift](../resources/shift.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fef43-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fef43-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fef43-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fef43-131">Request</span></span>

<span data-ttu-id="fef43-132">Ниже приводится пример запроса,  который получает все объекты переноса, которые имеют общую версию и черновик версии в период с 11 марта по 18 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="fef43-132">The following is an example of a request that gets all **shift** objects that have a shared version and a draft version between March 11 - March 18, 2019.</span></span>

# <a name="http"></a>[<span data-ttu-id="fef43-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fef43-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-shifts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts?$filter=sharedShift/startDateTime ge 2019-03-11T00:00:00.000Z and sharedShift/endDateTime le 2019-03-18T00:00:00.000Z and draftShift/startDateTime ge 2019-03-11T00:00:00.000Z and draftShift/endDateTime le 2019-03-18T00:00:00.000Z
```
# <a name="c"></a>[<span data-ttu-id="fef43-134">C#</span><span class="sxs-lookup"><span data-stu-id="fef43-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-shifts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fef43-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fef43-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-shifts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fef43-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fef43-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-shifts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fef43-137">Java</span><span class="sxs-lookup"><span data-stu-id="fef43-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-list-shifts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fef43-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fef43-138">Response</span></span>

<span data-ttu-id="fef43-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fef43-139">The following is an example of the response.</span></span> 

><span data-ttu-id="fef43-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fef43-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "value": [
    {
      "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
      "createdDateTime": "2019-03-14T04:32:51.451Z",
      "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
      "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
      "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
      "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
          "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
          "displayName": "John Doe"
        }
      },
      "sharedShift": {
        "displayName": "Day shift",
        "notes": "Please do inventory as part of your shift.",
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-12T00:00:00Z",
        "theme": "blue",
        "activities": [
          {
            "isPaid": true,
            "startDateTime": "2019-03-11T15:00:00Z",
            "endDateTime": "2019-03-11T15:15:00Z",
            "code": "",
            "displayName": "Lunch"
          }
        ]
      },
      "draftShift": {
        "displayName": "Day shift",
        "notes": "Please do inventory as part of your shift.",
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-12T00:00:00Z",
        "theme": "blue",
        "activities": [
          {
            "isPaid": true,
            "startDateTime": "2019-03-11T15:00:00Z",
            "endDateTime": "2019-03-11T15:30:00Z",
            "code": "",
            "displayName": "Lunch"
          }
        ]
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
  "description": "Get the list of shifts in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


