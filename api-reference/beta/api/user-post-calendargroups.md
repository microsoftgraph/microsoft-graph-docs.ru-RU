---
title: Создание объекта CalendarGroup
description: С помощью этого API можно создать экземпляр CalendarGroup.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bb38aba361c525268d10f2c3ccfc5408557ac19f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457669"
---
# <a name="create-calendargroup"></a><span data-ttu-id="800fa-103">Создание объекта CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="800fa-103">Create CalendarGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="800fa-104">С помощью этого API можно создать экземпляр CalendarGroup.</span><span class="sxs-lookup"><span data-stu-id="800fa-104">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="800fa-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="800fa-105">Permissions</span></span>
<span data-ttu-id="800fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="800fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="800fa-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="800fa-108">Permission type</span></span>      | <span data-ttu-id="800fa-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="800fa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="800fa-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="800fa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="800fa-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="800fa-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="800fa-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="800fa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="800fa-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="800fa-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="800fa-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="800fa-114">Application</span></span> | <span data-ttu-id="800fa-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="800fa-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="800fa-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="800fa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendarGroups
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="800fa-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="800fa-117">Request headers</span></span>
| <span data-ttu-id="800fa-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="800fa-118">Header</span></span>       | <span data-ttu-id="800fa-119">Значение</span><span class="sxs-lookup"><span data-stu-id="800fa-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="800fa-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="800fa-120">Authorization</span></span>  | <span data-ttu-id="800fa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="800fa-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="800fa-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="800fa-123">Content-Type</span></span>  | <span data-ttu-id="800fa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="800fa-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="800fa-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="800fa-125">Request body</span></span>
<span data-ttu-id="800fa-126">Предоставьте в тексте запроса описание объекта [CalendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="800fa-126">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="800fa-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="800fa-127">Response</span></span>

<span data-ttu-id="800fa-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [CalendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="800fa-128">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="800fa-129">Пример</span><span class="sxs-lookup"><span data-stu-id="800fa-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="800fa-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="800fa-130">Request</span></span>
<span data-ttu-id="800fa-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="800fa-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="800fa-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="800fa-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="800fa-133">C#</span><span class="sxs-lookup"><span data-stu-id="800fa-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendargroup-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="800fa-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="800fa-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendargroup-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="800fa-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="800fa-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendargroup-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="800fa-136">Предоставьте в тексте запроса описание объекта [calendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="800fa-136">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="800fa-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="800fa-137">Response</span></span>
<span data-ttu-id="800fa-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="800fa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
