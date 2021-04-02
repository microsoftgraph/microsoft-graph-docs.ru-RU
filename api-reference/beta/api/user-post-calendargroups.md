---
title: Создание объекта CalendarGroup
description: С помощью этого API можно создать экземпляр CalendarGroup.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 59535a9423d5ffe115d59cdcd396cd2cb9d2ad99
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507809"
---
# <a name="create-calendargroup"></a><span data-ttu-id="668ae-103">Создание объекта CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="668ae-103">Create CalendarGroup</span></span>

<span data-ttu-id="668ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="668ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="668ae-105">С помощью этого API можно создать экземпляр CalendarGroup.</span><span class="sxs-lookup"><span data-stu-id="668ae-105">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="668ae-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="668ae-106">Permissions</span></span>
<span data-ttu-id="668ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="668ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="668ae-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="668ae-109">Permission type</span></span>      | <span data-ttu-id="668ae-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="668ae-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="668ae-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="668ae-111">Delegated (work or school account)</span></span> | <span data-ttu-id="668ae-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="668ae-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="668ae-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="668ae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="668ae-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="668ae-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="668ae-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="668ae-115">Application</span></span> | <span data-ttu-id="668ae-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="668ae-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="668ae-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="668ae-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendarGroups
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="668ae-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="668ae-118">Request headers</span></span>
| <span data-ttu-id="668ae-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="668ae-119">Header</span></span>       | <span data-ttu-id="668ae-120">Значение</span><span class="sxs-lookup"><span data-stu-id="668ae-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="668ae-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="668ae-121">Authorization</span></span>  | <span data-ttu-id="668ae-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="668ae-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="668ae-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="668ae-124">Content-Type</span></span>  | <span data-ttu-id="668ae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="668ae-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="668ae-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="668ae-126">Request body</span></span>
<span data-ttu-id="668ae-127">Предоставьте в тексте запроса описание объекта [CalendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="668ae-127">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="668ae-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="668ae-128">Response</span></span>

<span data-ttu-id="668ae-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [CalendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="668ae-129">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="668ae-130">Пример</span><span class="sxs-lookup"><span data-stu-id="668ae-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="668ae-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="668ae-131">Request</span></span>
<span data-ttu-id="668ae-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="668ae-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="668ae-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="668ae-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendarGroups
Content-type: application/json

{
  "name": "Personal events"
}
```
# <a name="c"></a>[<span data-ttu-id="668ae-134">C#</span><span class="sxs-lookup"><span data-stu-id="668ae-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendargroup-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="668ae-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="668ae-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendargroup-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="668ae-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="668ae-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendargroup-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="668ae-137">Java</span><span class="sxs-lookup"><span data-stu-id="668ae-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-calendargroup-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="668ae-138">Предоставьте в тексте запроса описание объекта [calendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="668ae-138">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="668ae-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="668ae-139">Response</span></span>
<span data-ttu-id="668ae-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="668ae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('7d54cb02-aaa3-4016-9f9c-a4b49422dd9b')/calendarGroups/$entity",
    "id": "AAMkADIxYjJiYmIzLTFmNjYtNGNhMy0YOkcEEh3vhfAAAGgdFjAAA=",
    "name": "Personal events",
    "classId": "44288f7d-7710-4293-8c8e-36f310ed2e6a",
    "changeKey": "NreqLYgxdE2DpHBBId74XwAABn6y8Q=="
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


