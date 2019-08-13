---
title: Обновление календаря
description: 'Обновление свойств объекта calendar. Это может быть календарь для ресурса user '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fe2a985e6b232a9f7578c1dcd615d16fd42aede2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317846"
---
# <a name="update-calendar"></a><span data-ttu-id="e49f8-104">Обновление календаря</span><span class="sxs-lookup"><span data-stu-id="e49f8-104">Update calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e49f8-105">Обновление свойств объекта [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="e49f8-105">Update the properties of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="e49f8-106">Это может быть календарь для ресурса [user](../resources/user.md) или стандартный календарь для ресурса [group](../resources/group.md), представляющего группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="e49f8-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="e49f8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e49f8-107">Permissions</span></span>
<span data-ttu-id="e49f8-108">В зависимости от типа календаря, в котором находится событие, и запрошенного типа разрешения (делегированного или приложения), для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="e49f8-108">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="e49f8-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e49f8-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e49f8-110">Календарь</span><span class="sxs-lookup"><span data-stu-id="e49f8-110">Calendar</span></span> | <span data-ttu-id="e49f8-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e49f8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e49f8-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e49f8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e49f8-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e49f8-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="e49f8-114">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="e49f8-114">user calendar</span></span> | <span data-ttu-id="e49f8-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e49f8-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="e49f8-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e49f8-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="e49f8-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e49f8-117">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="e49f8-118">calendar для групп;</span><span class="sxs-lookup"><span data-stu-id="e49f8-118">group calendar</span></span> | <span data-ttu-id="e49f8-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e49f8-119">Group.ReadWrite.All</span></span> | <span data-ttu-id="e49f8-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e49f8-120">Not supported.</span></span> | <span data-ttu-id="e49f8-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e49f8-121">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="e49f8-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e49f8-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="e49f8-123">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e49f8-123">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="e49f8-124">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="e49f8-124">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="e49f8-125">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="e49f8-125">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e49f8-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e49f8-126">Request headers</span></span>
| <span data-ttu-id="e49f8-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e49f8-127">Header</span></span>       | <span data-ttu-id="e49f8-128">Значение</span><span class="sxs-lookup"><span data-stu-id="e49f8-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e49f8-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e49f8-129">Authorization</span></span>  | <span data-ttu-id="e49f8-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e49f8-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e49f8-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e49f8-132">Content-Type</span></span>  | <span data-ttu-id="e49f8-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e49f8-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e49f8-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e49f8-135">Request body</span></span>
<span data-ttu-id="e49f8-p106">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e49f8-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e49f8-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="e49f8-139">Property</span></span>     | <span data-ttu-id="e49f8-140">Тип</span><span class="sxs-lookup"><span data-stu-id="e49f8-140">Type</span></span>   |<span data-ttu-id="e49f8-141">Описание</span><span class="sxs-lookup"><span data-stu-id="e49f8-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e49f8-142">color</span><span class="sxs-lookup"><span data-stu-id="e49f8-142">color</span></span>|<span data-ttu-id="e49f8-143">String</span><span class="sxs-lookup"><span data-stu-id="e49f8-143">String</span></span>|<span data-ttu-id="e49f8-p107">Задает цветовую тему, отличающую этот календарь от других календарей в пользовательском интерфейсе. Значения свойств: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="e49f8-p107">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="e49f8-146">isDefaultCalendar</span><span class="sxs-lookup"><span data-stu-id="e49f8-146">isDefaultCalendar</span></span>|<span data-ttu-id="e49f8-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="e49f8-147">Boolean</span></span>|<span data-ttu-id="e49f8-148">Значение true, если это используемый по умолчанию календарь пользователя. В противном случае используется значение false.</span><span class="sxs-lookup"><span data-stu-id="e49f8-148">True if this calendar is the user's default calendar, false otherwise.</span></span>|
|<span data-ttu-id="e49f8-149">name</span><span class="sxs-lookup"><span data-stu-id="e49f8-149">name</span></span>|<span data-ttu-id="e49f8-150">String</span><span class="sxs-lookup"><span data-stu-id="e49f8-150">String</span></span>|<span data-ttu-id="e49f8-151">Имя календаря.</span><span class="sxs-lookup"><span data-stu-id="e49f8-151">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="e49f8-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="e49f8-152">Response</span></span>

<span data-ttu-id="e49f8-153">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e49f8-153">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e49f8-154">Пример</span><span class="sxs-lookup"><span data-stu-id="e49f8-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e49f8-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="e49f8-155">Request</span></span>
<span data-ttu-id="e49f8-156">В следующем примере обновляется имя календаря пользователя, вошедшего в систему по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e49f8-156">The following example updates the name of the signed-in user's default calendar.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e49f8-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="e49f8-157">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="e49f8-158">C#</span><span class="sxs-lookup"><span data-stu-id="e49f8-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e49f8-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e49f8-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e49f8-160">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e49f8-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e49f8-161">Java</span><span class="sxs-lookup"><span data-stu-id="e49f8-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e49f8-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="e49f8-162">Response</span></span>
<span data-ttu-id="e49f8-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e49f8-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
