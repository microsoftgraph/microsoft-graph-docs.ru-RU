---
title: Создание объекта Calendar
description: С помощью этого API можно создать календарь для пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 47e1511be02f44003b1793462e46d5ca49ebb134
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866979"
---
# <a name="create-calendar"></a><span data-ttu-id="5085e-103">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="5085e-103">Create Calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5085e-104">С помощью этого API можно создать календарь для экземпляра [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="5085e-104">Use this API to create a new calendar for a [user](../resources/user.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="5085e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5085e-105">Permissions</span></span>
<span data-ttu-id="5085e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5085e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5085e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5085e-108">Permission type</span></span>      | <span data-ttu-id="5085e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5085e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5085e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5085e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5085e-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5085e-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5085e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5085e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5085e-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5085e-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5085e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5085e-114">Application</span></span> | <span data-ttu-id="5085e-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5085e-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5085e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5085e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="5085e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5085e-117">Request headers</span></span>
| <span data-ttu-id="5085e-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5085e-118">Header</span></span>       | <span data-ttu-id="5085e-119">Значение</span><span class="sxs-lookup"><span data-stu-id="5085e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5085e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5085e-120">Authorization</span></span>  | <span data-ttu-id="5085e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5085e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5085e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5085e-123">Content-Type</span></span>  | <span data-ttu-id="5085e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5085e-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5085e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5085e-125">Request body</span></span>
<span data-ttu-id="5085e-126">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5085e-126">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5085e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="5085e-127">Response</span></span>

<span data-ttu-id="5085e-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5085e-128">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5085e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="5085e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5085e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="5085e-130">Request</span></span>
<span data-ttu-id="5085e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5085e-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5085e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5085e-132">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="5085e-133">C#</span><span class="sxs-lookup"><span data-stu-id="5085e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendar-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5085e-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="5085e-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendar-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5085e-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5085e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendar-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5085e-136">Java</span><span class="sxs-lookup"><span data-stu-id="5085e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-calendar-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="5085e-137">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5085e-137">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5085e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5085e-138">Response</span></span>
<span data-ttu-id="5085e-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5085e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
