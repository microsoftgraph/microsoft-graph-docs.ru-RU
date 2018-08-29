# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="9ca29-101">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="9ca29-101">ChartFill: setSolidColor</span></span>

<span data-ttu-id="9ca29-102">Задает заливку одним цветом для элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="9ca29-102">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="9ca29-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ca29-103">Permissions</span></span>
<span data-ttu-id="9ca29-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9ca29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9ca29-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ca29-106">Permission type</span></span>      | <span data-ttu-id="9ca29-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ca29-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ca29-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ca29-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9ca29-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ca29-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9ca29-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ca29-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ca29-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ca29-111">Not supported.</span></span>    |
|<span data-ttu-id="9ca29-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ca29-112">Application</span></span> | <span data-ttu-id="9ca29-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ca29-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ca29-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ca29-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="9ca29-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ca29-115">Request headers</span></span>
| <span data-ttu-id="9ca29-116">Имя</span><span class="sxs-lookup"><span data-stu-id="9ca29-116">Name</span></span>       | <span data-ttu-id="9ca29-117">Описание</span><span class="sxs-lookup"><span data-stu-id="9ca29-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9ca29-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ca29-118">Authorization</span></span>  | <span data-ttu-id="9ca29-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ca29-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9ca29-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9ca29-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="9ca29-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9ca29-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ca29-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ca29-124">Request body</span></span>
<span data-ttu-id="9ca29-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9ca29-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9ca29-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="9ca29-126">Parameter</span></span>    | <span data-ttu-id="9ca29-127">Тип</span><span class="sxs-lookup"><span data-stu-id="9ca29-127">Type</span></span>   |<span data-ttu-id="9ca29-128">Описание</span><span class="sxs-lookup"><span data-stu-id="9ca29-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ca29-129">color</span><span class="sxs-lookup"><span data-stu-id="9ca29-129">color</span></span>|<span data-ttu-id="9ca29-130">строка</span><span class="sxs-lookup"><span data-stu-id="9ca29-130">string</span></span>|<span data-ttu-id="9ca29-131">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="9ca29-131">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="9ca29-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ca29-132">Response</span></span>

<span data-ttu-id="9ca29-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9ca29-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ca29-135">Пример</span><span class="sxs-lookup"><span data-stu-id="9ca29-135">Example</span></span>
<span data-ttu-id="9ca29-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9ca29-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9ca29-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ca29-137">Request</span></span>
<span data-ttu-id="9ca29-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ca29-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

##### <a name="response"></a><span data-ttu-id="9ca29-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ca29-139">Response</span></span>
<span data-ttu-id="9ca29-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9ca29-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->