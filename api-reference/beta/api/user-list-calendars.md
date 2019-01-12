---
title: Список календарей
description: 'Получение всех календарей пользователя (свойство навигации `/calendars`), календарей из группы календарей по умолчанию или из указанной группы календарей. '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e34c6acbcab5e5da4852d547038be6891806b4d4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983523"
---
# <a name="list-calendars"></a><span data-ttu-id="a942c-103">Список календарей</span><span class="sxs-lookup"><span data-stu-id="a942c-103">List calendars</span></span>

> <span data-ttu-id="a942c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a942c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a942c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a942c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a942c-106">Получение всех календарей пользователя (свойство навигации `/calendars`), календарей из группы календарей по умолчанию или из указанной группы календарей.</span><span class="sxs-lookup"><span data-stu-id="a942c-106">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="a942c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a942c-107">Permissions</span></span>
<span data-ttu-id="a942c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a942c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a942c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a942c-110">Permission type</span></span>      | <span data-ttu-id="a942c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a942c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a942c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a942c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a942c-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a942c-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a942c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a942c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a942c-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a942c-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a942c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a942c-116">Application</span></span> | <span data-ttu-id="a942c-117">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a942c-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a942c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a942c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="a942c-119">Все календари пользователя.</span><span class="sxs-lookup"><span data-stu-id="a942c-119">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="a942c-120">Календари пользователя в объекте [calendarGroup](../resources/calendargroup.md) по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a942c-120">The user's calendars in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendargroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="a942c-121">Календари пользователя в указанном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="a942c-121">The user's calendars in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a942c-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a942c-122">Optional query parameters</span></span>
<span data-ttu-id="a942c-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a942c-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a942c-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a942c-124">Request headers</span></span>
| <span data-ttu-id="a942c-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a942c-125">Header</span></span>       | <span data-ttu-id="a942c-126">Значение</span><span class="sxs-lookup"><span data-stu-id="a942c-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a942c-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a942c-127">Authorization</span></span>  | <span data-ttu-id="a942c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a942c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a942c-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a942c-130">Content-Type</span></span>   | <span data-ttu-id="a942c-131">application/json</span><span class="sxs-lookup"><span data-stu-id="a942c-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a942c-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a942c-132">Request body</span></span>
<span data-ttu-id="a942c-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a942c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a942c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a942c-134">Response</span></span>

<span data-ttu-id="a942c-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a942c-135">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a942c-136">Пример</span><span class="sxs-lookup"><span data-stu-id="a942c-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a942c-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="a942c-137">Request</span></span>
<span data-ttu-id="a942c-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a942c-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendars
```
##### <a name="response"></a><span data-ttu-id="a942c-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="a942c-139">Response</span></span>
<span data-ttu-id="a942c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a942c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
