# <a name="create-tablecolumn"></a><span data-ttu-id="26451-101">Создание объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="26451-101">Create TableColumn</span></span>

<span data-ttu-id="26451-102">С помощью этого API можно создать объект TableColumn.</span><span class="sxs-lookup"><span data-stu-id="26451-102">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="26451-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26451-103">Permissions</span></span>
<span data-ttu-id="26451-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="26451-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="26451-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26451-106">Permission type</span></span>      | <span data-ttu-id="26451-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26451-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26451-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26451-108">Delegated (work or school account)</span></span> | <span data-ttu-id="26451-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26451-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="26451-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26451-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26451-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26451-111">Not supported.</span></span>    |
|<span data-ttu-id="26451-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26451-112">Application</span></span> | <span data-ttu-id="26451-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26451-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="26451-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26451-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="26451-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26451-115">Request headers</span></span>
| <span data-ttu-id="26451-116">Имя</span><span class="sxs-lookup"><span data-stu-id="26451-116">Name</span></span>       | <span data-ttu-id="26451-117">Описание</span><span class="sxs-lookup"><span data-stu-id="26451-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="26451-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26451-118">Authorization</span></span>  | <span data-ttu-id="26451-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26451-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="26451-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="26451-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="26451-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="26451-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="26451-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26451-124">Request body</span></span>
<span data-ttu-id="26451-125">В тексте запроса укажите представление JSON объекта [WorkbookTableColumn](../resources/tablecolumn.md).</span><span class="sxs-lookup"><span data-stu-id="26451-125">In the request body, supply a JSON representation of [directoryObject](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="26451-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="26451-126">Response</span></span>

<span data-ttu-id="26451-127">В случае успеха, этот метод возвращает `201 Created`код ответа и обновленный объект [WorkbookTableColumn](../resources/tablecolumn.md)в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="26451-127">If successful, this method returns `201 Created` response code and [groupSetting](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26451-128">Пример</span><span class="sxs-lookup"><span data-stu-id="26451-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26451-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="26451-129">Request</span></span>
<span data-ttu-id="26451-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26451-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="26451-131">В тексте запроса укажите представление JSON объекта [WorkbookTableColumn](../resources/tablecolumn.md).</span><span class="sxs-lookup"><span data-stu-id="26451-131">In the request body, supply a JSON representation of [plannerPlan](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="26451-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="26451-132">Response</span></span>
<span data-ttu-id="26451-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26451-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->