---
title: Создание объекта CalendarGroup
description: С помощью этого API можно создать экземпляр CalendarGroup.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c310cf484bc3dd5908dd23f5a262881a31dc098d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054303"
---
# <a name="create-calendargroup"></a><span data-ttu-id="75893-103">Создание объекта CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="75893-103">Create CalendarGroup</span></span>

<span data-ttu-id="75893-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75893-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75893-105">С помощью этого API можно создать экземпляр CalendarGroup.</span><span class="sxs-lookup"><span data-stu-id="75893-105">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="75893-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75893-106">Permissions</span></span>
<span data-ttu-id="75893-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75893-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75893-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75893-109">Permission type</span></span>      | <span data-ttu-id="75893-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75893-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75893-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75893-111">Delegated (work or school account)</span></span> | <span data-ttu-id="75893-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75893-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="75893-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75893-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75893-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75893-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="75893-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75893-115">Application</span></span> | <span data-ttu-id="75893-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75893-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="75893-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75893-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendarGroups
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="75893-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75893-118">Request headers</span></span>
| <span data-ttu-id="75893-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75893-119">Header</span></span>       | <span data-ttu-id="75893-120">Значение</span><span class="sxs-lookup"><span data-stu-id="75893-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="75893-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75893-121">Authorization</span></span>  | <span data-ttu-id="75893-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75893-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="75893-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="75893-124">Content-Type</span></span>  | <span data-ttu-id="75893-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75893-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="75893-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75893-126">Request body</span></span>
<span data-ttu-id="75893-127">Предоставьте в тексте запроса описание объекта [CalendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75893-127">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="75893-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="75893-128">Response</span></span>

<span data-ttu-id="75893-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [CalendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75893-129">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75893-130">Пример</span><span class="sxs-lookup"><span data-stu-id="75893-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="75893-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="75893-131">Request</span></span>
<span data-ttu-id="75893-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75893-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="75893-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="75893-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups
Content-type: application/json

{
  "name": "Personal events"
}
```
# <a name="c"></a>[<span data-ttu-id="75893-134">C#</span><span class="sxs-lookup"><span data-stu-id="75893-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendargroup-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75893-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75893-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendargroup-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75893-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75893-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendargroup-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75893-137">Java</span><span class="sxs-lookup"><span data-stu-id="75893-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-calendargroup-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="75893-138">Предоставьте в тексте запроса описание объекта [calendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75893-138">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="75893-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="75893-139">Response</span></span>
<span data-ttu-id="75893-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="75893-140">Here is an example of the response.</span></span> <span data-ttu-id="75893-141">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="75893-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('7d54cb02-aaa3-4016-9f9c-a4b49422dd9b')/calendarGroups/$entity",
    "id": "AAMkADIxYjJiYmIzLTFmNjYtNGNhMy0YOkcEEh3vhfAAAGgdFjAAA=",
    "name": "Personal events",
    "classId": "44288f7d-7710-4293-8c8e-36f310ed2e6a",
    "changeKey": "NreqLYgxdE2DpHBBId74XwAABn6y8Q=="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

