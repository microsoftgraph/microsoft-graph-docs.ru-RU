---
title: Удаление календаря
description: Удаление календаря, отличного от календаря по умолчанию.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1bdba9bb9da0ad0277ba73c4f2c28eec13072913
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511571"
---
# <a name="delete-calendar"></a><span data-ttu-id="fe82d-103">Удаление календаря</span><span class="sxs-lookup"><span data-stu-id="fe82d-103">Delete calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe82d-104">Удаление календаря, отличного от календаря по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fe82d-104">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe82d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe82d-105">Permissions</span></span>
<span data-ttu-id="fe82d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe82d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe82d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe82d-108">Permission type</span></span>      | <span data-ttu-id="fe82d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe82d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe82d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe82d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fe82d-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe82d-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fe82d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe82d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe82d-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe82d-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fe82d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe82d-114">Application</span></span> | <span data-ttu-id="fe82d-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe82d-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe82d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe82d-116">HTTP request</span></span>
<span data-ttu-id="fe82d-117"><!-- { "blockType": "ignored" } -->Пользователя [календаря](../resources/calendar.md) , отличный от календаря по умолчанию в [calendarGroup](../resources/calendargroup.md)по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fe82d-117"><!-- { "blockType": "ignored" } --> A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="fe82d-118">[Календарь](../resources/calendar.md), отличный от календаря по умолчанию, в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="fe82d-118">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fe82d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe82d-119">Request headers</span></span>
| <span data-ttu-id="fe82d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fe82d-120">Name</span></span>           |  <span data-ttu-id="fe82d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fe82d-121">Type</span></span>    | <span data-ttu-id="fe82d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fe82d-122">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="fe82d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe82d-123">Authorization</span></span>  |  <span data-ttu-id="fe82d-124">string</span><span class="sxs-lookup"><span data-stu-id="fe82d-124">string</span></span>  | <span data-ttu-id="fe82d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe82d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe82d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe82d-127">Request body</span></span>
<span data-ttu-id="fe82d-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fe82d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe82d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe82d-129">Response</span></span>

<span data-ttu-id="fe82d-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="fe82d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe82d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fe82d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe82d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe82d-133">Request</span></span>
<span data-ttu-id="fe82d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe82d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/calendar
```
##### <a name="response"></a><span data-ttu-id="fe82d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe82d-135">Response</span></span>
<span data-ttu-id="fe82d-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fe82d-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/calendar-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
