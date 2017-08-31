# <a name="chart-setposition"></a><span data-ttu-id="88396-101">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="88396-101">Chart: setPosition</span></span>

<span data-ttu-id="88396-102">Располагает диаграмму относительно ячеек на листе.</span><span class="sxs-lookup"><span data-stu-id="88396-102">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="88396-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88396-103">Permissions</span></span>
<span data-ttu-id="88396-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="88396-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="88396-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88396-106">Permission type</span></span>      | <span data-ttu-id="88396-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88396-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88396-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88396-108">Delegated (work or school account)</span></span> | <span data-ttu-id="88396-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88396-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="88396-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88396-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88396-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88396-111">Not supported.</span></span>    |
|<span data-ttu-id="88396-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88396-112">Application</span></span> | <span data-ttu-id="88396-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88396-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="88396-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88396-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="88396-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88396-115">Request headers</span></span>
| <span data-ttu-id="88396-116">Имя</span><span class="sxs-lookup"><span data-stu-id="88396-116">Name</span></span>       | <span data-ttu-id="88396-117">Описание</span><span class="sxs-lookup"><span data-stu-id="88396-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="88396-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88396-118">Authorization</span></span>  | <span data-ttu-id="88396-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88396-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88396-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88396-121">Request body</span></span>
<span data-ttu-id="88396-122">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="88396-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="88396-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="88396-123">Parameter</span></span>    | <span data-ttu-id="88396-124">Тип</span><span class="sxs-lookup"><span data-stu-id="88396-124">Type</span></span>   |<span data-ttu-id="88396-125">Описание</span><span class="sxs-lookup"><span data-stu-id="88396-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88396-126">startCell</span><span class="sxs-lookup"><span data-stu-id="88396-126">startCell</span></span>|<span data-ttu-id="88396-127">string</span><span class="sxs-lookup"><span data-stu-id="88396-127">string</span></span>|<span data-ttu-id="88396-p103">Начальная ячейка. Место, куда будет перемещена диаграмма. Начальная ячейка — это верхняя левая или верхняя правая ячейка (это зависит от того, использует ли пользователь параметры отображения справа налево).</span><span class="sxs-lookup"><span data-stu-id="88396-p103">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="88396-131">endCell</span><span class="sxs-lookup"><span data-stu-id="88396-131">endCell</span></span>|<span data-ttu-id="88396-132">string</span><span class="sxs-lookup"><span data-stu-id="88396-132">string</span></span>|<span data-ttu-id="88396-p104">Необязательный. Конечная ячейка. Если указан этот параметр, значения ширины и высоты диаграммы будут заданы так, чтобы полностью покрыть данную ячейку или диапазон.</span><span class="sxs-lookup"><span data-stu-id="88396-p104">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="88396-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="88396-136">Response</span></span>

<span data-ttu-id="88396-p105">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="88396-p105">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88396-139">Пример</span><span class="sxs-lookup"><span data-stu-id="88396-139">Example</span></span>
<span data-ttu-id="88396-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="88396-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="88396-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="88396-141">Request</span></span>
<span data-ttu-id="88396-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88396-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="88396-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="88396-143">Response</span></span>
<span data-ttu-id="88396-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="88396-144">Here is an example of the response.</span></span> 
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