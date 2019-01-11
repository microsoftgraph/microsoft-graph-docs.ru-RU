---
title: Удаление календаря
description: Удаление календаря, отличного от календаря по умолчанию.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: e489a0807f9069f3198f11955daba828b9c929e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823704"
---
# <a name="delete-calendar"></a><span data-ttu-id="d1012-103">Удаление календаря</span><span class="sxs-lookup"><span data-stu-id="d1012-103">Delete calendar</span></span>

<span data-ttu-id="d1012-104">Удаление календаря, отличного от календаря по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d1012-104">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="d1012-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1012-105">Permissions</span></span>
<span data-ttu-id="d1012-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1012-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1012-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1012-108">Permission type</span></span>      | <span data-ttu-id="d1012-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1012-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1012-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1012-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d1012-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1012-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d1012-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1012-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1012-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1012-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d1012-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1012-114">Application</span></span> | <span data-ttu-id="d1012-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1012-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1012-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1012-116">HTTP request</span></span>
<span data-ttu-id="d1012-117"><!-- { "blockType": "ignored" } -->Пользователя [календаря](../resources/calendar.md) , отличный от календаря по умолчанию в [calendarGroup](../resources/calendargroup.md)по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d1012-117"><!-- { "blockType": "ignored" } --> A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="d1012-118">[Календарь](../resources/calendar.md), отличный от календаря по умолчанию, в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="d1012-118">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d1012-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1012-119">Request headers</span></span>
| <span data-ttu-id="d1012-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d1012-120">Name</span></span>           |  <span data-ttu-id="d1012-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d1012-121">Type</span></span>    | <span data-ttu-id="d1012-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d1012-122">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="d1012-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1012-123">Authorization</span></span>  |  <span data-ttu-id="d1012-124">string</span><span class="sxs-lookup"><span data-stu-id="d1012-124">string</span></span>  | <span data-ttu-id="d1012-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1012-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1012-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1012-127">Request body</span></span>
<span data-ttu-id="d1012-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d1012-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1012-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1012-129">Response</span></span>

<span data-ttu-id="d1012-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d1012-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1012-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d1012-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1012-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1012-133">Request</span></span>
<span data-ttu-id="d1012-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1012-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="d1012-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="d1012-135">Response</span></span>
<span data-ttu-id="d1012-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d1012-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
