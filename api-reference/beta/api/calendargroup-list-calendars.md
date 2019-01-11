---
title: Список календарей
description: Получение списка календарей из группы календарей.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 9ffa22a25fcc5c42ca9a61ea09a5cc68d2f3351b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814205"
---
# <a name="list-calendars"></a><span data-ttu-id="6982d-103">Список календарей</span><span class="sxs-lookup"><span data-stu-id="6982d-103">List calendars</span></span>

> <span data-ttu-id="6982d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6982d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6982d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6982d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6982d-106">Получение списка календарей из группы календарей.</span><span class="sxs-lookup"><span data-stu-id="6982d-106">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="6982d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6982d-107">Permissions</span></span>

<span data-ttu-id="6982d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6982d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6982d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6982d-110">Permission type</span></span>                        | <span data-ttu-id="6982d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6982d-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="6982d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6982d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6982d-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6982d-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="6982d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6982d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6982d-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6982d-115">Calendars.Read</span></span>                              |
| <span data-ttu-id="6982d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6982d-116">Application</span></span>                            | <span data-ttu-id="6982d-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6982d-117">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="6982d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6982d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="6982d-119">Объект [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6982d-119">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="6982d-120">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="6982d-120">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6982d-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6982d-121">Optional query parameters</span></span>

<span data-ttu-id="6982d-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6982d-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6982d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6982d-123">Request headers</span></span>

| <span data-ttu-id="6982d-124">Имя</span><span class="sxs-lookup"><span data-stu-id="6982d-124">Name</span></span>          | <span data-ttu-id="6982d-125">Тип</span><span class="sxs-lookup"><span data-stu-id="6982d-125">Type</span></span>   | <span data-ttu-id="6982d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="6982d-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="6982d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="6982d-127">Authorization</span></span> | <span data-ttu-id="6982d-128">string</span><span class="sxs-lookup"><span data-stu-id="6982d-128">string</span></span> | <span data-ttu-id="6982d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6982d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6982d-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6982d-131">Request body</span></span>

<span data-ttu-id="6982d-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6982d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6982d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6982d-133">Response</span></span>

<span data-ttu-id="6982d-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6982d-134">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6982d-135">Пример</span><span class="sxs-lookup"><span data-stu-id="6982d-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6982d-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="6982d-136">Request</span></span>

<span data-ttu-id="6982d-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6982d-137">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```

##### <a name="response"></a><span data-ttu-id="6982d-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="6982d-138">Response</span></span>

<span data-ttu-id="6982d-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6982d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
