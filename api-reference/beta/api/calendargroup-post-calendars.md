---
title: Создание объекта Calendar
description: С помощью этого API можно для экземпляра user создать календарь в группе календарей.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 5cb13fc6259d21a752160b2a932f9a7c5b2330bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819735"
---
# <a name="create-calendar"></a><span data-ttu-id="38bfb-103">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="38bfb-103">Create Calendar</span></span>

> <span data-ttu-id="38bfb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="38bfb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38bfb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38bfb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="38bfb-106">С помощью этого API можно для экземпляра [user](../resources/user.md) создать календарь в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="38bfb-106">Use this API to create a new calendar in a calendar group for a [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="38bfb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="38bfb-107">Permissions</span></span>

<span data-ttu-id="38bfb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38bfb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38bfb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38bfb-110">Permission type</span></span>                        | <span data-ttu-id="38bfb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="38bfb-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="38bfb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38bfb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="38bfb-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38bfb-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="38bfb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38bfb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38bfb-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38bfb-115">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="38bfb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38bfb-116">Application</span></span>                            | <span data-ttu-id="38bfb-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38bfb-117">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="38bfb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38bfb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="38bfb-119">Объект [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="38bfb-119">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="38bfb-120">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="38bfb-120">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a><span data-ttu-id="38bfb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38bfb-121">Request headers</span></span>

| <span data-ttu-id="38bfb-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38bfb-122">Header</span></span>        | <span data-ttu-id="38bfb-123">Значение</span><span class="sxs-lookup"><span data-stu-id="38bfb-123">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="38bfb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38bfb-124">Authorization</span></span> | <span data-ttu-id="38bfb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38bfb-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="38bfb-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="38bfb-127">Content-Type</span></span>  | <span data-ttu-id="38bfb-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38bfb-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38bfb-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38bfb-130">Request body</span></span>

<span data-ttu-id="38bfb-131">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38bfb-131">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="38bfb-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="38bfb-132">Response</span></span>

<span data-ttu-id="38bfb-133">В случае успеха этот метод возвращает код отклика `201 Created` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="38bfb-133">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38bfb-134">Пример</span><span class="sxs-lookup"><span data-stu-id="38bfb-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="38bfb-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="38bfb-135">Request</span></span>

<span data-ttu-id="38bfb-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38bfb-136">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_calendar_from_calendargroup"
}-->

```http
POST https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
Content-type: application/json
Content-length: 78

{
  "name": "name-value",
  "color": {
  }
}
```

<span data-ttu-id="38bfb-137">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38bfb-137">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="38bfb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="38bfb-138">Response</span></span>

<span data-ttu-id="38bfb-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="38bfb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "name": "name-value",
  "color": {
  },
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
