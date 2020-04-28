---
title: Получение объекта calendarGroup
description: Получение свойств и связей, принадлежащих объекту группы календарей.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 666271f692f33299ceba5a8f9d83d66aeaba0fd1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388714"
---
# <a name="get-calendargroup"></a><span data-ttu-id="e6027-103">Получение объекта calendarGroup</span><span class="sxs-lookup"><span data-stu-id="e6027-103">Get calendarGroup</span></span>

<span data-ttu-id="e6027-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6027-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6027-105">Получение свойств и связей, принадлежащих объекту группы календарей.</span><span class="sxs-lookup"><span data-stu-id="e6027-105">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6027-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6027-106">Permissions</span></span>

<span data-ttu-id="e6027-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6027-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e6027-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6027-109">Permission type</span></span>                        | <span data-ttu-id="e6027-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6027-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e6027-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6027-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6027-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e6027-112">Calendars.Read</span></span>                              |
| <span data-ttu-id="e6027-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6027-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6027-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e6027-114">Calendars.Read</span></span>                              |
| <span data-ttu-id="e6027-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6027-115">Application</span></span>                            | <span data-ttu-id="e6027-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e6027-116">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="e6027-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6027-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="e6027-118">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="e6027-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e6027-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e6027-119">Optional query parameters</span></span>

<span data-ttu-id="e6027-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e6027-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6027-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6027-121">Request headers</span></span>

| <span data-ttu-id="e6027-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e6027-122">Name</span></span>          | <span data-ttu-id="e6027-123">Тип</span><span class="sxs-lookup"><span data-stu-id="e6027-123">Type</span></span>   | <span data-ttu-id="e6027-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e6027-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="e6027-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6027-125">Authorization</span></span> | <span data-ttu-id="e6027-126">string</span><span class="sxs-lookup"><span data-stu-id="e6027-126">string</span></span> | <span data-ttu-id="e6027-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6027-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6027-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e6027-129">Request body</span></span>

<span data-ttu-id="e6027-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e6027-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6027-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6027-131">Response</span></span>

<span data-ttu-id="e6027-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [calendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e6027-132">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6027-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e6027-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e6027-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6027-134">Request</span></span>

<span data-ttu-id="e6027-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6027-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e6027-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6027-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="e6027-137">C#</span><span class="sxs-lookup"><span data-stu-id="e6027-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6027-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6027-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6027-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6027-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e6027-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6027-140">Response</span></span>

<span data-ttu-id="e6027-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6027-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
