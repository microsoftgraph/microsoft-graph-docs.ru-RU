---
title: Список календарей
description: Получение списка календарей, входящих в группу.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d8d54b1dd3f8a1f75a3f4e4ab3449cb4fc8a8283
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322399"
---
# <a name="list-calendars"></a><span data-ttu-id="2b294-103">Список календарей</span><span class="sxs-lookup"><span data-stu-id="2b294-103">List calendars</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b294-104">Получение списка календарей, входящих в группу.</span><span class="sxs-lookup"><span data-stu-id="2b294-104">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b294-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b294-105">Permissions</span></span>

<span data-ttu-id="2b294-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b294-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2b294-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b294-108">Permission type</span></span>                        | <span data-ttu-id="2b294-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b294-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="2b294-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b294-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2b294-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2b294-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="2b294-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b294-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b294-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2b294-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="2b294-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b294-114">Application</span></span>                            | <span data-ttu-id="2b294-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2b294-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="2b294-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b294-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="2b294-117">Объект [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="2b294-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="2b294-118">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="2b294-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b294-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2b294-119">Optional query parameters</span></span>

<span data-ttu-id="2b294-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2b294-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b294-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b294-121">Request headers</span></span>

| <span data-ttu-id="2b294-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2b294-122">Name</span></span>          | <span data-ttu-id="2b294-123">Тип</span><span class="sxs-lookup"><span data-stu-id="2b294-123">Type</span></span>   | <span data-ttu-id="2b294-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2b294-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="2b294-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b294-125">Authorization</span></span> | <span data-ttu-id="2b294-126">string</span><span class="sxs-lookup"><span data-stu-id="2b294-126">string</span></span> | <span data-ttu-id="2b294-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b294-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b294-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2b294-129">Request body</span></span>

<span data-ttu-id="2b294-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b294-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b294-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b294-131">Response</span></span>

<span data-ttu-id="2b294-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b294-132">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b294-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2b294-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2b294-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b294-134">Request</span></span>

<span data-ttu-id="2b294-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b294-135">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```

##### <a name="response"></a><span data-ttu-id="2b294-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b294-136">Response</span></span>

<span data-ttu-id="2b294-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b294-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
