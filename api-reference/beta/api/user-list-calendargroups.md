---
title: Список объектов calendarGroup
description: Получение групп календарей пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 96bd77a390fdebfa004d854d740d12fe32feb750
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867544"
---
# <a name="list-calendargroups"></a><span data-ttu-id="08efd-103">Список объектов calendarGroup</span><span class="sxs-lookup"><span data-stu-id="08efd-103">List calendarGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08efd-104">Получение групп календарей пользователя.</span><span class="sxs-lookup"><span data-stu-id="08efd-104">Get the user's calendar groups.</span></span>
## <a name="permissions"></a><span data-ttu-id="08efd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08efd-105">Permissions</span></span>
<span data-ttu-id="08efd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08efd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08efd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08efd-108">Permission type</span></span>      | <span data-ttu-id="08efd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08efd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08efd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08efd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="08efd-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08efd-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="08efd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08efd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08efd-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08efd-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="08efd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08efd-114">Application</span></span> | <span data-ttu-id="08efd-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08efd-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="08efd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08efd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups
GET /users/{id | userPrincipalName}/calendarGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="08efd-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="08efd-117">Optional query parameters</span></span>
<span data-ttu-id="08efd-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="08efd-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="08efd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08efd-119">Request headers</span></span>
| <span data-ttu-id="08efd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08efd-120">Header</span></span>       | <span data-ttu-id="08efd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="08efd-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="08efd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08efd-122">Authorization</span></span>  | <span data-ttu-id="08efd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08efd-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="08efd-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08efd-125">Content-Type</span></span>  | <span data-ttu-id="08efd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08efd-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="08efd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="08efd-127">Request body</span></span>
<span data-ttu-id="08efd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08efd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08efd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="08efd-129">Response</span></span>

<span data-ttu-id="08efd-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [CalendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08efd-130">If successful, this method returns a `200 OK` response code and collection of [CalendarGroup](../resources/calendargroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="08efd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="08efd-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08efd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="08efd-132">Request</span></span>
<span data-ttu-id="08efd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08efd-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="08efd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="08efd-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendargroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendarGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="08efd-135">C#</span><span class="sxs-lookup"><span data-stu-id="08efd-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendargroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="08efd-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="08efd-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendargroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="08efd-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="08efd-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendargroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="08efd-138">Java</span><span class="sxs-lookup"><span data-stu-id="08efd-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendargroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="08efd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="08efd-139">Response</span></span>
<span data-ttu-id="08efd-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08efd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
