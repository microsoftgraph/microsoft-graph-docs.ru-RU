---
title: Список календарей
description: Получение списка календарей, входящих в группу.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6f4fc5997e3ec93e757137822742c281e39b506a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264703"
---
# <a name="list-calendars"></a><span data-ttu-id="bcce9-103">Список календарей</span><span class="sxs-lookup"><span data-stu-id="bcce9-103">List calendars</span></span>

<span data-ttu-id="bcce9-104">Получение списка календарей, входящих в группу.</span><span class="sxs-lookup"><span data-stu-id="bcce9-104">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcce9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bcce9-105">Permissions</span></span>

<span data-ttu-id="bcce9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcce9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bcce9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcce9-108">Permission type</span></span>                        | <span data-ttu-id="bcce9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcce9-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="bcce9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcce9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bcce9-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bcce9-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="bcce9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcce9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcce9-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bcce9-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="bcce9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcce9-114">Application</span></span>                            | <span data-ttu-id="bcce9-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bcce9-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="bcce9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcce9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="bcce9-117">Объект [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="bcce9-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="bcce9-118">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="bcce9-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bcce9-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bcce9-119">Optional query parameters</span></span>

<span data-ttu-id="bcce9-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bcce9-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bcce9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcce9-121">Request headers</span></span>

| <span data-ttu-id="bcce9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="bcce9-122">Name</span></span>          | <span data-ttu-id="bcce9-123">Тип</span><span class="sxs-lookup"><span data-stu-id="bcce9-123">Type</span></span>   | <span data-ttu-id="bcce9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="bcce9-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="bcce9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcce9-125">Authorization</span></span> | <span data-ttu-id="bcce9-126">string</span><span class="sxs-lookup"><span data-stu-id="bcce9-126">string</span></span> | <span data-ttu-id="bcce9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcce9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bcce9-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bcce9-129">Request body</span></span>

<span data-ttu-id="bcce9-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bcce9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcce9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcce9-131">Response</span></span>

<span data-ttu-id="bcce9-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bcce9-132">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcce9-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bcce9-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bcce9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcce9-134">Request</span></span>

<span data-ttu-id="bcce9-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcce9-135">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
```

##### <a name="response"></a><span data-ttu-id="bcce9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcce9-136">Response</span></span>

<span data-ttu-id="bcce9-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bcce9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 147

{
  "value": [
    {
      "name": "name-value",
      "color": {
      },
      "changeKey": "changeKey-value",
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bcce9-140">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="bcce9-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bcce9-141">C#</span><span class="sxs-lookup"><span data-stu-id="bcce9-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_calendars-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bcce9-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="bcce9-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_calendars-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bcce9-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bcce9-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_calendars-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/calendargroup-list-calendars.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/calendargroup-list-calendars.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/calendargroup-list-calendars.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
