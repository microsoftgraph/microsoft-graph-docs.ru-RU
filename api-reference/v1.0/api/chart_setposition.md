# <a name="chart-setposition"></a><span data-ttu-id="73af8-101">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="73af8-101">Chart: setPosition</span></span>

<span data-ttu-id="73af8-102">Располагает диаграмму относительно ячеек на листе.</span><span class="sxs-lookup"><span data-stu-id="73af8-102">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="73af8-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73af8-103">Permissions</span></span>
<span data-ttu-id="73af8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="73af8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="73af8-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73af8-106">Permission type</span></span>      | <span data-ttu-id="73af8-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73af8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73af8-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73af8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="73af8-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73af8-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="73af8-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73af8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73af8-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73af8-111">Not supported.</span></span>    |
|<span data-ttu-id="73af8-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73af8-112">Application</span></span> | <span data-ttu-id="73af8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73af8-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="73af8-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73af8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="73af8-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73af8-115">Request headers</span></span>
| <span data-ttu-id="73af8-116">Имя</span><span class="sxs-lookup"><span data-stu-id="73af8-116">Name</span></span>       | <span data-ttu-id="73af8-117">Описание</span><span class="sxs-lookup"><span data-stu-id="73af8-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="73af8-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73af8-118">Authorization</span></span>  | <span data-ttu-id="73af8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73af8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73af8-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="73af8-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="73af8-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="73af8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73af8-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73af8-124">Request body</span></span>
<span data-ttu-id="73af8-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="73af8-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="73af8-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="73af8-126">Parameter</span></span>    | <span data-ttu-id="73af8-127">Тип</span><span class="sxs-lookup"><span data-stu-id="73af8-127">Type</span></span>   |<span data-ttu-id="73af8-128">Описание</span><span class="sxs-lookup"><span data-stu-id="73af8-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73af8-129">startCell</span><span class="sxs-lookup"><span data-stu-id="73af8-129">startCell</span></span>|<span data-ttu-id="73af8-130">string</span><span class="sxs-lookup"><span data-stu-id="73af8-130">string</span></span>|<span data-ttu-id="73af8-p104">Начальная ячейка. Место, куда будет перемещена диаграмма. Начальная ячейка — это верхняя левая или верхняя правая ячейка (это зависит от того, использует ли пользователь параметры отображения справа налево).</span><span class="sxs-lookup"><span data-stu-id="73af8-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="73af8-134">endCell</span><span class="sxs-lookup"><span data-stu-id="73af8-134">endCell</span></span>|<span data-ttu-id="73af8-135">string</span><span class="sxs-lookup"><span data-stu-id="73af8-135">string</span></span>|<span data-ttu-id="73af8-p105">Необязательный. Конечная ячейка. Если указан этот параметр, значения ширины и высоты диаграммы будут заданы так, чтобы полностью покрыть данную ячейку или диапазон.</span><span class="sxs-lookup"><span data-stu-id="73af8-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="73af8-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="73af8-139">Response</span></span>

<span data-ttu-id="73af8-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="73af8-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73af8-142">Пример</span><span class="sxs-lookup"><span data-stu-id="73af8-142">Example</span></span>
<span data-ttu-id="73af8-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="73af8-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="73af8-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="73af8-144">Request</span></span>
<span data-ttu-id="73af8-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73af8-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a><span data-ttu-id="73af8-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="73af8-146">Response</span></span>
<span data-ttu-id="73af8-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="73af8-147">Here is an example of the response.</span></span> 
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
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->