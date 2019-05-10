---
title: Список календарей
description: 'Получение всех календарей пользователя (свойство навигации `/calendars`), календарей из группы календарей по умолчанию или из указанной группы календарей. '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 02346c418a94baa63f2d24ad86dca80442a344cc
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33602058"
---
# <a name="list-calendars"></a><span data-ttu-id="24b96-103">Список календарей</span><span class="sxs-lookup"><span data-stu-id="24b96-103">List calendars</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24b96-104">Получение всех календарей пользователя (свойство навигации `/calendars`), календарей из группы календарей по умолчанию или из указанной группы календарей.</span><span class="sxs-lookup"><span data-stu-id="24b96-104">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="24b96-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24b96-105">Permissions</span></span>
<span data-ttu-id="24b96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24b96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24b96-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24b96-108">Permission type</span></span>      | <span data-ttu-id="24b96-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24b96-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24b96-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24b96-110">Delegated (work or school account)</span></span> | <span data-ttu-id="24b96-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24b96-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="24b96-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24b96-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24b96-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24b96-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="24b96-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24b96-114">Application</span></span> | <span data-ttu-id="24b96-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24b96-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="24b96-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24b96-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="24b96-117">Все календари пользователя.</span><span class="sxs-lookup"><span data-stu-id="24b96-117">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="24b96-118">Календари пользователя в объекте [calendarGroup](../resources/calendargroup.md) по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="24b96-118">The user's calendars in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendargroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="24b96-119">Календари пользователя в указанном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="24b96-119">The user's calendars in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24b96-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="24b96-120">Optional query parameters</span></span>
<span data-ttu-id="24b96-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="24b96-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="24b96-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24b96-122">Request headers</span></span>
| <span data-ttu-id="24b96-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24b96-123">Header</span></span>       | <span data-ttu-id="24b96-124">Значение</span><span class="sxs-lookup"><span data-stu-id="24b96-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="24b96-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24b96-125">Authorization</span></span>  | <span data-ttu-id="24b96-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24b96-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="24b96-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="24b96-128">Content-Type</span></span>   | <span data-ttu-id="24b96-129">application/json</span><span class="sxs-lookup"><span data-stu-id="24b96-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="24b96-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24b96-130">Request body</span></span>
<span data-ttu-id="24b96-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24b96-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24b96-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="24b96-132">Response</span></span>

<span data-ttu-id="24b96-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24b96-133">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="24b96-134">Пример</span><span class="sxs-lookup"><span data-stu-id="24b96-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24b96-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="24b96-135">Request</span></span>
<span data-ttu-id="24b96-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24b96-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendars
```
##### <a name="response"></a><span data-ttu-id="24b96-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="24b96-137">Response</span></span>
<span data-ttu-id="24b96-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24b96-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#me/calendars",
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
            "id": "AAMkAGI2TGuLAAA=",
            "name": "Calendar",
            "color": "auto",
            "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
            "isDefaultCalendar": true,
            "canShare":true,
            "canViewPrivateItems":true,
            "hexColor": "",
            "isShared":false,
            "isSharedWithMe":false,
            "canEdit":true,
            "owner":{
                "name":"Samantha Booth",
                "address":"samanthab@adatum.onmicrosoft.com"
            }
        }
    ]
}

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="24b96-141">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="24b96-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="24b96-142">C#</span><span class="sxs-lookup"><span data-stu-id="24b96-142">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_calendars-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24b96-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24b96-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_calendars-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/user-list-calendars.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-calendars.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
