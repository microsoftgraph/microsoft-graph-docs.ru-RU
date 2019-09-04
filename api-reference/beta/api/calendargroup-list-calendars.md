---
title: Список календарей
description: Получение списка календарей, входящих в группу.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7db2208a2778c2bd014349c3b58774dee14ee8ef
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718741"
---
# <a name="list-calendars"></a><span data-ttu-id="9f10a-103">Список календарей</span><span class="sxs-lookup"><span data-stu-id="9f10a-103">List calendars</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f10a-104">Получение списка календарей, входящих в группу.</span><span class="sxs-lookup"><span data-stu-id="9f10a-104">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f10a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f10a-105">Permissions</span></span>

<span data-ttu-id="9f10a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f10a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f10a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f10a-108">Permission type</span></span>                        | <span data-ttu-id="9f10a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f10a-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="9f10a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f10a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f10a-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9f10a-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="9f10a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f10a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f10a-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9f10a-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="9f10a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f10a-114">Application</span></span>                            | <span data-ttu-id="9f10a-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9f10a-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="9f10a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f10a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="9f10a-117">Объект [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="9f10a-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="9f10a-118">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="9f10a-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f10a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9f10a-119">Optional query parameters</span></span>

<span data-ttu-id="9f10a-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9f10a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f10a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f10a-121">Request headers</span></span>

| <span data-ttu-id="9f10a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="9f10a-122">Name</span></span>          | <span data-ttu-id="9f10a-123">Тип</span><span class="sxs-lookup"><span data-stu-id="9f10a-123">Type</span></span>   | <span data-ttu-id="9f10a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9f10a-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="9f10a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f10a-125">Authorization</span></span> | <span data-ttu-id="9f10a-126">string</span><span class="sxs-lookup"><span data-stu-id="9f10a-126">string</span></span> | <span data-ttu-id="9f10a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f10a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f10a-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9f10a-129">Request body</span></span>

<span data-ttu-id="9f10a-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f10a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f10a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f10a-131">Response</span></span>

<span data-ttu-id="9f10a-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f10a-132">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f10a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9f10a-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9f10a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f10a-134">Request</span></span>

<span data-ttu-id="9f10a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f10a-135">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9f10a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f10a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendargroup_get_calendars"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9f10a-137">C#</span><span class="sxs-lookup"><span data-stu-id="9f10a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendargroup-get-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9f10a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f10a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendargroup-get-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9f10a-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9f10a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendargroup-get-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9f10a-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f10a-140">Response</span></span>

<span data-ttu-id="9f10a-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f10a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
