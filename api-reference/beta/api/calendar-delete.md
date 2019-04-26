---
title: Удаление календаря
description: Удаление календаря, отличного от календаря по умолчанию.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a5ace08afb8f496d34f8cd86660cb73d69e3cda9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322386"
---
# <a name="delete-calendar"></a><span data-ttu-id="84bcb-103">Удаление календаря</span><span class="sxs-lookup"><span data-stu-id="84bcb-103">Delete calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84bcb-104">Удаление календаря, отличного от календаря по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="84bcb-104">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="84bcb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84bcb-105">Permissions</span></span>
<span data-ttu-id="84bcb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84bcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84bcb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84bcb-108">Permission type</span></span>      | <span data-ttu-id="84bcb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84bcb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84bcb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84bcb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="84bcb-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84bcb-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="84bcb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84bcb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84bcb-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84bcb-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="84bcb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84bcb-114">Application</span></span> | <span data-ttu-id="84bcb-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84bcb-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="84bcb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84bcb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="84bcb-117">[Календарь](../resources/calendar.md) пользователя, отличный от календаря по умолчанию, в группе [calendarGroup](../resources/calendargroup.md) по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="84bcb-117">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="84bcb-118">[Календарь](../resources/calendar.md), отличный от календаря по умолчанию, в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="84bcb-118">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="84bcb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84bcb-119">Request headers</span></span>
| <span data-ttu-id="84bcb-120">Имя</span><span class="sxs-lookup"><span data-stu-id="84bcb-120">Name</span></span>           |  <span data-ttu-id="84bcb-121">Тип</span><span class="sxs-lookup"><span data-stu-id="84bcb-121">Type</span></span>    | <span data-ttu-id="84bcb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="84bcb-122">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="84bcb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="84bcb-123">Authorization</span></span>  |  <span data-ttu-id="84bcb-124">string</span><span class="sxs-lookup"><span data-stu-id="84bcb-124">string</span></span>  | <span data-ttu-id="84bcb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84bcb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84bcb-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="84bcb-127">Request body</span></span>
<span data-ttu-id="84bcb-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84bcb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84bcb-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="84bcb-129">Response</span></span>

<span data-ttu-id="84bcb-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="84bcb-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84bcb-132">Пример</span><span class="sxs-lookup"><span data-stu-id="84bcb-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84bcb-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="84bcb-133">Request</span></span>
<span data-ttu-id="84bcb-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84bcb-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/calendar
```
##### <a name="response"></a><span data-ttu-id="84bcb-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="84bcb-135">Response</span></span>
<span data-ttu-id="84bcb-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="84bcb-136">Here is an example of the response.</span></span> 
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
  "suppressions": []
}
-->
