---
title: Обновление календаря
description: 'Обновление свойств объекта calendar. Это может быть календарь для ресурса user '
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 63ac3812bcf71418f8747502d6212be18d55dbaf
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897829"
---
# <a name="update-calendar"></a><span data-ttu-id="559c8-104">Обновление календаря</span><span class="sxs-lookup"><span data-stu-id="559c8-104">Update calendar</span></span>

<span data-ttu-id="559c8-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="559c8-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="559c8-106">Обновление свойств объекта [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="559c8-106">Update the properties of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="559c8-107">В качестве календаря может использоваться календарь [пользователя](../resources/user.md)или стандартный календарь [группы](../resources/group.md)Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="559c8-107">The calendar can be one for a [user](../resources/user.md), or the default calendar of a Microsoft 365 [group](../resources/group.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="559c8-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="559c8-108">Permissions</span></span>
<span data-ttu-id="559c8-109">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="559c8-109">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="559c8-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="559c8-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="559c8-111">Календарь</span><span class="sxs-lookup"><span data-stu-id="559c8-111">Calendar</span></span> | <span data-ttu-id="559c8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="559c8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="559c8-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="559c8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="559c8-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="559c8-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="559c8-115">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="559c8-115">user calendar</span></span> | <span data-ttu-id="559c8-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="559c8-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="559c8-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="559c8-117">Calendars.ReadWrite</span></span> | <span data-ttu-id="559c8-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="559c8-118">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="559c8-119">календарь группы</span><span class="sxs-lookup"><span data-stu-id="559c8-119">group calendar</span></span> | <span data-ttu-id="559c8-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="559c8-120">Group.ReadWrite.All</span></span> | <span data-ttu-id="559c8-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="559c8-121">Not supported.</span></span> | <span data-ttu-id="559c8-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="559c8-122">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="559c8-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="559c8-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="559c8-124">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="559c8-124">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="559c8-125">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="559c8-125">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="559c8-126">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="559c8-126">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="559c8-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="559c8-127">Request headers</span></span>
| <span data-ttu-id="559c8-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="559c8-128">Header</span></span>       | <span data-ttu-id="559c8-129">Значение</span><span class="sxs-lookup"><span data-stu-id="559c8-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="559c8-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="559c8-130">Authorization</span></span>  | <span data-ttu-id="559c8-131">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="559c8-131">Bearer {token}.</span></span> <span data-ttu-id="559c8-132">Required.</span><span class="sxs-lookup"><span data-stu-id="559c8-132">Required.</span></span>  |
| <span data-ttu-id="559c8-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="559c8-133">Content-Type</span></span>  | <span data-ttu-id="559c8-134">application/json.</span><span class="sxs-lookup"><span data-stu-id="559c8-134">application/json.</span></span> <span data-ttu-id="559c8-135">Required.</span><span class="sxs-lookup"><span data-stu-id="559c8-135">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="559c8-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="559c8-136">Request body</span></span>
<span data-ttu-id="559c8-137">In the request body, supply the values for relevant fields that should be updated.</span><span class="sxs-lookup"><span data-stu-id="559c8-137">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="559c8-138">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span><span class="sxs-lookup"><span data-stu-id="559c8-138">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="559c8-139">For best performance you shouldn't include existing values that haven't changed.</span><span class="sxs-lookup"><span data-stu-id="559c8-139">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="559c8-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="559c8-140">Property</span></span>     | <span data-ttu-id="559c8-141">Тип</span><span class="sxs-lookup"><span data-stu-id="559c8-141">Type</span></span>   |<span data-ttu-id="559c8-142">Описание</span><span class="sxs-lookup"><span data-stu-id="559c8-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="559c8-143">color</span><span class="sxs-lookup"><span data-stu-id="559c8-143">color</span></span>|<span data-ttu-id="559c8-144">String</span><span class="sxs-lookup"><span data-stu-id="559c8-144">String</span></span>|<span data-ttu-id="559c8-145">Specifies the color theme to distinguish the calendar from other calendars in a UI.</span><span class="sxs-lookup"><span data-stu-id="559c8-145">Specifies the color theme to distinguish the calendar from other calendars in a UI.</span></span> <span data-ttu-id="559c8-146">The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="559c8-146">The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="559c8-147">name</span><span class="sxs-lookup"><span data-stu-id="559c8-147">name</span></span>|<span data-ttu-id="559c8-148">String</span><span class="sxs-lookup"><span data-stu-id="559c8-148">String</span></span>|<span data-ttu-id="559c8-149">Имя календаря.</span><span class="sxs-lookup"><span data-stu-id="559c8-149">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="559c8-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="559c8-150">Response</span></span>

<span data-ttu-id="559c8-151">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="559c8-151">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="559c8-152">Пример</span><span class="sxs-lookup"><span data-stu-id="559c8-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="559c8-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="559c8-153">Request</span></span>
<span data-ttu-id="559c8-154">В следующем примере обновляется имя календаря пользователя, вошедшего в систему по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="559c8-154">The following example updates the name of the signed-in user's default calendar.</span></span>

# <a name="http"></a>[<span data-ttu-id="559c8-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="559c8-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_calendar"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/calendar
Content-type: application/json

{
  "name": "Social events"
}
```
# <a name="c"></a>[<span data-ttu-id="559c8-156">C#</span><span class="sxs-lookup"><span data-stu-id="559c8-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="559c8-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="559c8-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="559c8-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="559c8-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="559c8-159">Java</span><span class="sxs-lookup"><span data-stu-id="559c8-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="559c8-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="559c8-160">Response</span></span>
<span data-ttu-id="559c8-161">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="559c8-161">Here is an example of the response.</span></span> <span data-ttu-id="559c8-162">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="559c8-162">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="559c8-163">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="559c8-163">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Social events",
    "color":"auto",
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
    "canShare":true,
    "canViewPrivateItems":true,
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
<!-- {
  "type": "#page.annotation",
  "description": "Update calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
