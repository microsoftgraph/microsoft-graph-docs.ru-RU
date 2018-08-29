# <a name="list-pivottables"></a><span data-ttu-id="1a348-101">Получение списка pivotTables</span><span class="sxs-lookup"><span data-stu-id="1a348-101">List pivotTables</span></span>

<span data-ttu-id="1a348-102">Получение списка объектов workbookpivottable.</span><span class="sxs-lookup"><span data-stu-id="1a348-102">Retrieve a list of workbookpivottable objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a348-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a348-103">Permissions</span></span>
<span data-ttu-id="1a348-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1a348-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="1a348-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a348-106">Permission type</span></span>      | <span data-ttu-id="1a348-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a348-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a348-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a348-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1a348-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a348-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1a348-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a348-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a348-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a348-111">Not supported.</span></span>    |
|<span data-ttu-id="1a348-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a348-112">Application</span></span> | <span data-ttu-id="1a348-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a348-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a348-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a348-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1a348-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1a348-115">Optional query parameters</span></span>
<span data-ttu-id="1a348-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1a348-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a348-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a348-117">Request headers</span></span>
| <span data-ttu-id="1a348-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1a348-118">Name</span></span>      |<span data-ttu-id="1a348-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1a348-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1a348-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a348-120">Authorization</span></span>  | <span data-ttu-id="1a348-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a348-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1a348-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1a348-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="1a348-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="1a348-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a348-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a348-126">Request body</span></span>
<span data-ttu-id="1a348-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1a348-127">Do not supply a request body for this method.</span></span>
### <a name="response"></a><span data-ttu-id="1a348-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a348-128">Response</span></span>
<span data-ttu-id="1a348-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [workbookPivotTable](../resources/workbookpivottable.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1a348-129">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/workbookpivottable.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1a348-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1a348-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a348-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a348-131">Request</span></span>
<span data-ttu-id="1a348-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a348-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_pivottables"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables
```
##### <a name="response"></a><span data-ttu-id="1a348-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="1a348-133">Response</span></span>
<span data-ttu-id="1a348-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a348-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookPivotTable",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 83

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value"
    }
  ]
}
```
