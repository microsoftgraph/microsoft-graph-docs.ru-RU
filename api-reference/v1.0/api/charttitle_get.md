# <a name="get-charttitle"></a><span data-ttu-id="e4a9a-101">Получение объекта ChartTitle</span><span class="sxs-lookup"><span data-stu-id="e4a9a-101">Get ChartTitle</span></span>

<span data-ttu-id="e4a9a-102">Получение свойств и связей объекта charttitle.</span><span class="sxs-lookup"><span data-stu-id="e4a9a-102">Retrieve the properties and relationships of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e4a9a-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4a9a-103">Permissions</span></span>
<span data-ttu-id="e4a9a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e4a9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e4a9a-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4a9a-106">Permission type</span></span>      | <span data-ttu-id="e4a9a-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4a9a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4a9a-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4a9a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e4a9a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4a9a-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e4a9a-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4a9a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4a9a-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4a9a-111">Not supported.</span></span>    |
|<span data-ttu-id="e4a9a-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4a9a-112">Application</span></span> | <span data-ttu-id="e4a9a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4a9a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4a9a-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4a9a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e4a9a-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e4a9a-115">Optional query parameters</span></span>
<span data-ttu-id="e4a9a-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e4a9a-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4a9a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4a9a-117">Request headers</span></span>
| <span data-ttu-id="e4a9a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e4a9a-118">Name</span></span>      |<span data-ttu-id="e4a9a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e4a9a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e4a9a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4a9a-120">Authorization</span></span>  | <span data-ttu-id="e4a9a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4a9a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e4a9a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e4a9a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e4a9a-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e4a9a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4a9a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4a9a-126">Request body</span></span>
<span data-ttu-id="e4a9a-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4a9a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4a9a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4a9a-128">Response</span></span>

<span data-ttu-id="e4a9a-129">В случае успеха этот метод возвращает код отклика  и объект WorkbookChartTitle в тексте отклика.`200 OK` [ ](../resources/charttitle.md)</span><span class="sxs-lookup"><span data-stu-id="e4a9a-129">If successful, this method returns a `200 OK` response code and a [termsAndConditionsAssignment](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e4a9a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e4a9a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4a9a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4a9a-131">Request</span></span>
<span data-ttu-id="e4a9a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4a9a-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_charttitle"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
```
##### <a name="response"></a><span data-ttu-id="e4a9a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4a9a-133">Response</span></span>
<span data-ttu-id="e4a9a-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4a9a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartTitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->