---
title: Список объектов calendarGroup
description: Получение групп календарей пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 797df667efc027f1270324be23bafd9ccb061ed1
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722029"
---
# <a name="list-calendargroups"></a><span data-ttu-id="40e3f-103">Список объектов calendarGroup</span><span class="sxs-lookup"><span data-stu-id="40e3f-103">List calendarGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40e3f-104">Получение групп календарей пользователя.</span><span class="sxs-lookup"><span data-stu-id="40e3f-104">Get the user's calendar groups.</span></span>
## <a name="permissions"></a><span data-ttu-id="40e3f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40e3f-105">Permissions</span></span>
<span data-ttu-id="40e3f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40e3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40e3f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40e3f-108">Permission type</span></span>      | <span data-ttu-id="40e3f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40e3f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40e3f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40e3f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="40e3f-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40e3f-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="40e3f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40e3f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40e3f-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40e3f-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="40e3f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40e3f-114">Application</span></span> | <span data-ttu-id="40e3f-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40e3f-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="40e3f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40e3f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups
GET /users/{id | userPrincipalName}/calendarGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="40e3f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="40e3f-117">Optional query parameters</span></span>
<span data-ttu-id="40e3f-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="40e3f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="40e3f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40e3f-119">Request headers</span></span>
| <span data-ttu-id="40e3f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40e3f-120">Header</span></span>       | <span data-ttu-id="40e3f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="40e3f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="40e3f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40e3f-122">Authorization</span></span>  | <span data-ttu-id="40e3f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40e3f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="40e3f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40e3f-125">Content-Type</span></span>  | <span data-ttu-id="40e3f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40e3f-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="40e3f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="40e3f-127">Request body</span></span>
<span data-ttu-id="40e3f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40e3f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40e3f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="40e3f-129">Response</span></span>

<span data-ttu-id="40e3f-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [CalendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40e3f-130">If successful, this method returns a `200 OK` response code and collection of [CalendarGroup](../resources/calendargroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="40e3f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="40e3f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40e3f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="40e3f-132">Request</span></span>
<span data-ttu-id="40e3f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40e3f-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="40e3f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="40e3f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendargroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendarGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="40e3f-135">C#</span><span class="sxs-lookup"><span data-stu-id="40e3f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendargroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="40e3f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40e3f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendargroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="40e3f-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="40e3f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendargroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="40e3f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="40e3f-138">Response</span></span>
<span data-ttu-id="40e3f-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40e3f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
