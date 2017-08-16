# <a name="create-calendar"></a><span data-ttu-id="614aa-101">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="614aa-101">Create Calendar</span></span>

<span data-ttu-id="614aa-102">С помощью этого API можно создать календарь.</span><span class="sxs-lookup"><span data-stu-id="614aa-102">Use this API to create a new calendar.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="614aa-103">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="614aa-103">Prerequisites</span></span>
<span data-ttu-id="614aa-104">Для применения этого API требуется одна из указанных **областей**: *Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="614aa-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="614aa-105">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="614aa-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="614aa-106">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="614aa-106">Request headers</span></span>
| <span data-ttu-id="614aa-107">Заголовок</span><span class="sxs-lookup"><span data-stu-id="614aa-107">Header</span></span>       | <span data-ttu-id="614aa-108">Значение</span><span class="sxs-lookup"><span data-stu-id="614aa-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="614aa-109">Авторизация</span><span class="sxs-lookup"><span data-stu-id="614aa-109">Authorization</span></span>  | <span data-ttu-id="614aa-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="614aa-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="614aa-112">Content-Type</span><span class="sxs-lookup"><span data-stu-id="614aa-112">Content-Type</span></span>  | <span data-ttu-id="614aa-113">application/json</span><span class="sxs-lookup"><span data-stu-id="614aa-113">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="614aa-114">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="614aa-114">Request body</span></span>
<span data-ttu-id="614aa-115">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="614aa-115">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="614aa-116">Отклик</span><span class="sxs-lookup"><span data-stu-id="614aa-116">Response</span></span>

<span data-ttu-id="614aa-117">В случае успеха этот метод возвращает код отклика `201, Created` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="614aa-117">If successful, this method returns `201, Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="614aa-118">Пример</span><span class="sxs-lookup"><span data-stu-id="614aa-118">Example</span></span>
##### <a name="request"></a><span data-ttu-id="614aa-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="614aa-119">Request</span></span>
<span data-ttu-id="614aa-120">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="614aa-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars
Content-type: application/json

{
  "name": "Volunteer"
}
```
<span data-ttu-id="614aa-121">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="614aa-121">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="614aa-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="614aa-122">Response</span></span>
<span data-ttu-id="614aa-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="614aa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Volunteer",
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
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
