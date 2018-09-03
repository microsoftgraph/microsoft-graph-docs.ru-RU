# <a name="update-table"></a><span data-ttu-id="ca03f-101">Обновление таблицы</span><span class="sxs-lookup"><span data-stu-id="ca03f-101">Update table</span></span>

<span data-ttu-id="ca03f-102">Обновление свойств объекта таблицы.</span><span class="sxs-lookup"><span data-stu-id="ca03f-102">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ca03f-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca03f-103">Permissions</span></span>
<span data-ttu-id="ca03f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ca03f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ca03f-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca03f-106">Permission type</span></span>      | <span data-ttu-id="ca03f-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca03f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca03f-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca03f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ca03f-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca03f-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ca03f-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca03f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca03f-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca03f-111">Not supported.</span></span>    |
|<span data-ttu-id="ca03f-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca03f-112">Application</span></span> | <span data-ttu-id="ca03f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca03f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca03f-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca03f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="ca03f-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca03f-115">Optional request headers</span></span>
| <span data-ttu-id="ca03f-116">Имя</span><span class="sxs-lookup"><span data-stu-id="ca03f-116">Name</span></span>       | <span data-ttu-id="ca03f-117">Описание</span><span class="sxs-lookup"><span data-stu-id="ca03f-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ca03f-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca03f-118">Authorization</span></span>  | <span data-ttu-id="ca03f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca03f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ca03f-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ca03f-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="ca03f-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ca03f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca03f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca03f-124">Request body</span></span>
<span data-ttu-id="ca03f-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ca03f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ca03f-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca03f-128">Property</span></span>     | <span data-ttu-id="ca03f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ca03f-129">Type</span></span>   |<span data-ttu-id="ca03f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ca03f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca03f-131">name</span><span class="sxs-lookup"><span data-stu-id="ca03f-131">name</span></span>|<span data-ttu-id="ca03f-132">строка</span><span class="sxs-lookup"><span data-stu-id="ca03f-132">string</span></span>|<span data-ttu-id="ca03f-133">Имя таблицы.</span><span class="sxs-lookup"><span data-stu-id="ca03f-133">Name of the table.</span></span>|
|<span data-ttu-id="ca03f-134">showHeaders</span><span class="sxs-lookup"><span data-stu-id="ca03f-134">showHeaders</span></span>|<span data-ttu-id="ca03f-135">логический</span><span class="sxs-lookup"><span data-stu-id="ca03f-135">boolean</span></span>|<span data-ttu-id="ca03f-p105">Указывает, отображается ли строка заголовков. Можно задать это значение, чтобы отобразить или скрыть строку заголовков.</span><span class="sxs-lookup"><span data-stu-id="ca03f-p105">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="ca03f-138">showTotals</span><span class="sxs-lookup"><span data-stu-id="ca03f-138">showTotals</span></span>|<span data-ttu-id="ca03f-139">логический</span><span class="sxs-lookup"><span data-stu-id="ca03f-139">boolean</span></span>|<span data-ttu-id="ca03f-p106">Указывает, отображается ли строка итогов. Можно задать это значение, чтобы отобразить или скрыть строку итогов.</span><span class="sxs-lookup"><span data-stu-id="ca03f-p106">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="ca03f-142">style</span><span class="sxs-lookup"><span data-stu-id="ca03f-142">style</span></span>|<span data-ttu-id="ca03f-143">строка</span><span class="sxs-lookup"><span data-stu-id="ca03f-143">string</span></span>|<span data-ttu-id="ca03f-144">Постоянное значение, представляющее стиль таблицы.</span><span class="sxs-lookup"><span data-stu-id="ca03f-144">Constant value that represents the Table style.</span></span> <span data-ttu-id="ca03f-145">Возможные значения: от TableStyleLight1 до TableStyleLight21, от TableStyleMedium1 до TableStyleMedium28, от TableStyleStyleDark1 до TableStyleStyleDark11.</span><span class="sxs-lookup"><span data-stu-id="ca03f-145">The possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11.</span></span> <span data-ttu-id="ca03f-146">Также может быть определён настраиваемый пользователем стиль, имеющийся в книге.</span><span class="sxs-lookup"><span data-stu-id="ca03f-146">A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="ca03f-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="ca03f-147">Response</span></span>

<span data-ttu-id="ca03f-148">В случае успеха, этот метод возвращает`200 OK`код ответа и объект [WorkbookTable](../resources/table.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ca03f-148">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ca03f-149">Пример</span><span class="sxs-lookup"><span data-stu-id="ca03f-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca03f-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca03f-150">Request</span></span>
<span data-ttu-id="ca03f-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca03f-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_table"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}
Content-type: application/json
Content-length: 109

{
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
##### <a name="response"></a><span data-ttu-id="ca03f-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="ca03f-152">Response</span></span>
<span data-ttu-id="ca03f-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca03f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
