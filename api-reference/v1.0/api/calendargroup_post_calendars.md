# <a name="create-calendar"></a><span data-ttu-id="33272-101">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="33272-101">Create Calendar</span></span>

<span data-ttu-id="33272-102">С помощью этого API можно для экземпляра [user](../resources/user.md) создать календарь в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="33272-102">Use this API to create a new calendar in a calendar group for a [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="33272-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33272-103">Permissions</span></span>

<span data-ttu-id="33272-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="33272-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="33272-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33272-106">Permission type</span></span>                        | <span data-ttu-id="33272-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33272-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="33272-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33272-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="33272-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33272-109">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="33272-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33272-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33272-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33272-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="33272-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33272-112">Application</span></span>                            | <span data-ttu-id="33272-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33272-113">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="33272-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33272-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="33272-115">Объект [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="33272-115">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="33272-116">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="33272-116">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a><span data-ttu-id="33272-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33272-117">Request headers</span></span>

| <span data-ttu-id="33272-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33272-118">Header</span></span>        | <span data-ttu-id="33272-119">Значение</span><span class="sxs-lookup"><span data-stu-id="33272-119">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="33272-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33272-120">Authorization</span></span> | <span data-ttu-id="33272-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33272-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="33272-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="33272-123">Content-Type</span></span>  | <span data-ttu-id="33272-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33272-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33272-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33272-126">Request body</span></span>

<span data-ttu-id="33272-127">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33272-127">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="33272-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="33272-128">Response</span></span>

<span data-ttu-id="33272-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="33272-129">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33272-130">Пример</span><span class="sxs-lookup"><span data-stu-id="33272-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="33272-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="33272-131">Request</span></span>

<span data-ttu-id="33272-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33272-132">Here is an example of the request.</span></span>

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

<span data-ttu-id="33272-133">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33272-133">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="33272-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="33272-134">Response</span></span>

<span data-ttu-id="33272-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="33272-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
