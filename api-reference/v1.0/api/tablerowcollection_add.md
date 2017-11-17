# <a name="tablerowcollection-add"></a><span data-ttu-id="66dae-101">TableRowCollection: add</span><span class="sxs-lookup"><span data-stu-id="66dae-101">TableRowCollection: add</span></span>

<span data-ttu-id="66dae-102">Добавляет новую строку в таблицу.</span><span class="sxs-lookup"><span data-stu-id="66dae-102">Adds a new row to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="66dae-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66dae-103">Permissions</span></span>
<span data-ttu-id="66dae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="66dae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="66dae-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66dae-106">Permission type</span></span>      | <span data-ttu-id="66dae-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66dae-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66dae-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66dae-108">Delegated (work or school account)</span></span> | <span data-ttu-id="66dae-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66dae-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="66dae-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66dae-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66dae-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66dae-111">Not supported.</span></span>    |
|<span data-ttu-id="66dae-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66dae-112">Application</span></span> | <span data-ttu-id="66dae-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66dae-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66dae-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66dae-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="66dae-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66dae-115">Request headers</span></span>
| <span data-ttu-id="66dae-116">Имя</span><span class="sxs-lookup"><span data-stu-id="66dae-116">Name</span></span>       | <span data-ttu-id="66dae-117">Описание</span><span class="sxs-lookup"><span data-stu-id="66dae-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="66dae-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66dae-118">Authorization</span></span>  | <span data-ttu-id="66dae-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66dae-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66dae-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66dae-121">Request body</span></span>
<span data-ttu-id="66dae-122">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="66dae-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="66dae-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="66dae-123">Parameter</span></span>    | <span data-ttu-id="66dae-124">Тип</span><span class="sxs-lookup"><span data-stu-id="66dae-124">Type</span></span>   |<span data-ttu-id="66dae-125">Описание</span><span class="sxs-lookup"><span data-stu-id="66dae-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66dae-126">index</span><span class="sxs-lookup"><span data-stu-id="66dae-126">index</span></span>|<span data-ttu-id="66dae-127">number</span><span class="sxs-lookup"><span data-stu-id="66dae-127">number</span></span>|<span data-ttu-id="66dae-p103">Необязательный параметр. Определяет относительную позицию новой строки. Если параметру присвоено значение null, строка добавляется в конце. Все строки ниже вставляемой строки сдвигаются вниз. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="66dae-p103">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="66dae-133">values</span><span class="sxs-lookup"><span data-stu-id="66dae-133">values</span></span>|<span data-ttu-id="66dae-134">(boolean, string или number)</span><span class="sxs-lookup"><span data-stu-id="66dae-134">(boolean or string or number)</span></span>|<span data-ttu-id="66dae-p104">Необязательный параметр. Двухмерный массив неформатированных значений строки таблицы.</span><span class="sxs-lookup"><span data-stu-id="66dae-p104">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="66dae-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="66dae-137">Response</span></span>

<span data-ttu-id="66dae-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект [TableRow](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="66dae-138">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66dae-139">Пример</span><span class="sxs-lookup"><span data-stu-id="66dae-139">Example</span></span>
<span data-ttu-id="66dae-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="66dae-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="66dae-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="66dae-141">Request</span></span>
<span data-ttu-id="66dae-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66dae-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": null,
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```

##### <a name="response"></a><span data-ttu-id="66dae-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="66dae-143">Response</span></span>
<span data-ttu-id="66dae-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="66dae-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
