---
title: Список календарей
description: Получение списка календарей из группы календарей.
author: angelgolfer-ms
ms.openlocfilehash: e150d25976cda8cde52a70669fb38333f2a95fd2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341386"
---
# <a name="list-calendars"></a><span data-ttu-id="c83e0-103">Список календарей</span><span class="sxs-lookup"><span data-stu-id="c83e0-103">List calendars</span></span>

<span data-ttu-id="c83e0-104">Получение списка календарей из группы календарей.</span><span class="sxs-lookup"><span data-stu-id="c83e0-104">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="c83e0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c83e0-105">Permissions</span></span>

<span data-ttu-id="c83e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c83e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c83e0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c83e0-108">Permission type</span></span>                        | <span data-ttu-id="c83e0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c83e0-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c83e0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c83e0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c83e0-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c83e0-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="c83e0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c83e0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c83e0-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c83e0-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="c83e0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c83e0-114">Application</span></span>                            | <span data-ttu-id="c83e0-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c83e0-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="c83e0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c83e0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="c83e0-117">Объект [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="c83e0-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="c83e0-118">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="c83e0-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c83e0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c83e0-119">Optional query parameters</span></span>

<span data-ttu-id="c83e0-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c83e0-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c83e0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c83e0-121">Request headers</span></span>

| <span data-ttu-id="c83e0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c83e0-122">Name</span></span>          | <span data-ttu-id="c83e0-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c83e0-123">Type</span></span>   | <span data-ttu-id="c83e0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c83e0-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="c83e0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c83e0-125">Authorization</span></span> | <span data-ttu-id="c83e0-126">string</span><span class="sxs-lookup"><span data-stu-id="c83e0-126">string</span></span> | <span data-ttu-id="c83e0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c83e0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c83e0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c83e0-129">Request body</span></span>

<span data-ttu-id="c83e0-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c83e0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c83e0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c83e0-131">Response</span></span>

<span data-ttu-id="c83e0-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c83e0-132">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c83e0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c83e0-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c83e0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c83e0-134">Request</span></span>

<span data-ttu-id="c83e0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c83e0-135">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
```

##### <a name="response"></a><span data-ttu-id="c83e0-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="c83e0-136">Response</span></span>

<span data-ttu-id="c83e0-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c83e0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
      "changeKey": "changeKey-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
