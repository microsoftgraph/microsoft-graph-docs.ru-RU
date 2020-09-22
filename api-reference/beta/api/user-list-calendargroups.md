---
title: Список объектов calendarGroup
description: Получение групп календарей пользователя.
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6da9158bec099a1bcd0ba9146b3c9e8fe325eaaf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017075"
---
# <a name="list-calendargroups"></a><span data-ttu-id="a4bf3-103">Список объектов calendarGroup</span><span class="sxs-lookup"><span data-stu-id="a4bf3-103">List calendarGroups</span></span>

<span data-ttu-id="a4bf3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4bf3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4bf3-105">Получение групп календарей пользователя.</span><span class="sxs-lookup"><span data-stu-id="a4bf3-105">Get the user's calendar groups.</span></span>
## <a name="permissions"></a><span data-ttu-id="a4bf3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4bf3-106">Permissions</span></span>
<span data-ttu-id="a4bf3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4bf3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4bf3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4bf3-109">Permission type</span></span>      | <span data-ttu-id="a4bf3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4bf3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4bf3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4bf3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a4bf3-112">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4bf3-112">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a4bf3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4bf3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4bf3-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4bf3-114">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a4bf3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4bf3-115">Application</span></span> | <span data-ttu-id="a4bf3-116">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4bf3-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4bf3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4bf3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups
GET /users/{id | userPrincipalName}/calendarGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a4bf3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a4bf3-118">Optional query parameters</span></span>
<span data-ttu-id="a4bf3-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a4bf3-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a4bf3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4bf3-120">Request headers</span></span>
| <span data-ttu-id="a4bf3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4bf3-121">Header</span></span>       | <span data-ttu-id="a4bf3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a4bf3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a4bf3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4bf3-123">Authorization</span></span>  | <span data-ttu-id="a4bf3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4bf3-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a4bf3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a4bf3-126">Content-Type</span></span>  | <span data-ttu-id="a4bf3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a4bf3-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a4bf3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4bf3-128">Request body</span></span>
<span data-ttu-id="a4bf3-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a4bf3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4bf3-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4bf3-130">Response</span></span>

<span data-ttu-id="a4bf3-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [CalendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a4bf3-131">If successful, this method returns a `200 OK` response code and collection of [CalendarGroup](../resources/calendargroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a4bf3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a4bf3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a4bf3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4bf3-133">Request</span></span>
<span data-ttu-id="a4bf3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4bf3-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a4bf3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4bf3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendargroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendarGroups
```
# <a name="c"></a>[<span data-ttu-id="a4bf3-136">C#</span><span class="sxs-lookup"><span data-stu-id="a4bf3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendargroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4bf3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4bf3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendargroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4bf3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4bf3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendargroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a4bf3-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4bf3-139">Response</span></span>
<span data-ttu-id="a4bf3-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4bf3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 155

{
  "value": [
    {
      "name": "name-value",
      "classId": "classId-value",
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
  "description": "List calendarGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


