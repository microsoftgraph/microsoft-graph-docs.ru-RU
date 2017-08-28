# <a name="update-calendar"></a><span data-ttu-id="da990-101">Обновление календаря</span><span class="sxs-lookup"><span data-stu-id="da990-101">Update calendar</span></span>

<span data-ttu-id="da990-102">Обновление свойств объекта календаря.</span><span class="sxs-lookup"><span data-stu-id="da990-102">Update the properties of calendar object.</span></span>
## <a name="permissions"></a><span data-ttu-id="da990-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da990-103">Permissions</span></span>
<span data-ttu-id="da990-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="da990-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="da990-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da990-106">Permission type</span></span>      | <span data-ttu-id="da990-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da990-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da990-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da990-108">Delegated (work or school account)</span></span> | <span data-ttu-id="da990-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da990-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="da990-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da990-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da990-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da990-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="da990-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da990-112">Application</span></span> | <span data-ttu-id="da990-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da990-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="da990-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da990-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="da990-115">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="da990-115">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="da990-116">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="da990-116">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="da990-117">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="da990-117">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="da990-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da990-118">Request headers</span></span>
| <span data-ttu-id="da990-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="da990-119">Header</span></span>       | <span data-ttu-id="da990-120">Значение</span><span class="sxs-lookup"><span data-stu-id="da990-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="da990-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da990-121">Authorization</span></span>  | <span data-ttu-id="da990-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da990-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="da990-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da990-124">Content-Type</span></span>  | <span data-ttu-id="da990-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da990-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="da990-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da990-127">Request body</span></span>
<span data-ttu-id="da990-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="da990-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="da990-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="da990-131">Property</span></span>     | <span data-ttu-id="da990-132">Тип</span><span class="sxs-lookup"><span data-stu-id="da990-132">Type</span></span>   |<span data-ttu-id="da990-133">Описание</span><span class="sxs-lookup"><span data-stu-id="da990-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da990-134">color</span><span class="sxs-lookup"><span data-stu-id="da990-134">color</span></span>|<span data-ttu-id="da990-135">String</span><span class="sxs-lookup"><span data-stu-id="da990-135">String</span></span>|<span data-ttu-id="da990-p105">Задает цветовую тему, отличающую этот календарь от других календарей в пользовательском интерфейсе. Значения свойств: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="da990-p105">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="da990-138">имя</span><span class="sxs-lookup"><span data-stu-id="da990-138">name</span></span>|<span data-ttu-id="da990-139">String</span><span class="sxs-lookup"><span data-stu-id="da990-139">String</span></span>|<span data-ttu-id="da990-140">Имя календаря.</span><span class="sxs-lookup"><span data-stu-id="da990-140">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="da990-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="da990-141">Response</span></span>

<span data-ttu-id="da990-142">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="da990-142">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da990-143">Пример</span><span class="sxs-lookup"><span data-stu-id="da990-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da990-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="da990-144">Request</span></span>
<span data-ttu-id="da990-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da990-145">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="da990-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="da990-146">Response</span></span>
<span data-ttu-id="da990-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="da990-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "owner":{
        "name":"Fanny Downs",
        "address":"fannyd@adatum.onmicrosoft.com"
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
