---
title: Список календарей
description: Получение списка календарей, входящих в группу.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 492844e76005456865a455ec90f88eb295bdfcea
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443751"
---
# <a name="list-calendars"></a><span data-ttu-id="fa68d-103">Список календарей</span><span class="sxs-lookup"><span data-stu-id="fa68d-103">List calendars</span></span>

<span data-ttu-id="fa68d-104">Получение списка календарей, входящих в группу.</span><span class="sxs-lookup"><span data-stu-id="fa68d-104">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa68d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa68d-105">Permissions</span></span>

<span data-ttu-id="fa68d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa68d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa68d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa68d-108">Permission type</span></span>                        | <span data-ttu-id="fa68d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa68d-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="fa68d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa68d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa68d-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fa68d-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="fa68d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa68d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa68d-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fa68d-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="fa68d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa68d-114">Application</span></span>                            | <span data-ttu-id="fa68d-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fa68d-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="fa68d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa68d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="fa68d-117">Объект [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="fa68d-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="fa68d-118">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="fa68d-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa68d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fa68d-119">Optional query parameters</span></span>

<span data-ttu-id="fa68d-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fa68d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa68d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa68d-121">Request headers</span></span>

| <span data-ttu-id="fa68d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="fa68d-122">Name</span></span>          | <span data-ttu-id="fa68d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="fa68d-123">Type</span></span>   | <span data-ttu-id="fa68d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="fa68d-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="fa68d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa68d-125">Authorization</span></span> | <span data-ttu-id="fa68d-126">string</span><span class="sxs-lookup"><span data-stu-id="fa68d-126">string</span></span> | <span data-ttu-id="fa68d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa68d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa68d-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fa68d-129">Request body</span></span>

<span data-ttu-id="fa68d-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa68d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa68d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa68d-131">Response</span></span>

<span data-ttu-id="fa68d-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa68d-132">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa68d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fa68d-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fa68d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa68d-134">Request</span></span>

<span data-ttu-id="fa68d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa68d-135">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fa68d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa68d-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fa68d-137">C#</span><span class="sxs-lookup"><span data-stu-id="fa68d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa68d-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="fa68d-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa68d-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fa68d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fa68d-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa68d-140">Response</span></span>

<span data-ttu-id="fa68d-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa68d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
