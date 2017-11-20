# <a name="tablecolumncollection-add"></a><span data-ttu-id="56e27-101">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="56e27-101">TableColumnCollection: add</span></span>

<span data-ttu-id="56e27-102">Добавляет новый столбец в таблицу.</span><span class="sxs-lookup"><span data-stu-id="56e27-102">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="56e27-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56e27-103">Permissions</span></span>
<span data-ttu-id="56e27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="56e27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="56e27-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56e27-106">Permission type</span></span>      | <span data-ttu-id="56e27-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56e27-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56e27-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56e27-108">Delegated (work or school account)</span></span> | <span data-ttu-id="56e27-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56e27-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="56e27-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56e27-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56e27-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56e27-111">Not supported.</span></span>    |
|<span data-ttu-id="56e27-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56e27-112">Application</span></span> | <span data-ttu-id="56e27-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56e27-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="56e27-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56e27-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="56e27-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56e27-115">Request headers</span></span>
| <span data-ttu-id="56e27-116">Имя</span><span class="sxs-lookup"><span data-stu-id="56e27-116">Name</span></span>       | <span data-ttu-id="56e27-117">Описание</span><span class="sxs-lookup"><span data-stu-id="56e27-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="56e27-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56e27-118">Authorization</span></span>  | <span data-ttu-id="56e27-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56e27-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="56e27-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="56e27-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="56e27-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="56e27-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="56e27-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56e27-124">Request body</span></span>
<span data-ttu-id="56e27-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="56e27-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="56e27-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="56e27-126">Parameter</span></span>    | <span data-ttu-id="56e27-127">Тип</span><span class="sxs-lookup"><span data-stu-id="56e27-127">Type</span></span>   |<span data-ttu-id="56e27-128">Описание</span><span class="sxs-lookup"><span data-stu-id="56e27-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56e27-129">index</span><span class="sxs-lookup"><span data-stu-id="56e27-129">index</span></span>|<span data-ttu-id="56e27-130">number</span><span class="sxs-lookup"><span data-stu-id="56e27-130">number</span></span>|<span data-ttu-id="56e27-p104">Определяет относительную позицию нового столбца. Предыдущий столбец на этой позиции сдвигается вправо. Значение индекса должно быть равно или меньше значения индекса последнего столбца, чтобы его невозможно было использовать для добавления столбца в конце таблицы. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="56e27-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="56e27-135">values</span><span class="sxs-lookup"><span data-stu-id="56e27-135">values</span></span>|<span data-ttu-id="56e27-136">(boolean, string или number)</span><span class="sxs-lookup"><span data-stu-id="56e27-136">(boolean or string or number)</span></span>|<span data-ttu-id="56e27-p105">Необязательный параметр. Двухмерный массив неформатированных значений столбца таблицы.</span><span class="sxs-lookup"><span data-stu-id="56e27-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="56e27-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="56e27-139">Response</span></span>

<span data-ttu-id="56e27-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [TableColumn](../resources/tablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="56e27-140">If successful, this method returns `200 OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56e27-141">Пример</span><span class="sxs-lookup"><span data-stu-id="56e27-141">Example</span></span>
<span data-ttu-id="56e27-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="56e27-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="56e27-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="56e27-143">Request</span></span>
<span data-ttu-id="56e27-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56e27-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": {
  },
  "values": [
    {
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="56e27-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="56e27-145">Response</span></span>
<span data-ttu-id="56e27-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="56e27-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->