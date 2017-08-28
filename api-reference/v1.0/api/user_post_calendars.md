# <a name="create-calendar"></a><span data-ttu-id="066cf-101">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="066cf-101">Create Calendar</span></span>

<span data-ttu-id="066cf-102">С помощью этого API можно создать календарь.</span><span class="sxs-lookup"><span data-stu-id="066cf-102">Use this API to create a new calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="066cf-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="066cf-103">Permissions</span></span>
<span data-ttu-id="066cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="066cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="066cf-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="066cf-106">Permission type</span></span>      | <span data-ttu-id="066cf-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="066cf-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="066cf-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="066cf-108">Delegated (work or school account)</span></span> | <span data-ttu-id="066cf-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="066cf-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="066cf-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="066cf-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="066cf-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="066cf-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="066cf-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="066cf-112">Application</span></span> | <span data-ttu-id="066cf-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="066cf-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="066cf-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="066cf-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="066cf-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="066cf-115">Request headers</span></span>
| <span data-ttu-id="066cf-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="066cf-116">Header</span></span>       | <span data-ttu-id="066cf-117">Значение</span><span class="sxs-lookup"><span data-stu-id="066cf-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="066cf-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="066cf-118">Authorization</span></span>  | <span data-ttu-id="066cf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="066cf-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="066cf-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="066cf-121">Content-Type</span></span>  | <span data-ttu-id="066cf-122">application/json</span><span class="sxs-lookup"><span data-stu-id="066cf-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="066cf-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="066cf-123">Request body</span></span>
<span data-ttu-id="066cf-124">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="066cf-124">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="066cf-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="066cf-125">Response</span></span>

<span data-ttu-id="066cf-126">В случае успеха этот метод возвращает код отклика `201, Created` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="066cf-126">If successful, this method returns `201, Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="066cf-127">Пример</span><span class="sxs-lookup"><span data-stu-id="066cf-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="066cf-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="066cf-128">Request</span></span>
<span data-ttu-id="066cf-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="066cf-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="066cf-130">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="066cf-130">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="066cf-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="066cf-131">Response</span></span>
<span data-ttu-id="066cf-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="066cf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
