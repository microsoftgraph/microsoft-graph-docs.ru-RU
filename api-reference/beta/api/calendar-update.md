---
title: Обновление календаря
description: 'Обновление свойств объекта calendar. Это может быть календарь для ресурса user '
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e68e33ba57b784af10e1b0b22e271ca0da1bbaf3
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895631"
---
# <a name="update-calendar"></a><span data-ttu-id="87fa0-104">Обновление календаря</span><span class="sxs-lookup"><span data-stu-id="87fa0-104">Update calendar</span></span>

<span data-ttu-id="87fa0-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87fa0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87fa0-106">Обновление свойств объекта [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="87fa0-106">Update the properties of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="87fa0-107">В качестве календаря может использоваться календарь [пользователя](../resources/user.md)или стандартный календарь [группы](../resources/group.md)Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="87fa0-107">The calendar can be one for a [user](../resources/user.md), or the default calendar of a Microsoft 365 [group](../resources/group.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="87fa0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87fa0-108">Permissions</span></span>
<span data-ttu-id="87fa0-109">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="87fa0-109">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="87fa0-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87fa0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="87fa0-111">Календарь</span><span class="sxs-lookup"><span data-stu-id="87fa0-111">Calendar</span></span> | <span data-ttu-id="87fa0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87fa0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="87fa0-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87fa0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87fa0-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="87fa0-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="87fa0-115">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="87fa0-115">user calendar</span></span> | <span data-ttu-id="87fa0-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87fa0-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="87fa0-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87fa0-117">Calendars.ReadWrite</span></span> | <span data-ttu-id="87fa0-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87fa0-118">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="87fa0-119">календарь группы</span><span class="sxs-lookup"><span data-stu-id="87fa0-119">group calendar</span></span> | <span data-ttu-id="87fa0-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87fa0-120">Group.ReadWrite.All</span></span> | <span data-ttu-id="87fa0-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87fa0-121">Not supported.</span></span> | <span data-ttu-id="87fa0-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87fa0-122">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="87fa0-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87fa0-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="87fa0-124">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="87fa0-124">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="87fa0-125">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="87fa0-125">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="87fa0-126">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="87fa0-126">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="87fa0-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87fa0-127">Request headers</span></span>
| <span data-ttu-id="87fa0-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87fa0-128">Header</span></span>       | <span data-ttu-id="87fa0-129">Значение</span><span class="sxs-lookup"><span data-stu-id="87fa0-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="87fa0-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87fa0-130">Authorization</span></span>  | <span data-ttu-id="87fa0-131">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="87fa0-131">Bearer {token}.</span></span> <span data-ttu-id="87fa0-132">Required.</span><span class="sxs-lookup"><span data-stu-id="87fa0-132">Required.</span></span>  |
| <span data-ttu-id="87fa0-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="87fa0-133">Content-Type</span></span>  | <span data-ttu-id="87fa0-134">application/json.</span><span class="sxs-lookup"><span data-stu-id="87fa0-134">application/json.</span></span> <span data-ttu-id="87fa0-135">Required.</span><span class="sxs-lookup"><span data-stu-id="87fa0-135">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="87fa0-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87fa0-136">Request body</span></span>
<span data-ttu-id="87fa0-137">In the request body, supply the values for relevant fields that should be updated.</span><span class="sxs-lookup"><span data-stu-id="87fa0-137">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="87fa0-138">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span><span class="sxs-lookup"><span data-stu-id="87fa0-138">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="87fa0-139">For best performance you shouldn't include existing values that haven't changed.</span><span class="sxs-lookup"><span data-stu-id="87fa0-139">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="87fa0-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="87fa0-140">Property</span></span>     | <span data-ttu-id="87fa0-141">Тип</span><span class="sxs-lookup"><span data-stu-id="87fa0-141">Type</span></span>   |<span data-ttu-id="87fa0-142">Описание</span><span class="sxs-lookup"><span data-stu-id="87fa0-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87fa0-143">color</span><span class="sxs-lookup"><span data-stu-id="87fa0-143">color</span></span>|<span data-ttu-id="87fa0-144">String</span><span class="sxs-lookup"><span data-stu-id="87fa0-144">String</span></span>|<span data-ttu-id="87fa0-145">Specifies the color theme to distinguish the calendar from other calendars in a UI.</span><span class="sxs-lookup"><span data-stu-id="87fa0-145">Specifies the color theme to distinguish the calendar from other calendars in a UI.</span></span> <span data-ttu-id="87fa0-146">The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="87fa0-146">The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="87fa0-147">isDefaultCalendar</span><span class="sxs-lookup"><span data-stu-id="87fa0-147">isDefaultCalendar</span></span>|<span data-ttu-id="87fa0-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="87fa0-148">Boolean</span></span>|<span data-ttu-id="87fa0-149">Значение true, если это используемый по умолчанию календарь пользователя. В противном случае используется значение false.</span><span class="sxs-lookup"><span data-stu-id="87fa0-149">True if this calendar is the user's default calendar, false otherwise.</span></span>|
|<span data-ttu-id="87fa0-150">name</span><span class="sxs-lookup"><span data-stu-id="87fa0-150">name</span></span>|<span data-ttu-id="87fa0-151">String</span><span class="sxs-lookup"><span data-stu-id="87fa0-151">String</span></span>|<span data-ttu-id="87fa0-152">Имя календаря.</span><span class="sxs-lookup"><span data-stu-id="87fa0-152">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="87fa0-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="87fa0-153">Response</span></span>

<span data-ttu-id="87fa0-154">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="87fa0-154">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87fa0-155">Пример</span><span class="sxs-lookup"><span data-stu-id="87fa0-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87fa0-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="87fa0-156">Request</span></span>
<span data-ttu-id="87fa0-157">В следующем примере обновляется имя календаря пользователя, вошедшего в систему по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="87fa0-157">The following example updates the name of the signed-in user's default calendar.</span></span>

# <a name="http"></a>[<span data-ttu-id="87fa0-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="87fa0-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="87fa0-159">C#</span><span class="sxs-lookup"><span data-stu-id="87fa0-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87fa0-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87fa0-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87fa0-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87fa0-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="87fa0-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="87fa0-162">Response</span></span>
<span data-ttu-id="87fa0-163">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="87fa0-163">Here is an example of the response.</span></span> <span data-ttu-id="87fa0-164">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="87fa0-164">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="87fa0-165">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="87fa0-165">All of the properties will be returned from an actual call.</span></span>
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
    "allowedOnlineMeetingProviders": [
                "teamsForBusiness"
            ],
    "defaultOnlineMeetingProvider": "teamsForBusiness",
    "isTallyingResponses": true,
    "isRemovable": false,
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
