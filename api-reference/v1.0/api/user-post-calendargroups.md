---
title: Создание объекта CalendarGroup
description: С помощью этого API можно создать экземпляр CalendarGroup.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e925204ffece948da1fe73851353ef8669d372b1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509012"
---
# <a name="create-calendargroup"></a><span data-ttu-id="77174-103">Создание объекта CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="77174-103">Create CalendarGroup</span></span>

<span data-ttu-id="77174-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77174-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="77174-105">С помощью этого API можно создать экземпляр CalendarGroup.</span><span class="sxs-lookup"><span data-stu-id="77174-105">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="77174-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77174-106">Permissions</span></span>
<span data-ttu-id="77174-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77174-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77174-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77174-109">Permission type</span></span>      | <span data-ttu-id="77174-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77174-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77174-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77174-111">Delegated (work or school account)</span></span> | <span data-ttu-id="77174-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77174-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="77174-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77174-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77174-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77174-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="77174-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77174-115">Application</span></span> | <span data-ttu-id="77174-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77174-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="77174-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77174-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendarGroups
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="77174-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77174-118">Request headers</span></span>
| <span data-ttu-id="77174-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77174-119">Header</span></span>       | <span data-ttu-id="77174-120">Значение</span><span class="sxs-lookup"><span data-stu-id="77174-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="77174-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77174-121">Authorization</span></span>  | <span data-ttu-id="77174-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77174-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="77174-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="77174-124">Content-Type</span></span>  | <span data-ttu-id="77174-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77174-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="77174-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77174-126">Request body</span></span>
<span data-ttu-id="77174-127">Предоставьте в тексте запроса описание объекта [CalendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77174-127">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="77174-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="77174-128">Response</span></span>

<span data-ttu-id="77174-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [CalendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="77174-129">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77174-130">Пример</span><span class="sxs-lookup"><span data-stu-id="77174-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77174-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="77174-131">Request</span></span>
<span data-ttu-id="77174-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77174-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="77174-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="77174-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
# <a name="c"></a>[<span data-ttu-id="77174-134">C#</span><span class="sxs-lookup"><span data-stu-id="77174-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendargroup-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77174-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77174-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendargroup-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77174-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77174-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendargroup-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77174-137">Java</span><span class="sxs-lookup"><span data-stu-id="77174-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-calendargroup-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="77174-138">Предоставьте в тексте запроса описание объекта [calendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77174-138">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="77174-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="77174-139">Response</span></span>
<span data-ttu-id="77174-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77174-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
