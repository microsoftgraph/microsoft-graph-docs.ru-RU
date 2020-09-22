---
title: Список календарей
description: Получение списка календарей, входящих в группу.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 13b3899b1631230798a0324f29e573dc0e6ac829
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987577"
---
# <a name="list-calendars"></a><span data-ttu-id="a3e19-103">Список календарей</span><span class="sxs-lookup"><span data-stu-id="a3e19-103">List calendars</span></span>

<span data-ttu-id="a3e19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3e19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3e19-105">Получение списка календарей, входящих в группу.</span><span class="sxs-lookup"><span data-stu-id="a3e19-105">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3e19-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a3e19-106">Permissions</span></span>

<span data-ttu-id="a3e19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3e19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a3e19-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3e19-109">Permission type</span></span>                        | <span data-ttu-id="a3e19-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3e19-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a3e19-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3e19-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a3e19-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a3e19-112">Calendars.Read</span></span>                              |
| <span data-ttu-id="a3e19-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3e19-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3e19-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a3e19-114">Calendars.Read</span></span>                              |
| <span data-ttu-id="a3e19-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3e19-115">Application</span></span>                            | <span data-ttu-id="a3e19-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a3e19-116">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="a3e19-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3e19-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="a3e19-118">Объект [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a3e19-118">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="a3e19-119">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="a3e19-119">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3e19-120">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="a3e19-120">Optional query parameters</span></span>

<span data-ttu-id="a3e19-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a3e19-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3e19-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3e19-122">Request headers</span></span>

| <span data-ttu-id="a3e19-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a3e19-123">Name</span></span>          | <span data-ttu-id="a3e19-124">Тип</span><span class="sxs-lookup"><span data-stu-id="a3e19-124">Type</span></span>   | <span data-ttu-id="a3e19-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a3e19-125">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="a3e19-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3e19-126">Authorization</span></span> | <span data-ttu-id="a3e19-127">string</span><span class="sxs-lookup"><span data-stu-id="a3e19-127">string</span></span> | <span data-ttu-id="a3e19-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3e19-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3e19-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a3e19-130">Request body</span></span>

<span data-ttu-id="a3e19-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3e19-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3e19-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3e19-132">Response</span></span>

<span data-ttu-id="a3e19-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a3e19-133">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3e19-134">Пример</span><span class="sxs-lookup"><span data-stu-id="a3e19-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a3e19-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3e19-135">Request</span></span>

<span data-ttu-id="a3e19-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3e19-136">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a3e19-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3e19-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendargroup_get_calendars"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```
# <a name="c"></a>[<span data-ttu-id="a3e19-138">C#</span><span class="sxs-lookup"><span data-stu-id="a3e19-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendargroup-get-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3e19-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3e19-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendargroup-get-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3e19-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3e19-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendargroup-get-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a3e19-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3e19-141">Response</span></span>

<span data-ttu-id="a3e19-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3e19-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
      "calendarGroupId":"calendarGroupId-value",
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


