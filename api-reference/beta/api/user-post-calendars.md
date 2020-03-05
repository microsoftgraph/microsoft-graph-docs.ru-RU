---
title: Создание объекта Calendar
description: С помощью этого API можно создать календарь для пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 07bf9d9069a89cef3bbf74526fc954a987d12f2c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451734"
---
# <a name="create-calendar"></a><span data-ttu-id="16cbb-103">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="16cbb-103">Create Calendar</span></span>

<span data-ttu-id="16cbb-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="16cbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16cbb-105">С помощью этого API можно создать календарь для экземпляра [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="16cbb-105">Use this API to create a new calendar for a [user](../resources/user.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="16cbb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16cbb-106">Permissions</span></span>
<span data-ttu-id="16cbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16cbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16cbb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16cbb-109">Permission type</span></span>      | <span data-ttu-id="16cbb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16cbb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16cbb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16cbb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="16cbb-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16cbb-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="16cbb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16cbb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16cbb-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16cbb-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="16cbb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16cbb-115">Application</span></span> | <span data-ttu-id="16cbb-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16cbb-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="16cbb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16cbb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="16cbb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16cbb-118">Request headers</span></span>
| <span data-ttu-id="16cbb-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16cbb-119">Header</span></span>       | <span data-ttu-id="16cbb-120">Значение</span><span class="sxs-lookup"><span data-stu-id="16cbb-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="16cbb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16cbb-121">Authorization</span></span>  | <span data-ttu-id="16cbb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16cbb-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="16cbb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="16cbb-124">Content-Type</span></span>  | <span data-ttu-id="16cbb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="16cbb-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="16cbb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16cbb-126">Request body</span></span>
<span data-ttu-id="16cbb-127">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16cbb-127">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="16cbb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="16cbb-128">Response</span></span>

<span data-ttu-id="16cbb-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16cbb-129">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16cbb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="16cbb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="16cbb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="16cbb-131">Request</span></span>
<span data-ttu-id="16cbb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16cbb-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="16cbb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="16cbb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendars
Content-type: application/json

{
  "name": "Volunteer"
}

```
# <a name="c"></a>[<span data-ttu-id="16cbb-134">C#</span><span class="sxs-lookup"><span data-stu-id="16cbb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendar-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16cbb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16cbb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendar-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16cbb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16cbb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendar-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="16cbb-137">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16cbb-137">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="16cbb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="16cbb-138">Response</span></span>
<span data-ttu-id="16cbb-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16cbb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Volunteer",
    "color":"auto",
    "isDefaultCalendar":false,
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
