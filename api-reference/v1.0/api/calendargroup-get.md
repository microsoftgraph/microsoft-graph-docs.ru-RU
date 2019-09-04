---
title: Получение объекта calendarGroup
description: Получение свойств и связей, принадлежащих объекту группы календарей.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0e403c45bc955b49c500f6b347e12413d6a988bc
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726531"
---
# <a name="get-calendargroup"></a><span data-ttu-id="dbab6-103">Получение объекта calendarGroup</span><span class="sxs-lookup"><span data-stu-id="dbab6-103">Get calendarGroup</span></span>

<span data-ttu-id="dbab6-104">Получение свойств и связей, принадлежащих объекту группы календарей.</span><span class="sxs-lookup"><span data-stu-id="dbab6-104">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbab6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dbab6-105">Permissions</span></span>

<span data-ttu-id="dbab6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbab6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dbab6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbab6-108">Permission type</span></span>                        | <span data-ttu-id="dbab6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbab6-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="dbab6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbab6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dbab6-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dbab6-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="dbab6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbab6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbab6-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dbab6-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="dbab6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbab6-114">Application</span></span>                            | <span data-ttu-id="dbab6-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dbab6-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="dbab6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbab6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="dbab6-117">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="dbab6-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dbab6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dbab6-118">Optional query parameters</span></span>

<span data-ttu-id="dbab6-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dbab6-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dbab6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dbab6-120">Request headers</span></span>

| <span data-ttu-id="dbab6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="dbab6-121">Name</span></span>          | <span data-ttu-id="dbab6-122">Тип</span><span class="sxs-lookup"><span data-stu-id="dbab6-122">Type</span></span>   | <span data-ttu-id="dbab6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="dbab6-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="dbab6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbab6-124">Authorization</span></span> | <span data-ttu-id="dbab6-125">string</span><span class="sxs-lookup"><span data-stu-id="dbab6-125">string</span></span> | <span data-ttu-id="dbab6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dbab6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbab6-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dbab6-128">Request body</span></span>

<span data-ttu-id="dbab6-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dbab6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbab6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbab6-130">Response</span></span>

<span data-ttu-id="dbab6-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [calendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dbab6-131">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbab6-132">Пример</span><span class="sxs-lookup"><span data-stu-id="dbab6-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dbab6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbab6-133">Request</span></span>

<span data-ttu-id="dbab6-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dbab6-134">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dbab6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbab6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dbab6-136">C#</span><span class="sxs-lookup"><span data-stu-id="dbab6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dbab6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbab6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dbab6-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dbab6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dbab6-139">Java</span><span class="sxs-lookup"><span data-stu-id="dbab6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dbab6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbab6-140">Response</span></span>

<span data-ttu-id="dbab6-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dbab6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
