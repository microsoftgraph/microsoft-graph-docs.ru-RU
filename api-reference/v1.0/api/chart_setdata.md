# <a name="chart-setdata"></a><span data-ttu-id="c5e6a-101">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="c5e6a-101">Chart: setData</span></span>

<span data-ttu-id="c5e6a-102">Сбрасывает исходные данные для диаграммы.</span><span class="sxs-lookup"><span data-stu-id="c5e6a-102">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5e6a-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5e6a-103">Permissions</span></span>
<span data-ttu-id="c5e6a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5e6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c5e6a-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5e6a-106">Permission type</span></span>      | <span data-ttu-id="c5e6a-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5e6a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5e6a-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5e6a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c5e6a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5e6a-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c5e6a-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5e6a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5e6a-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5e6a-111">Not supported.</span></span>    |
|<span data-ttu-id="c5e6a-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5e6a-112">Application</span></span> | <span data-ttu-id="c5e6a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5e6a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5e6a-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5e6a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setData

```
## <a name="request-headers"></a><span data-ttu-id="c5e6a-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5e6a-115">Request headers</span></span>
| <span data-ttu-id="c5e6a-116">Имя</span><span class="sxs-lookup"><span data-stu-id="c5e6a-116">Name</span></span>       | <span data-ttu-id="c5e6a-117">Описание</span><span class="sxs-lookup"><span data-stu-id="c5e6a-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c5e6a-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5e6a-118">Authorization</span></span>  | <span data-ttu-id="c5e6a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5e6a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c5e6a-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c5e6a-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="c5e6a-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c5e6a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5e6a-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5e6a-124">Request body</span></span>
<span data-ttu-id="c5e6a-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c5e6a-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c5e6a-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="c5e6a-126">Parameter</span></span>    | <span data-ttu-id="c5e6a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c5e6a-127">Type</span></span>   |<span data-ttu-id="c5e6a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c5e6a-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5e6a-129">sourceData</span><span class="sxs-lookup"><span data-stu-id="c5e6a-129">sourceData</span></span>|<span data-ttu-id="c5e6a-130">string</span><span class="sxs-lookup"><span data-stu-id="c5e6a-130">string</span></span>|<span data-ttu-id="c5e6a-131">Объект Range, соответствующий исходным данным.</span><span class="sxs-lookup"><span data-stu-id="c5e6a-131">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="c5e6a-132">seriesBy</span><span class="sxs-lookup"><span data-stu-id="c5e6a-132">seriesBy</span></span>|<span data-ttu-id="c5e6a-133">string</span><span class="sxs-lookup"><span data-stu-id="c5e6a-133">string</span></span>|<span data-ttu-id="c5e6a-p104">Необязательный параметр. Определяет способ использования столбцов или строк в качестве рядов данных на диаграмме. Может иметь одно из следующих значений: Auto (по умолчанию), Rows, Columns.  Возможные значения: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="c5e6a-p104">Optional. Specifies the way columns or rows are used as data series on the chart. Can be one of the following: Auto (default), Rows, Columns.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="c5e6a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5e6a-138">Response</span></span>

<span data-ttu-id="c5e6a-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c5e6a-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5e6a-141">Пример</span><span class="sxs-lookup"><span data-stu-id="c5e6a-141">Example</span></span>
<span data-ttu-id="c5e6a-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c5e6a-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c5e6a-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5e6a-143">Request</span></span>
<span data-ttu-id="c5e6a-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5e6a-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="c5e6a-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5e6a-145">Response</span></span>
<span data-ttu-id="c5e6a-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c5e6a-146">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->