---
title: Список объектов calendarGroup
description: Получение групп календарей пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 646a2566c11778282e5473258f867143b85a88ef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925394"
---
# <a name="list-calendargroups"></a><span data-ttu-id="be176-103">Список объектов calendarGroup</span><span class="sxs-lookup"><span data-stu-id="be176-103">List calendarGroups</span></span>

> <span data-ttu-id="be176-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="be176-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be176-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be176-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="be176-106">Получение групп календарей пользователя.</span><span class="sxs-lookup"><span data-stu-id="be176-106">Get the user's calendar groups.</span></span>
## <a name="permissions"></a><span data-ttu-id="be176-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be176-107">Permissions</span></span>
<span data-ttu-id="be176-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be176-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be176-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be176-110">Permission type</span></span>      | <span data-ttu-id="be176-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be176-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be176-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be176-112">Delegated (work or school account)</span></span> | <span data-ttu-id="be176-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be176-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="be176-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be176-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be176-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be176-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="be176-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be176-116">Application</span></span> | <span data-ttu-id="be176-117">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be176-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="be176-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be176-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/calendarGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="be176-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="be176-119">Optional query parameters</span></span>
<span data-ttu-id="be176-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="be176-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="be176-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be176-121">Request headers</span></span>
| <span data-ttu-id="be176-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be176-122">Header</span></span>       | <span data-ttu-id="be176-123">Значение</span><span class="sxs-lookup"><span data-stu-id="be176-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="be176-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be176-124">Authorization</span></span>  | <span data-ttu-id="be176-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be176-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="be176-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="be176-127">Content-Type</span></span>  | <span data-ttu-id="be176-128">application/json</span><span class="sxs-lookup"><span data-stu-id="be176-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="be176-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="be176-129">Request body</span></span>
<span data-ttu-id="be176-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be176-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be176-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="be176-131">Response</span></span>

<span data-ttu-id="be176-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [CalendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="be176-132">If successful, this method returns a `200 OK` response code and collection of [CalendarGroup](../resources/calendargroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be176-133">Пример</span><span class="sxs-lookup"><span data-stu-id="be176-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be176-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="be176-134">Request</span></span>
<span data-ttu-id="be176-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be176-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendargroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendarGroups
```
##### <a name="response"></a><span data-ttu-id="be176-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="be176-136">Response</span></span>
<span data-ttu-id="be176-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="be176-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 155

{
  "value": [
    {
      "name": "name-value",
      "classId": "classId-value",
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
  "description": "List calendarGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
