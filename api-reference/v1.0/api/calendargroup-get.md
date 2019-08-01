---
title: Получение объекта calendarGroup
description: Получение свойств и связей, принадлежащих объекту группы календарей.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e0b958a82b9e63c72be91a5bdc61af73b43f7477
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003954"
---
# <a name="get-calendargroup"></a><span data-ttu-id="d2a6e-103">Получение объекта calendarGroup</span><span class="sxs-lookup"><span data-stu-id="d2a6e-103">Get calendarGroup</span></span>

<span data-ttu-id="d2a6e-104">Получение свойств и связей, принадлежащих объекту группы календарей.</span><span class="sxs-lookup"><span data-stu-id="d2a6e-104">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2a6e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2a6e-105">Permissions</span></span>

<span data-ttu-id="d2a6e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2a6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2a6e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2a6e-108">Permission type</span></span>                        | <span data-ttu-id="d2a6e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2a6e-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="d2a6e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2a6e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2a6e-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d2a6e-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="d2a6e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2a6e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2a6e-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d2a6e-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="d2a6e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2a6e-114">Application</span></span>                            | <span data-ttu-id="d2a6e-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d2a6e-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="d2a6e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2a6e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="d2a6e-117">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="d2a6e-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2a6e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d2a6e-118">Optional query parameters</span></span>

<span data-ttu-id="d2a6e-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d2a6e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2a6e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2a6e-120">Request headers</span></span>

| <span data-ttu-id="d2a6e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d2a6e-121">Name</span></span>          | <span data-ttu-id="d2a6e-122">Тип</span><span class="sxs-lookup"><span data-stu-id="d2a6e-122">Type</span></span>   | <span data-ttu-id="d2a6e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d2a6e-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="d2a6e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2a6e-124">Authorization</span></span> | <span data-ttu-id="d2a6e-125">string</span><span class="sxs-lookup"><span data-stu-id="d2a6e-125">string</span></span> | <span data-ttu-id="d2a6e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2a6e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2a6e-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d2a6e-128">Request body</span></span>

<span data-ttu-id="d2a6e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2a6e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2a6e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2a6e-130">Response</span></span>

<span data-ttu-id="d2a6e-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [calendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2a6e-131">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2a6e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d2a6e-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d2a6e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2a6e-133">Request</span></span>

<span data-ttu-id="d2a6e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2a6e-134">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d2a6e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2a6e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d2a6e-136">C#</span><span class="sxs-lookup"><span data-stu-id="d2a6e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d2a6e-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="d2a6e-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d2a6e-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d2a6e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d2a6e-139">Java</span><span class="sxs-lookup"><span data-stu-id="d2a6e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d2a6e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2a6e-140">Response</span></span>

<span data-ttu-id="d2a6e-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2a6e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
