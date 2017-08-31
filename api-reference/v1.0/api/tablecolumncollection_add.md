# <a name="tablecolumncollection-add"></a><span data-ttu-id="63303-101">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="63303-101">TableColumnCollection: add</span></span>

<span data-ttu-id="63303-102">Добавляет новый столбец в таблицу.</span><span class="sxs-lookup"><span data-stu-id="63303-102">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="63303-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63303-103">Permissions</span></span>
<span data-ttu-id="63303-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="63303-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="63303-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63303-106">Permission type</span></span>      | <span data-ttu-id="63303-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63303-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63303-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63303-108">Delegated (work or school account)</span></span> | <span data-ttu-id="63303-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63303-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="63303-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63303-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63303-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63303-111">Not supported.</span></span>    |
|<span data-ttu-id="63303-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63303-112">Application</span></span> | <span data-ttu-id="63303-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63303-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63303-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63303-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="63303-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63303-115">Request headers</span></span>
| <span data-ttu-id="63303-116">Имя</span><span class="sxs-lookup"><span data-stu-id="63303-116">Name</span></span>       | <span data-ttu-id="63303-117">Описание</span><span class="sxs-lookup"><span data-stu-id="63303-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="63303-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63303-118">Authorization</span></span>  | <span data-ttu-id="63303-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63303-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63303-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63303-121">Request body</span></span>
<span data-ttu-id="63303-122">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="63303-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="63303-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="63303-123">Parameter</span></span>    | <span data-ttu-id="63303-124">Тип</span><span class="sxs-lookup"><span data-stu-id="63303-124">Type</span></span>   |<span data-ttu-id="63303-125">Описание</span><span class="sxs-lookup"><span data-stu-id="63303-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63303-126">index</span><span class="sxs-lookup"><span data-stu-id="63303-126">index</span></span>|<span data-ttu-id="63303-127">number</span><span class="sxs-lookup"><span data-stu-id="63303-127">number</span></span>|<span data-ttu-id="63303-p103">Определяет относительную позицию нового столбца. Предыдущий столбец на этой позиции сдвигается вправо. Значение индекса должно быть равно или меньше значения индекса последнего столбца, чтобы его невозможно было использовать для добавления столбца в конце таблицы. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="63303-p103">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="63303-132">values</span><span class="sxs-lookup"><span data-stu-id="63303-132">values</span></span>|<span data-ttu-id="63303-133">(boolean, string или number)</span><span class="sxs-lookup"><span data-stu-id="63303-133">(boolean or string or number)</span></span>|<span data-ttu-id="63303-p104">Необязательный параметр. Двухмерный массив неформатированных значений столбца таблицы.</span><span class="sxs-lookup"><span data-stu-id="63303-p104">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="63303-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="63303-136">Response</span></span>

<span data-ttu-id="63303-137">В случае успеха этот метод возвращает код отклика `200, OK` и объект [TableColumn](../resources/tablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="63303-137">If successful, this method returns `200, OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63303-138">Пример</span><span class="sxs-lookup"><span data-stu-id="63303-138">Example</span></span>
<span data-ttu-id="63303-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="63303-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="63303-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="63303-140">Request</span></span>
<span data-ttu-id="63303-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63303-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="63303-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="63303-142">Response</span></span>
<span data-ttu-id="63303-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="63303-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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