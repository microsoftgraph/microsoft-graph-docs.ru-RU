---
title: Список timesOff
description: Получите список timesOff в этом расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aec47b6dcd27c9e9b05a4794e1fdef3465e06eec
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036676"
---
# <a name="list-timesoff"></a><span data-ttu-id="3c560-103">Список timesOff</span><span class="sxs-lookup"><span data-stu-id="3c560-103">List timesOff</span></span>

<span data-ttu-id="3c560-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c560-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c560-105">Получите список экземпляров [timeOff](../resources/timeoff.md) в [расписании.](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="3c560-105">Get the list of [timeOff](../resources/timeoff.md) instances in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3c560-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c560-106">Permissions</span></span>

<span data-ttu-id="3c560-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c560-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c560-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c560-109">Permission type</span></span>      | <span data-ttu-id="3c560-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c560-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c560-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c560-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3c560-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c560-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3c560-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c560-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c560-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c560-114">Not supported.</span></span>    |
|<span data-ttu-id="3c560-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c560-115">Application</span></span> | <span data-ttu-id="3c560-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c560-116">Not supported.</span></span> |

> <span data-ttu-id="3c560-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="3c560-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3c560-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="3c560-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3c560-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c560-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3c560-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3c560-120">Optional query parameters</span></span>
<span data-ttu-id="3c560-121">Этот метод поддерживает параметр запроса $filter [OData,](/graph/query-parameters) чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="3c560-121">This method supports the $filter [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c560-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c560-122">Request headers</span></span>

| <span data-ttu-id="3c560-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c560-123">Header</span></span>       | <span data-ttu-id="3c560-124">Значение</span><span class="sxs-lookup"><span data-stu-id="3c560-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3c560-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c560-125">Authorization</span></span>  | <span data-ttu-id="3c560-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c560-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3c560-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3c560-128">Content-Type</span></span>  | <span data-ttu-id="3c560-129">application/json</span><span class="sxs-lookup"><span data-stu-id="3c560-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3c560-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c560-130">Request body</span></span>
<span data-ttu-id="3c560-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c560-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c560-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c560-132">Response</span></span>

<span data-ttu-id="3c560-133">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [timeOff](../resources/timeoff.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3c560-133">If successful, this method returns a `200 OK` response code and a collection of [timeOff](../resources/timeoff.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c560-134">Пример</span><span class="sxs-lookup"><span data-stu-id="3c560-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3c560-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c560-135">Request</span></span>

<span data-ttu-id="3c560-136">Ниже приводится пример запроса, который получает все объекты **timeOff,** которые имеют общую версию и черновик версии в период с 11 марта по 18 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="3c560-136">The following is an example of a request that gets all **timeOff** objects that have a shared version and a draft version between March 11 - March 18, 2019.</span></span>

# <a name="http"></a>[<span data-ttu-id="3c560-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c560-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-timesoff"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff?$filter=sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z
```
# <a name="c"></a>[<span data-ttu-id="3c560-138">C#</span><span class="sxs-lookup"><span data-stu-id="3c560-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-timesoff-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c560-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c560-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-timesoff-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c560-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c560-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-timesoff-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c560-141">Java</span><span class="sxs-lookup"><span data-stu-id="3c560-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-list-timesoff-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3c560-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c560-142">Response</span></span>

<span data-ttu-id="3c560-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3c560-143">The following is an example of the response.</span></span> 

><span data-ttu-id="3c560-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3c560-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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


