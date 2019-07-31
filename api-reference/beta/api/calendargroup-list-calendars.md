---
title: Список календарей
description: Получение списка календарей, входящих в группу.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0e6faa71d202a49c1a6a55b1326748b6771214af
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944651"
---
# <a name="list-calendars"></a><span data-ttu-id="3dbde-103">Список календарей</span><span class="sxs-lookup"><span data-stu-id="3dbde-103">List calendars</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3dbde-104">Получение списка календарей, входящих в группу.</span><span class="sxs-lookup"><span data-stu-id="3dbde-104">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="3dbde-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3dbde-105">Permissions</span></span>

<span data-ttu-id="3dbde-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3dbde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3dbde-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3dbde-108">Permission type</span></span>                        | <span data-ttu-id="3dbde-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3dbde-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="3dbde-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3dbde-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3dbde-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3dbde-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="3dbde-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3dbde-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dbde-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3dbde-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="3dbde-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3dbde-114">Application</span></span>                            | <span data-ttu-id="3dbde-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3dbde-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="3dbde-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3dbde-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="3dbde-117">Объект [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="3dbde-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="3dbde-118">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="3dbde-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3dbde-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3dbde-119">Optional query parameters</span></span>

<span data-ttu-id="3dbde-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3dbde-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3dbde-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3dbde-121">Request headers</span></span>

| <span data-ttu-id="3dbde-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3dbde-122">Name</span></span>          | <span data-ttu-id="3dbde-123">Тип</span><span class="sxs-lookup"><span data-stu-id="3dbde-123">Type</span></span>   | <span data-ttu-id="3dbde-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3dbde-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="3dbde-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3dbde-125">Authorization</span></span> | <span data-ttu-id="3dbde-126">string</span><span class="sxs-lookup"><span data-stu-id="3dbde-126">string</span></span> | <span data-ttu-id="3dbde-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3dbde-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3dbde-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3dbde-129">Request body</span></span>

<span data-ttu-id="3dbde-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3dbde-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3dbde-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="3dbde-131">Response</span></span>

<span data-ttu-id="3dbde-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3dbde-132">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dbde-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3dbde-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3dbde-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3dbde-134">Request</span></span>

<span data-ttu-id="3dbde-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3dbde-135">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3dbde-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dbde-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendargroup_get_calendars"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3dbde-137">C#</span><span class="sxs-lookup"><span data-stu-id="3dbde-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendargroup-get-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3dbde-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="3dbde-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendargroup-get-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3dbde-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3dbde-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendargroup-get-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3dbde-140">Java</span><span class="sxs-lookup"><span data-stu-id="3dbde-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendargroup-get-calendars-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3dbde-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="3dbde-141">Response</span></span>

<span data-ttu-id="3dbde-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3dbde-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
