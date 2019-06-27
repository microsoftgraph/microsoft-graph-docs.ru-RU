---
title: Создание объекта CalendarGroup
description: С помощью этого API можно создать экземпляр CalendarGroup.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 67c03ba7b7b48480d05ee28ae15c7000c8385cbc
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269540"
---
# <a name="create-calendargroup"></a><span data-ttu-id="937bc-103">Создание объекта CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="937bc-103">Create CalendarGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="937bc-104">С помощью этого API можно создать экземпляр CalendarGroup.</span><span class="sxs-lookup"><span data-stu-id="937bc-104">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="937bc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="937bc-105">Permissions</span></span>
<span data-ttu-id="937bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="937bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="937bc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="937bc-108">Permission type</span></span>      | <span data-ttu-id="937bc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="937bc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="937bc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="937bc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="937bc-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="937bc-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="937bc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="937bc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="937bc-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="937bc-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="937bc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="937bc-114">Application</span></span> | <span data-ttu-id="937bc-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="937bc-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="937bc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="937bc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendarGroups
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="937bc-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="937bc-117">Request headers</span></span>
| <span data-ttu-id="937bc-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="937bc-118">Header</span></span>       | <span data-ttu-id="937bc-119">Значение</span><span class="sxs-lookup"><span data-stu-id="937bc-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="937bc-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="937bc-120">Authorization</span></span>  | <span data-ttu-id="937bc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="937bc-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="937bc-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="937bc-123">Content-Type</span></span>  | <span data-ttu-id="937bc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="937bc-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="937bc-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="937bc-125">Request body</span></span>
<span data-ttu-id="937bc-126">Предоставьте в тексте запроса описание объекта [CalendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="937bc-126">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="937bc-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="937bc-127">Response</span></span>

<span data-ttu-id="937bc-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [CalendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="937bc-128">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="937bc-129">Пример</span><span class="sxs-lookup"><span data-stu-id="937bc-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="937bc-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="937bc-130">Request</span></span>
<span data-ttu-id="937bc-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="937bc-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="937bc-132">Предоставьте в тексте запроса описание объекта [calendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="937bc-132">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="937bc-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="937bc-133">Response</span></span>
<span data-ttu-id="937bc-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="937bc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="937bc-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="937bc-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="937bc-138">C#</span><span class="sxs-lookup"><span data-stu-id="937bc-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_calendargroup_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="937bc-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="937bc-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_calendargroup_from_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="937bc-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="937bc-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_calendargroup_from_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/user-post-calendargroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-post-calendargroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-calendargroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
