# <a name="create-calendargroup"></a><span data-ttu-id="cc93d-101">Создание объекта CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="cc93d-101">Create CalendarGroup</span></span>

<span data-ttu-id="cc93d-102">С помощью этого API можно создать экземпляр CalendarGroup.</span><span class="sxs-lookup"><span data-stu-id="cc93d-102">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="cc93d-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc93d-103">Permissions</span></span>
<span data-ttu-id="cc93d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cc93d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cc93d-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc93d-106">Permission type</span></span>      | <span data-ttu-id="cc93d-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc93d-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="cc93d-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc93d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cc93d-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc93d-109">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="cc93d-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc93d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc93d-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc93d-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="cc93d-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc93d-112">Application</span></span> | <span data-ttu-id="cc93d-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc93d-113">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cc93d-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc93d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="cc93d-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc93d-115">Request headers</span></span>
| <span data-ttu-id="cc93d-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc93d-116">Header</span></span>       | <span data-ttu-id="cc93d-117">Значение</span><span class="sxs-lookup"><span data-stu-id="cc93d-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc93d-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc93d-118">Authorization</span></span>  | <span data-ttu-id="cc93d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc93d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cc93d-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc93d-121">Content-Type</span></span>  | <span data-ttu-id="cc93d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="cc93d-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc93d-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc93d-123">Request body</span></span>
<span data-ttu-id="cc93d-124">Предоставьте в тексте запроса описание объекта [CalendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc93d-124">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cc93d-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc93d-125">Response</span></span>

<span data-ttu-id="cc93d-126">В случае успеха этот метод возвращает код отклика `201, Created` и объект [CalendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cc93d-126">If successful, this method returns `201, Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc93d-127">Пример</span><span class="sxs-lookup"><span data-stu-id="cc93d-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc93d-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc93d-128">Request</span></span>
<span data-ttu-id="cc93d-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc93d-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
<span data-ttu-id="cc93d-130">Предоставьте в тексте запроса описание объекта [calendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc93d-130">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cc93d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc93d-131">Response</span></span>
<span data-ttu-id="cc93d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cc93d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
