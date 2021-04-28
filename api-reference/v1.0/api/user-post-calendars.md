---
title: Создание объекта Calendar
description: С помощью этого API можно создать календарь для пользователя.
author: harini84
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2b19e7fdfb56518d26ba0dafd597838047ea21ae
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52031510"
---
# <a name="create-calendar"></a><span data-ttu-id="3cf8c-103">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="3cf8c-103">Create Calendar</span></span>

<span data-ttu-id="3cf8c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cf8c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3cf8c-105">С помощью этого API можно создать календарь для экземпляра [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="3cf8c-105">Use this API to create a new calendar for a [user](../resources/user.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3cf8c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3cf8c-106">Permissions</span></span>
<span data-ttu-id="3cf8c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cf8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cf8c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3cf8c-109">Permission type</span></span>      | <span data-ttu-id="3cf8c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3cf8c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cf8c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3cf8c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3cf8c-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3cf8c-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="3cf8c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3cf8c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cf8c-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3cf8c-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="3cf8c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3cf8c-115">Application</span></span> | <span data-ttu-id="3cf8c-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3cf8c-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cf8c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cf8c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="3cf8c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3cf8c-118">Request headers</span></span>
| <span data-ttu-id="3cf8c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3cf8c-119">Header</span></span>       | <span data-ttu-id="3cf8c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3cf8c-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3cf8c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3cf8c-121">Authorization</span></span>  | <span data-ttu-id="3cf8c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3cf8c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3cf8c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3cf8c-124">Content-Type</span></span>  | <span data-ttu-id="3cf8c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3cf8c-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3cf8c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3cf8c-126">Request body</span></span>
<span data-ttu-id="3cf8c-127">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3cf8c-127">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3cf8c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cf8c-128">Response</span></span>

<span data-ttu-id="3cf8c-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3cf8c-129">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cf8c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3cf8c-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="3cf8c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3cf8c-131">Request</span></span>
<span data-ttu-id="3cf8c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3cf8c-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3cf8c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cf8c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars
Content-type: application/json

{
  "name": "Volunteer"
}
```
# <a name="c"></a>[<span data-ttu-id="3cf8c-134">C#</span><span class="sxs-lookup"><span data-stu-id="3cf8c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendar-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cf8c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cf8c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendar-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cf8c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cf8c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendar-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cf8c-137">Java</span><span class="sxs-lookup"><span data-stu-id="3cf8c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-calendar-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="3cf8c-138">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3cf8c-138">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="3cf8c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cf8c-139">Response</span></span>
<span data-ttu-id="3cf8c-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3cf8c-140">Here is an example of the response.</span></span> <span data-ttu-id="3cf8c-141">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3cf8c-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Volunteer",
    "color":"auto",
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
    "canShare":true,
    "canViewPrivateItems":true,
    "hexColor": "",
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

