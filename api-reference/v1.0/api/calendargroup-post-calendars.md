---
title: Создание объекта Calendar
description: С помощью этого API можно для экземпляра user создать календарь в группе календарей.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 791615d7b934536a27d4a8d1ea88be42a4ca2d79
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928453"
---
# <a name="create-calendar"></a><span data-ttu-id="e8e20-103">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="e8e20-103">Create Calendar</span></span>

<span data-ttu-id="e8e20-104">С помощью этого API можно для экземпляра [user](../resources/user.md) создать календарь в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="e8e20-104">Use this API to create a new calendar in a calendar group for a [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e8e20-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8e20-105">Permissions</span></span>

<span data-ttu-id="e8e20-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8e20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8e20-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8e20-108">Permission type</span></span>                        | <span data-ttu-id="e8e20-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8e20-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e8e20-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8e20-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8e20-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8e20-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="e8e20-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8e20-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8e20-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8e20-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="e8e20-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8e20-114">Application</span></span>                            | <span data-ttu-id="e8e20-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8e20-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e8e20-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8e20-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="e8e20-117">Объект [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="e8e20-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="e8e20-118">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="e8e20-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a><span data-ttu-id="e8e20-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8e20-119">Request headers</span></span>

| <span data-ttu-id="e8e20-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8e20-120">Header</span></span>        | <span data-ttu-id="e8e20-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e8e20-121">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="e8e20-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8e20-122">Authorization</span></span> | <span data-ttu-id="e8e20-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8e20-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e8e20-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e8e20-125">Content-Type</span></span>  | <span data-ttu-id="e8e20-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8e20-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8e20-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8e20-128">Request body</span></span>

<span data-ttu-id="e8e20-129">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8e20-129">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e8e20-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8e20-130">Response</span></span>

<span data-ttu-id="e8e20-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8e20-131">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8e20-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e8e20-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e8e20-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8e20-133">Request</span></span>

<span data-ttu-id="e8e20-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8e20-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_calendar_from_calendargroup"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
Content-type: application/json
Content-length: 78

{
  "name": "name-value",
  "color": {
  }
}
```

<span data-ttu-id="e8e20-135">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8e20-135">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="e8e20-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8e20-136">Response</span></span>

<span data-ttu-id="e8e20-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e8e20-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
