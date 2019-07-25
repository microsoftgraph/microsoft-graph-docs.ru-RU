---
title: Список календарей
description: 'Получение всех календарей пользователя (свойство навигации `/calendars`), календарей из группы календарей по умолчанию или из указанной группы календарей. '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d4ea121577225f5176b59c4121fed90d829592ce
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880770"
---
# <a name="list-calendars"></a><span data-ttu-id="d56fd-103">Список календарей</span><span class="sxs-lookup"><span data-stu-id="d56fd-103">List calendars</span></span>

<span data-ttu-id="d56fd-104">Получение всех календарей пользователя (свойство навигации `/calendars`), календарей из группы календарей по умолчанию или из указанной группы календарей.</span><span class="sxs-lookup"><span data-stu-id="d56fd-104">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="d56fd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d56fd-105">Permissions</span></span>
<span data-ttu-id="d56fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d56fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d56fd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d56fd-108">Permission type</span></span>      | <span data-ttu-id="d56fd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d56fd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d56fd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d56fd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d56fd-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d56fd-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d56fd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d56fd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d56fd-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d56fd-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d56fd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d56fd-114">Application</span></span> | <span data-ttu-id="d56fd-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d56fd-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d56fd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d56fd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="d56fd-117">Все календари пользователя.</span><span class="sxs-lookup"><span data-stu-id="d56fd-117">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="d56fd-118">Календари пользователя в объекте [calendarGroup](../resources/calendargroup.md) по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d56fd-118">The user's calendars in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendargroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="d56fd-119">Календари пользователя в указанном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="d56fd-119">The user's calendars in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d56fd-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d56fd-120">Optional query parameters</span></span>
<span data-ttu-id="d56fd-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d56fd-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d56fd-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d56fd-122">Request headers</span></span>
| <span data-ttu-id="d56fd-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d56fd-123">Header</span></span>       | <span data-ttu-id="d56fd-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d56fd-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d56fd-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d56fd-125">Authorization</span></span>  | <span data-ttu-id="d56fd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d56fd-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d56fd-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d56fd-128">Content-Type</span></span>   | <span data-ttu-id="d56fd-129">application/json</span><span class="sxs-lookup"><span data-stu-id="d56fd-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d56fd-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d56fd-130">Request body</span></span>
<span data-ttu-id="d56fd-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d56fd-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d56fd-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d56fd-132">Response</span></span>

<span data-ttu-id="d56fd-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d56fd-133">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d56fd-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d56fd-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d56fd-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d56fd-135">Request</span></span>
<span data-ttu-id="d56fd-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d56fd-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d56fd-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d56fd-137">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_calendars"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendars
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d56fd-138">C#</span><span class="sxs-lookup"><span data-stu-id="d56fd-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d56fd-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d56fd-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d56fd-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d56fd-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d56fd-141">Java</span><span class="sxs-lookup"><span data-stu-id="d56fd-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-calendars-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d56fd-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d56fd-142">Response</span></span>
<span data-ttu-id="d56fd-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d56fd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#me/calendars",
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
            "id": "AAMkAGI2TGuLAAA=",
            "name": "Calendar",
            "color": "auto",
            "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
            "canShare":true,
            "canViewPrivateItems":true,
            "canEdit":true,
            "owner":{
                "name":"Samantha Booth",
                "address":"samanthab@adatum.onmicrosoft.com"
            }
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
