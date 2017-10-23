# <a name="range-insert"></a><span data-ttu-id="a6fa4-101">Range: insert</span><span class="sxs-lookup"><span data-stu-id="a6fa4-101">Range: insert</span></span>

<span data-ttu-id="a6fa4-p101">Вставляет ячейку или диапазон ячеек на лист вместо этого диапазона, а также сдвигает другие ячейки, чтобы освободить место. Возвращает новый объект Range в пустом месте.</span><span class="sxs-lookup"><span data-stu-id="a6fa4-p101">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="a6fa4-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6fa4-104">Permissions</span></span>
<span data-ttu-id="a6fa4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a6fa4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a6fa4-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6fa4-107">Permission type</span></span>      | <span data-ttu-id="a6fa4-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6fa4-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6fa4-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6fa4-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a6fa4-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6fa4-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a6fa4-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6fa4-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6fa4-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6fa4-112">Not supported.</span></span>    |
|<span data-ttu-id="a6fa4-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6fa4-113">Application</span></span> | <span data-ttu-id="a6fa4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6fa4-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6fa4-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6fa4-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/insert
POST /workbook/worksheets/{id|name}/range(<address>)/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="a6fa4-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6fa4-116">Request headers</span></span>
| <span data-ttu-id="a6fa4-117">Имя</span><span class="sxs-lookup"><span data-stu-id="a6fa4-117">Name</span></span>       | <span data-ttu-id="a6fa4-118">Описание</span><span class="sxs-lookup"><span data-stu-id="a6fa4-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a6fa4-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6fa4-119">Authorization</span></span>  | <span data-ttu-id="a6fa4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6fa4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6fa4-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6fa4-122">Request body</span></span>
<span data-ttu-id="a6fa4-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a6fa4-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a6fa4-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="a6fa4-124">Parameter</span></span>    | <span data-ttu-id="a6fa4-125">Тип</span><span class="sxs-lookup"><span data-stu-id="a6fa4-125">Type</span></span>   |<span data-ttu-id="a6fa4-126">Описание</span><span class="sxs-lookup"><span data-stu-id="a6fa4-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6fa4-127">shift</span><span class="sxs-lookup"><span data-stu-id="a6fa4-127">shift</span></span>|<span data-ttu-id="a6fa4-128">string</span><span class="sxs-lookup"><span data-stu-id="a6fa4-128">string</span></span>|<span data-ttu-id="a6fa4-p104">Указывает направление сдвига ячеек.  Возможные значения: `Down`, `Right`.</span><span class="sxs-lookup"><span data-stu-id="a6fa4-p104">Specifies which way to shift the cells.  Possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="a6fa4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6fa4-131">Response</span></span>

<span data-ttu-id="a6fa4-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a6fa4-132">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6fa4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a6fa4-133">Example</span></span>
<span data-ttu-id="a6fa4-134">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a6fa4-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a6fa4-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6fa4-135">Request</span></span>
<span data-ttu-id="a6fa4-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6fa4-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="a6fa4-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6fa4-137">Response</span></span>
<span data-ttu-id="a6fa4-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a6fa4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->