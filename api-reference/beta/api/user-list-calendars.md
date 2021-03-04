---
title: Список календарей
description: 'Получение всех календарей пользователя (свойство навигации `/calendars`), календарей из группы календарей по умолчанию или из указанной группы календарей. '
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fed35d14abc6295c900aff50b0db8da74f1a5ec7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433553"
---
# <a name="list-calendars"></a><span data-ttu-id="b6037-103">Список календарей</span><span class="sxs-lookup"><span data-stu-id="b6037-103">List calendars</span></span>

<span data-ttu-id="b6037-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6037-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6037-105">Получение всех календарей пользователя (свойство навигации `/calendars`), календарей из группы календарей по умолчанию или из указанной группы календарей.</span><span class="sxs-lookup"><span data-stu-id="b6037-105">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="b6037-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6037-106">Permissions</span></span>
<span data-ttu-id="b6037-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6037-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6037-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6037-109">Permission type</span></span>      | <span data-ttu-id="b6037-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6037-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6037-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6037-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b6037-112">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6037-112">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b6037-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6037-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6037-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6037-114">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b6037-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6037-115">Application</span></span> | <span data-ttu-id="b6037-116">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6037-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6037-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6037-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="b6037-118">Все календари пользователя.</span><span class="sxs-lookup"><span data-stu-id="b6037-118">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="b6037-119">Календари пользователя в объекте [calendarGroup](../resources/calendargroup.md) по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b6037-119">The user's calendars in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="b6037-120">Календари пользователя в указанном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="b6037-120">The user's calendars in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6037-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b6037-121">Optional query parameters</span></span>
<span data-ttu-id="b6037-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b6037-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b6037-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6037-123">Request headers</span></span>
| <span data-ttu-id="b6037-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6037-124">Header</span></span>       | <span data-ttu-id="b6037-125">Значение</span><span class="sxs-lookup"><span data-stu-id="b6037-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b6037-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6037-126">Authorization</span></span>  | <span data-ttu-id="b6037-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6037-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b6037-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b6037-129">Content-Type</span></span>   | <span data-ttu-id="b6037-130">application/json</span><span class="sxs-lookup"><span data-stu-id="b6037-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6037-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b6037-131">Request body</span></span>
<span data-ttu-id="b6037-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b6037-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6037-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6037-133">Response</span></span>

<span data-ttu-id="b6037-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b6037-134">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b6037-135">Пример</span><span class="sxs-lookup"><span data-stu-id="b6037-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6037-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6037-136">Request</span></span>
<span data-ttu-id="b6037-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6037-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b6037-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6037-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_calendars"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendars
```
# <a name="c"></a>[<span data-ttu-id="b6037-139">C#</span><span class="sxs-lookup"><span data-stu-id="b6037-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6037-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6037-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6037-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6037-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6037-142">Java</span><span class="sxs-lookup"><span data-stu-id="b6037-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-calendars-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b6037-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6037-143">Response</span></span>
<span data-ttu-id="b6037-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b6037-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
            "calendarGroupId":null,
            "isDefaultCalendar": true,
            "canShare":true,
            "canViewPrivateItems":true,
            "hexColor": "",
            "isShared":false,
            "isSharedWithMe":false,
            "canEdit":true,
            "allowedOnlineMeetingProviders": [
                "teamsForBusiness"
            ],
            "defaultOnlineMeetingProvider": "teamsForBusiness",
            "isTallyingResponses": true,
            "isRemovable": false,
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
