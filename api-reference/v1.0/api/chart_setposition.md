# <a name="chart-setposition"></a><span data-ttu-id="47d89-101">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="47d89-101">Chart: setPosition</span></span>

<span data-ttu-id="47d89-102">Располагает диаграмму относительно ячеек на листе.</span><span class="sxs-lookup"><span data-stu-id="47d89-102">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="47d89-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47d89-103">Permissions</span></span>
<span data-ttu-id="47d89-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="47d89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="47d89-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47d89-106">Permission type</span></span>      | <span data-ttu-id="47d89-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47d89-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47d89-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47d89-108">Delegated (work or school account)</span></span> | <span data-ttu-id="47d89-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47d89-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="47d89-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47d89-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47d89-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47d89-111">Not supported.</span></span>    |
|<span data-ttu-id="47d89-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47d89-112">Application</span></span> | <span data-ttu-id="47d89-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47d89-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="47d89-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47d89-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="47d89-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47d89-115">Request headers</span></span>
| <span data-ttu-id="47d89-116">Имя</span><span class="sxs-lookup"><span data-stu-id="47d89-116">Name</span></span>       | <span data-ttu-id="47d89-117">Описание</span><span class="sxs-lookup"><span data-stu-id="47d89-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="47d89-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47d89-118">Authorization</span></span>  | <span data-ttu-id="47d89-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47d89-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="47d89-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="47d89-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="47d89-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="47d89-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47d89-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47d89-124">Request body</span></span>
<span data-ttu-id="47d89-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="47d89-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="47d89-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="47d89-126">Parameter</span></span>    | <span data-ttu-id="47d89-127">Тип</span><span class="sxs-lookup"><span data-stu-id="47d89-127">Type</span></span>   |<span data-ttu-id="47d89-128">Описание</span><span class="sxs-lookup"><span data-stu-id="47d89-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47d89-129">startCell</span><span class="sxs-lookup"><span data-stu-id="47d89-129">startCell</span></span>|<span data-ttu-id="47d89-130">Json</span><span class="sxs-lookup"><span data-stu-id="47d89-130">Json</span></span>|<span data-ttu-id="47d89-p104">Начальная ячейка. Место, куда будет перемещена диаграмма. Начальная ячейка — это верхняя левая или верхняя правая ячейка (это зависит от того, использует ли пользователь параметры отображения справа налево).</span><span class="sxs-lookup"><span data-stu-id="47d89-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="47d89-134">endCell</span><span class="sxs-lookup"><span data-stu-id="47d89-134">endCell</span></span>|<span data-ttu-id="47d89-135">Json</span><span class="sxs-lookup"><span data-stu-id="47d89-135">Json</span></span>|<span data-ttu-id="47d89-p105">Необязательный. Конечная ячейка. Если указан этот параметр, значения ширины и высоты диаграммы будут заданы так, чтобы полностью покрыть данную ячейку или диапазон.</span><span class="sxs-lookup"><span data-stu-id="47d89-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="47d89-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="47d89-139">Response</span></span>

<span data-ttu-id="47d89-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="47d89-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47d89-142">Пример</span><span class="sxs-lookup"><span data-stu-id="47d89-142">Example</span></span>
<span data-ttu-id="47d89-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="47d89-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="47d89-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="47d89-144">Request</span></span>
<span data-ttu-id="47d89-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47d89-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a><span data-ttu-id="47d89-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="47d89-146">Response</span></span>
<span data-ttu-id="47d89-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="47d89-147">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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