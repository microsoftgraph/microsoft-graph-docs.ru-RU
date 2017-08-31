# <a name="chart-setdata"></a><span data-ttu-id="f01b0-101">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="f01b0-101">Chart: setData</span></span>

<span data-ttu-id="f01b0-102">Сбрасывает исходные данные для диаграммы.</span><span class="sxs-lookup"><span data-stu-id="f01b0-102">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="f01b0-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f01b0-103">Permissions</span></span>
<span data-ttu-id="f01b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f01b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f01b0-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f01b0-106">Permission type</span></span>      | <span data-ttu-id="f01b0-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f01b0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f01b0-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f01b0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f01b0-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f01b0-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f01b0-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f01b0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f01b0-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f01b0-111">Not supported.</span></span>    |
|<span data-ttu-id="f01b0-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f01b0-112">Application</span></span> | <span data-ttu-id="f01b0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f01b0-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f01b0-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f01b0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setData

```
## <a name="request-headers"></a><span data-ttu-id="f01b0-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f01b0-115">Request headers</span></span>
| <span data-ttu-id="f01b0-116">Имя</span><span class="sxs-lookup"><span data-stu-id="f01b0-116">Name</span></span>       | <span data-ttu-id="f01b0-117">Описание</span><span class="sxs-lookup"><span data-stu-id="f01b0-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f01b0-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f01b0-118">Authorization</span></span>  | <span data-ttu-id="f01b0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f01b0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f01b0-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f01b0-121">Request body</span></span>
<span data-ttu-id="f01b0-122">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f01b0-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f01b0-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="f01b0-123">Parameter</span></span>    | <span data-ttu-id="f01b0-124">Тип</span><span class="sxs-lookup"><span data-stu-id="f01b0-124">Type</span></span>   |<span data-ttu-id="f01b0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f01b0-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f01b0-126">sourceData</span><span class="sxs-lookup"><span data-stu-id="f01b0-126">sourceData</span></span>|<span data-ttu-id="f01b0-127">string</span><span class="sxs-lookup"><span data-stu-id="f01b0-127">string</span></span>|<span data-ttu-id="f01b0-128">Объект Range, соответствующий исходным данным.</span><span class="sxs-lookup"><span data-stu-id="f01b0-128">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="f01b0-129">seriesBy</span><span class="sxs-lookup"><span data-stu-id="f01b0-129">seriesBy</span></span>|<span data-ttu-id="f01b0-130">string</span><span class="sxs-lookup"><span data-stu-id="f01b0-130">string</span></span>|<span data-ttu-id="f01b0-p103">Необязательный параметр. Определяет способ использования столбцов или строк в качестве рядов данных на диаграмме. Может иметь одно из следующих значений: Auto (по умолчанию), Rows, Columns.  Возможные значения: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="f01b0-p103">Optional. Specifies the way columns or rows are used as data series on the chart. Can be one of the following: Auto (default), Rows, Columns.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="f01b0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f01b0-135">Response</span></span>

<span data-ttu-id="f01b0-p104">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f01b0-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f01b0-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f01b0-138">Example</span></span>
<span data-ttu-id="f01b0-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f01b0-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f01b0-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="f01b0-140">Request</span></span>
<span data-ttu-id="f01b0-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f01b0-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f01b0-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="f01b0-142">Response</span></span>
<span data-ttu-id="f01b0-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f01b0-143">Here is an example of the response.</span></span> 
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