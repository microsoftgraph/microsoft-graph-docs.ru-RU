---
title: Создание объекта CalendarGroup
description: С помощью этого API можно создать экземпляр CalendarGroup.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ddf26be745f22ca9ef98fb4949005b17d332e2cc
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107488"
---
# <a name="create-calendargroup"></a><span data-ttu-id="482e5-103">Создание объекта CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="482e5-103">Create CalendarGroup</span></span>

<span data-ttu-id="482e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="482e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="482e5-105">С помощью этого API можно создать экземпляр CalendarGroup.</span><span class="sxs-lookup"><span data-stu-id="482e5-105">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="482e5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="482e5-106">Permissions</span></span>
<span data-ttu-id="482e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="482e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="482e5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="482e5-109">Permission type</span></span>      | <span data-ttu-id="482e5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="482e5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="482e5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="482e5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="482e5-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="482e5-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="482e5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="482e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="482e5-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="482e5-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="482e5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="482e5-115">Application</span></span> | <span data-ttu-id="482e5-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="482e5-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="482e5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="482e5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendarGroups
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="482e5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="482e5-118">Request headers</span></span>
| <span data-ttu-id="482e5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="482e5-119">Header</span></span>       | <span data-ttu-id="482e5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="482e5-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="482e5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="482e5-121">Authorization</span></span>  | <span data-ttu-id="482e5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="482e5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="482e5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="482e5-124">Content-Type</span></span>  | <span data-ttu-id="482e5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="482e5-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="482e5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="482e5-126">Request body</span></span>
<span data-ttu-id="482e5-127">Предоставьте в тексте запроса описание объекта [CalendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="482e5-127">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="482e5-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="482e5-128">Response</span></span>

<span data-ttu-id="482e5-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [CalendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="482e5-129">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="482e5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="482e5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="482e5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="482e5-131">Request</span></span>
<span data-ttu-id="482e5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="482e5-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="482e5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="482e5-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="482e5-134">C#</span><span class="sxs-lookup"><span data-stu-id="482e5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendargroup-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="482e5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="482e5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendargroup-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="482e5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="482e5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendargroup-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="482e5-137">Предоставьте в тексте запроса описание объекта [calendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="482e5-137">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="482e5-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="482e5-138">Response</span></span>
<span data-ttu-id="482e5-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="482e5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
