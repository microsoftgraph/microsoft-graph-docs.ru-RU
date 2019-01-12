---
title: Обновление календаря
description: 'Обновление свойств объекта calendar. Календарь может иметь одно для пользователя '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: a9b9ac65fa5d03b73a7508f6032ebe199118b09c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922497"
---
# <a name="update-calendar"></a><span data-ttu-id="7e0ba-104">Обновление календаря</span><span class="sxs-lookup"><span data-stu-id="7e0ba-104">Update calendar</span></span>

> <span data-ttu-id="7e0ba-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7e0ba-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e0ba-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e0ba-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7e0ba-107">Обновление свойств объекта [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="7e0ba-107">Update the properties of of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="7e0ba-108">Это может быть календарь для ресурса [user](../resources/user.md) или стандартный календарь для ресурса [group](../resources/group.md), представляющего группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="7e0ba-108">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="7e0ba-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e0ba-109">Permissions</span></span>
<span data-ttu-id="7e0ba-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e0ba-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e0ba-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e0ba-112">Permission type</span></span>      | <span data-ttu-id="7e0ba-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e0ba-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e0ba-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e0ba-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7e0ba-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e0ba-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7e0ba-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e0ba-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e0ba-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e0ba-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7e0ba-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e0ba-118">Application</span></span> | <span data-ttu-id="7e0ba-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e0ba-119">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e0ba-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e0ba-120">HTTP request</span></span>
<span data-ttu-id="7e0ba-121"><!-- { "blockType": "ignored" } -->Пользователя или группы по умолчанию [календаря](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="7e0ba-121"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="7e0ba-122">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="7e0ba-122">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="7e0ba-123">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="7e0ba-123">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7e0ba-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e0ba-124">Request headers</span></span>
| <span data-ttu-id="7e0ba-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e0ba-125">Header</span></span>       | <span data-ttu-id="7e0ba-126">Значение</span><span class="sxs-lookup"><span data-stu-id="7e0ba-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7e0ba-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e0ba-127">Authorization</span></span>  | <span data-ttu-id="7e0ba-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e0ba-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7e0ba-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7e0ba-130">Content-Type</span></span>  | <span data-ttu-id="7e0ba-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e0ba-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7e0ba-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7e0ba-133">Request body</span></span>
<span data-ttu-id="7e0ba-p107">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7e0ba-p107">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7e0ba-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e0ba-137">Property</span></span>     | <span data-ttu-id="7e0ba-138">Тип</span><span class="sxs-lookup"><span data-stu-id="7e0ba-138">Type</span></span>   |<span data-ttu-id="7e0ba-139">Описание</span><span class="sxs-lookup"><span data-stu-id="7e0ba-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e0ba-140">color</span><span class="sxs-lookup"><span data-stu-id="7e0ba-140">color</span></span>|<span data-ttu-id="7e0ba-141">String</span><span class="sxs-lookup"><span data-stu-id="7e0ba-141">String</span></span>|<span data-ttu-id="7e0ba-p108">Задает цветовую тему, отличающую этот календарь от других календарей в пользовательском интерфейсе. Значения свойств: LightBlue = 0, LightGreen = 1, LightOrange = 2, LightGray = 3, LightYellow = 4, LightTeal = 5, LightPink = 6, LightBrown = 7, LightRed = 8, MaxColor = 9, Auto = -1.</span><span class="sxs-lookup"><span data-stu-id="7e0ba-p108">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="7e0ba-144">isDefaultCalendar</span><span class="sxs-lookup"><span data-stu-id="7e0ba-144">isDefaultCalendar</span></span>|<span data-ttu-id="7e0ba-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e0ba-145">Boolean</span></span>|<span data-ttu-id="7e0ba-146">Значение true, если этот календарь является пользователя по умолчанию, значение false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="7e0ba-146">True if this calendar is the user's default calendar, false otherwise.</span></span>|
|<span data-ttu-id="7e0ba-147">name</span><span class="sxs-lookup"><span data-stu-id="7e0ba-147">name</span></span>|<span data-ttu-id="7e0ba-148">String</span><span class="sxs-lookup"><span data-stu-id="7e0ba-148">String</span></span>|<span data-ttu-id="7e0ba-149">Имя календаря.</span><span class="sxs-lookup"><span data-stu-id="7e0ba-149">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="7e0ba-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e0ba-150">Response</span></span>

<span data-ttu-id="7e0ba-151">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7e0ba-151">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7e0ba-152">Пример</span><span class="sxs-lookup"><span data-stu-id="7e0ba-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e0ba-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e0ba-153">Request</span></span>
<span data-ttu-id="7e0ba-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e0ba-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_calendar"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/calendar
Content-type: application/json

{
  "name": "Social events"
}
```
##### <a name="response"></a><span data-ttu-id="7e0ba-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e0ba-155">Response</span></span>
<span data-ttu-id="7e0ba-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7e0ba-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Social events",
    "color":"auto",
    "hexColor": "",
    "isDefaultCalendar":false,
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
    "canShare":true,
    "canViewPrivateItems":true,
    "isShared":false,
    "isSharedWithMe":false,
    "canEdit":true,
    "owner":{
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
