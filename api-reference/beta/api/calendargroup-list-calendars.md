---
title: Список календарей
description: Получение списка календарей, входящих в группу.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d1dc7c556f304b15935f2c1ec14c16d035dfdf64
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047709"
---
# <a name="list-calendars"></a><span data-ttu-id="dea14-103">Список календарей</span><span class="sxs-lookup"><span data-stu-id="dea14-103">List calendars</span></span>

<span data-ttu-id="dea14-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dea14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dea14-105">Получение списка календарей, входящих в группу.</span><span class="sxs-lookup"><span data-stu-id="dea14-105">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="dea14-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dea14-106">Permissions</span></span>

<span data-ttu-id="dea14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dea14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dea14-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dea14-109">Permission type</span></span>                        | <span data-ttu-id="dea14-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dea14-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="dea14-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dea14-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dea14-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dea14-112">Calendars.Read</span></span>                              |
| <span data-ttu-id="dea14-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dea14-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dea14-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dea14-114">Calendars.Read</span></span>                              |
| <span data-ttu-id="dea14-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dea14-115">Application</span></span>                            | <span data-ttu-id="dea14-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dea14-116">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="dea14-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dea14-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="dea14-118">Объект [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="dea14-118">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="dea14-119">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="dea14-119">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dea14-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dea14-120">Optional query parameters</span></span>

<span data-ttu-id="dea14-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dea14-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dea14-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dea14-122">Request headers</span></span>

| <span data-ttu-id="dea14-123">Имя</span><span class="sxs-lookup"><span data-stu-id="dea14-123">Name</span></span>          | <span data-ttu-id="dea14-124">Тип</span><span class="sxs-lookup"><span data-stu-id="dea14-124">Type</span></span>   | <span data-ttu-id="dea14-125">Описание</span><span class="sxs-lookup"><span data-stu-id="dea14-125">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="dea14-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="dea14-126">Authorization</span></span> | <span data-ttu-id="dea14-127">string</span><span class="sxs-lookup"><span data-stu-id="dea14-127">string</span></span> | <span data-ttu-id="dea14-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dea14-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dea14-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dea14-130">Request body</span></span>

<span data-ttu-id="dea14-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dea14-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dea14-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="dea14-132">Response</span></span>

<span data-ttu-id="dea14-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dea14-133">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dea14-134">Пример</span><span class="sxs-lookup"><span data-stu-id="dea14-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dea14-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="dea14-135">Request</span></span>

<span data-ttu-id="dea14-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dea14-136">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dea14-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="dea14-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendargroup_get_calendars"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```
# <a name="c"></a>[<span data-ttu-id="dea14-138">C#</span><span class="sxs-lookup"><span data-stu-id="dea14-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendargroup-get-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dea14-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dea14-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendargroup-get-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dea14-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dea14-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendargroup-get-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dea14-141">Java</span><span class="sxs-lookup"><span data-stu-id="dea14-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendargroup-get-calendars-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dea14-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="dea14-142">Response</span></span>

<span data-ttu-id="dea14-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dea14-143">Here is an example of the response.</span></span> <span data-ttu-id="dea14-144">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dea14-144">Note: The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 147

{
  "value": [
    {
      "name": "name-value",
      "color": {
      },
      "calendarGroupId":"calendarGroupId-value",
      "changeKey": "changeKey-value",
      "id": "id-value"      
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
