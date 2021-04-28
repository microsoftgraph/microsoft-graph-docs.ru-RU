---
title: Создание объекта Calendar
description: С помощью этого API можно для экземпляра user создать календарь в группе календарей.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d3e3904487bf82ecd552fd61a3217474de89d300
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054177"
---
# <a name="create-calendar"></a><span data-ttu-id="2ee12-103">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="2ee12-103">Create Calendar</span></span>

<span data-ttu-id="2ee12-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ee12-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2ee12-105">С помощью этого API можно для экземпляра [user](../resources/user.md) создать календарь в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="2ee12-105">Use this API to create a new calendar in a calendar group for a [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2ee12-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ee12-106">Permissions</span></span>

<span data-ttu-id="2ee12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ee12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ee12-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ee12-109">Permission type</span></span>                        | <span data-ttu-id="2ee12-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ee12-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="2ee12-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ee12-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ee12-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ee12-112">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="2ee12-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ee12-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ee12-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ee12-114">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="2ee12-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ee12-115">Application</span></span>                            | <span data-ttu-id="2ee12-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ee12-116">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2ee12-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ee12-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="2ee12-118">Объект [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="2ee12-118">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
POST /me/calendars
POST /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="2ee12-119">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="2ee12-119">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a><span data-ttu-id="2ee12-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ee12-120">Request headers</span></span>

| <span data-ttu-id="2ee12-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2ee12-121">Header</span></span>        | <span data-ttu-id="2ee12-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2ee12-122">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="2ee12-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ee12-123">Authorization</span></span> | <span data-ttu-id="2ee12-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ee12-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="2ee12-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ee12-126">Content-Type</span></span>  | <span data-ttu-id="2ee12-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ee12-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ee12-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ee12-129">Request body</span></span>

<span data-ttu-id="2ee12-130">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ee12-130">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2ee12-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ee12-131">Response</span></span>

<span data-ttu-id="2ee12-132">В случае успеха этот метод возвращает код отклика `201 Created` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ee12-132">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ee12-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2ee12-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2ee12-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ee12-134">Request</span></span>

<span data-ttu-id="2ee12-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ee12-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2ee12-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ee12-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADYAAAR9NR5AAA="],
  "name": "create_calendar_from_calendargroup"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/calendargroups/AAMkADYAAAR9NR5AAA=/calendars
Content-type: application/json

{
  "name": "Marketing calendar"
}
```
# <a name="javascript"></a>[<span data-ttu-id="2ee12-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ee12-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendar-from-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="2ee12-138">C#</span><span class="sxs-lookup"><span data-stu-id="2ee12-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendar-from-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ee12-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ee12-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendar-from-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ee12-140">Java</span><span class="sxs-lookup"><span data-stu-id="2ee12-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-calendar-from-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="2ee12-141">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ee12-141">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="2ee12-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ee12-142">Response</span></span>

<span data-ttu-id="2ee12-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2ee12-143">Here is an example of the response.</span></span> <span data-ttu-id="2ee12-144">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2ee12-144">Note: The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/calendarGroups('AAMkADYAAAR9NR5AAA%3D')/calendars/$entity",
    "id": "AAMkADYCQM0GfRAAAcrRD-AAA=",
    "name": "Marketing calendar",
    "color": "auto",
    "changeKey": "4xTfgHLeDkOqYVAkDNBn0QAAHKl46A==",
    "canShare": true,
    "canViewPrivateItems": true,
    "canEdit": true,
    "owner": {
        "name": "Adele Vance",
        "address": "adelev@contoso.OnMicrosoft.com"
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

