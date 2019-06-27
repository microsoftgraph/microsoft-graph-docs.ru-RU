---
title: Получение объекта calendarGroup
description: Получение свойств и связей, принадлежащих объекту группы календарей.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 28244675e105be3cc1c4c6506b49a2ef3c6bb2df
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264717"
---
# <a name="get-calendargroup"></a><span data-ttu-id="447c7-103">Получение объекта calendarGroup</span><span class="sxs-lookup"><span data-stu-id="447c7-103">Get calendarGroup</span></span>

<span data-ttu-id="447c7-104">Получение свойств и связей, принадлежащих объекту группы календарей.</span><span class="sxs-lookup"><span data-stu-id="447c7-104">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="447c7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="447c7-105">Permissions</span></span>

<span data-ttu-id="447c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="447c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="447c7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="447c7-108">Permission type</span></span>                        | <span data-ttu-id="447c7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="447c7-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="447c7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="447c7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="447c7-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="447c7-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="447c7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="447c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="447c7-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="447c7-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="447c7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="447c7-114">Application</span></span>                            | <span data-ttu-id="447c7-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="447c7-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="447c7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="447c7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="447c7-117">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="447c7-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="447c7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="447c7-118">Optional query parameters</span></span>

<span data-ttu-id="447c7-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="447c7-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="447c7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="447c7-120">Request headers</span></span>

| <span data-ttu-id="447c7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="447c7-121">Name</span></span>          | <span data-ttu-id="447c7-122">Тип</span><span class="sxs-lookup"><span data-stu-id="447c7-122">Type</span></span>   | <span data-ttu-id="447c7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="447c7-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="447c7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="447c7-124">Authorization</span></span> | <span data-ttu-id="447c7-125">string</span><span class="sxs-lookup"><span data-stu-id="447c7-125">string</span></span> | <span data-ttu-id="447c7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="447c7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="447c7-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="447c7-128">Request body</span></span>

<span data-ttu-id="447c7-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="447c7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="447c7-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="447c7-130">Response</span></span>

<span data-ttu-id="447c7-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [calendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="447c7-131">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="447c7-132">Пример</span><span class="sxs-lookup"><span data-stu-id="447c7-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="447c7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="447c7-133">Request</span></span>

<span data-ttu-id="447c7-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="447c7-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="447c7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="447c7-135">Response</span></span>

<span data-ttu-id="447c7-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="447c7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="447c7-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="447c7-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="447c7-140">C#</span><span class="sxs-lookup"><span data-stu-id="447c7-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_calendargroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="447c7-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="447c7-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_calendargroup-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="447c7-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="447c7-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_calendargroup-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/calendargroup-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/calendargroup-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/calendargroup-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
