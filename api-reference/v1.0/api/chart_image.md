# <a name="chart-image"></a><span data-ttu-id="596d8-101">Chart: Image</span><span class="sxs-lookup"><span data-stu-id="596d8-101">Chart: Image</span></span>

<span data-ttu-id="596d8-102">Отрисовывает диаграмму в виде изображения с кодировкой Base64, масштабируя ее в соответствии с указанным размером.</span><span class="sxs-lookup"><span data-stu-id="596d8-102">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="596d8-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="596d8-103">Permissions</span></span>
<span data-ttu-id="596d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="596d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="596d8-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="596d8-106">Permission type</span></span>      | <span data-ttu-id="596d8-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="596d8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="596d8-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="596d8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="596d8-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="596d8-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="596d8-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="596d8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="596d8-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="596d8-111">Not supported.</span></span>    |
|<span data-ttu-id="596d8-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="596d8-112">Application</span></span> | <span data-ttu-id="596d8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="596d8-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="596d8-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="596d8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="596d8-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="596d8-115">Request headers</span></span>
| <span data-ttu-id="596d8-116">Имя</span><span class="sxs-lookup"><span data-stu-id="596d8-116">Name</span></span>       | <span data-ttu-id="596d8-117">Описание</span><span class="sxs-lookup"><span data-stu-id="596d8-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="596d8-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="596d8-118">Authorization</span></span>  | <span data-ttu-id="596d8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="596d8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="596d8-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="596d8-121">Request body</span></span>
<span data-ttu-id="596d8-122">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="596d8-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="596d8-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="596d8-123">Parameter</span></span>    | <span data-ttu-id="596d8-124">Тип</span><span class="sxs-lookup"><span data-stu-id="596d8-124">Type</span></span>   |<span data-ttu-id="596d8-125">Описание</span><span class="sxs-lookup"><span data-stu-id="596d8-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="596d8-126">height</span><span class="sxs-lookup"><span data-stu-id="596d8-126">height</span></span>|<span data-ttu-id="596d8-127">number</span><span class="sxs-lookup"><span data-stu-id="596d8-127">number</span></span>|<span data-ttu-id="596d8-p103">Необязательный. Нужная высота создаваемого изображения.</span><span class="sxs-lookup"><span data-stu-id="596d8-p103">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="596d8-130">width</span><span class="sxs-lookup"><span data-stu-id="596d8-130">width</span></span>|<span data-ttu-id="596d8-131">number</span><span class="sxs-lookup"><span data-stu-id="596d8-131">number</span></span>|<span data-ttu-id="596d8-p104">Необязательный. Нужная ширина создаваемого изображения.</span><span class="sxs-lookup"><span data-stu-id="596d8-p104">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="596d8-134">fittingMode</span><span class="sxs-lookup"><span data-stu-id="596d8-134">fittingMode</span></span>|<span data-ttu-id="596d8-135">string</span><span class="sxs-lookup"><span data-stu-id="596d8-135">string</span></span>|<span data-ttu-id="596d8-p105">Необязательный. Метод, используемый для масштабирования диаграммы до указанного размера (если указаны и высота, и ширина).  Возможные значения: `Fit`, `FitAndCenter`, `Fill`.</span><span class="sxs-lookup"><span data-stu-id="596d8-p105">Optional. The method used to scale the chart to the specified to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="596d8-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="596d8-139">Response</span></span>

<span data-ttu-id="596d8-140">В случае успеха этот метод возвращает код отклика `200, OK` и строку изображения с кодировкой base-64 в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="596d8-140">If successful, this method returns `200, OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="596d8-141">Пример</span><span class="sxs-lookup"><span data-stu-id="596d8-141">Example</span></span>
<span data-ttu-id="596d8-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="596d8-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="596d8-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="596d8-143">Request</span></span>
<span data-ttu-id="596d8-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="596d8-144">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')
Content-type: application/json
Content-length: 77

{
  "height": {
  },
  "width": {
  },
  "fittingMode": "fittingMode-value"
}
```

##### <a name="response"></a><span data-ttu-id="596d8-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="596d8-145">Response</span></span>
<span data-ttu-id="596d8-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="596d8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: Image",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
