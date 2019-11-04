---
title: Обновление календаря
description: 'Обновление свойств объекта calendar. Это может быть календарь для ресурса user '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f4817b4121f238246338d6a3ed6f66015ebc3a05
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936820"
---
# <a name="update-calendar"></a><span data-ttu-id="d4509-104">Обновление календаря</span><span class="sxs-lookup"><span data-stu-id="d4509-104">Update calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4509-105">Обновление свойств объекта [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="d4509-105">Update the properties of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="d4509-106">Это может быть календарь для ресурса [user](../resources/user.md) или стандартный календарь для ресурса [group](../resources/group.md), представляющего группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="d4509-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="d4509-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4509-107">Permissions</span></span>
<span data-ttu-id="d4509-108">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="d4509-108">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="d4509-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4509-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4509-110">Календарь</span><span class="sxs-lookup"><span data-stu-id="d4509-110">Calendar</span></span> | <span data-ttu-id="d4509-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4509-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d4509-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4509-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4509-113">Приложение</span><span class="sxs-lookup"><span data-stu-id="d4509-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="d4509-114">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="d4509-114">user calendar</span></span> | <span data-ttu-id="d4509-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4509-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="d4509-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4509-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="d4509-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4509-117">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="d4509-118">календарь группы</span><span class="sxs-lookup"><span data-stu-id="d4509-118">group calendar</span></span> | <span data-ttu-id="d4509-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4509-119">Group.ReadWrite.All</span></span> | <span data-ttu-id="d4509-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4509-120">Not supported.</span></span> | <span data-ttu-id="d4509-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4509-121">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="d4509-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4509-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="d4509-123">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d4509-123">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="d4509-124">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="d4509-124">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="d4509-125">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="d4509-125">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d4509-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4509-126">Request headers</span></span>
| <span data-ttu-id="d4509-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4509-127">Header</span></span>       | <span data-ttu-id="d4509-128">Значение</span><span class="sxs-lookup"><span data-stu-id="d4509-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d4509-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4509-129">Authorization</span></span>  | <span data-ttu-id="d4509-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4509-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d4509-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d4509-132">Content-Type</span></span>  | <span data-ttu-id="d4509-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4509-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d4509-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4509-135">Request body</span></span>
<span data-ttu-id="d4509-p106">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d4509-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d4509-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4509-139">Property</span></span>     | <span data-ttu-id="d4509-140">Тип</span><span class="sxs-lookup"><span data-stu-id="d4509-140">Type</span></span>   |<span data-ttu-id="d4509-141">Описание</span><span class="sxs-lookup"><span data-stu-id="d4509-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4509-142">color</span><span class="sxs-lookup"><span data-stu-id="d4509-142">color</span></span>|<span data-ttu-id="d4509-143">String</span><span class="sxs-lookup"><span data-stu-id="d4509-143">String</span></span>|<span data-ttu-id="d4509-p107">Задает цветовую тему, отличающую этот календарь от других календарей в пользовательском интерфейсе. Значения свойств: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="d4509-p107">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="d4509-146">isDefaultCalendar</span><span class="sxs-lookup"><span data-stu-id="d4509-146">isDefaultCalendar</span></span>|<span data-ttu-id="d4509-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4509-147">Boolean</span></span>|<span data-ttu-id="d4509-148">Значение true, если это используемый по умолчанию календарь пользователя. В противном случае используется значение false.</span><span class="sxs-lookup"><span data-stu-id="d4509-148">True if this calendar is the user's default calendar, false otherwise.</span></span>|
|<span data-ttu-id="d4509-149">name</span><span class="sxs-lookup"><span data-stu-id="d4509-149">name</span></span>|<span data-ttu-id="d4509-150">String</span><span class="sxs-lookup"><span data-stu-id="d4509-150">String</span></span>|<span data-ttu-id="d4509-151">Имя календаря.</span><span class="sxs-lookup"><span data-stu-id="d4509-151">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="d4509-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4509-152">Response</span></span>

<span data-ttu-id="d4509-153">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4509-153">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d4509-154">Пример</span><span class="sxs-lookup"><span data-stu-id="d4509-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d4509-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4509-155">Request</span></span>
<span data-ttu-id="d4509-156">В следующем примере обновляется имя календаря пользователя, вошедшего в систему по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d4509-156">The following example updates the name of the signed-in user's default calendar.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d4509-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4509-157">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d4509-158">C#</span><span class="sxs-lookup"><span data-stu-id="d4509-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d4509-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4509-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d4509-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4509-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d4509-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4509-161">Response</span></span>
<span data-ttu-id="d4509-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4509-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
