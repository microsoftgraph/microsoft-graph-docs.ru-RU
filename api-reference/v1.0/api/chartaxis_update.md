# <a name="update-chartaxis"></a><span data-ttu-id="9f5b3-101">Обновление объекта chartAxis</span><span class="sxs-lookup"><span data-stu-id="9f5b3-101">Update chartaxis</span></span>

<span data-ttu-id="9f5b3-102">Обновление свойств объекта chartaxis.</span><span class="sxs-lookup"><span data-stu-id="9f5b3-102">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9f5b3-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f5b3-103">Permissions</span></span>
<span data-ttu-id="9f5b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9f5b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9f5b3-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f5b3-106">Permission type</span></span>      | <span data-ttu-id="9f5b3-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f5b3-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f5b3-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f5b3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9f5b3-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f5b3-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9f5b3-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f5b3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f5b3-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f5b3-111">Not supported.</span></span>    |
|<span data-ttu-id="9f5b3-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f5b3-112">Application</span></span> | <span data-ttu-id="9f5b3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f5b3-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f5b3-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f5b3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="9f5b3-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f5b3-115">Optional request headers</span></span>
| <span data-ttu-id="9f5b3-116">Имя</span><span class="sxs-lookup"><span data-stu-id="9f5b3-116">Name</span></span>       | <span data-ttu-id="9f5b3-117">Описание</span><span class="sxs-lookup"><span data-stu-id="9f5b3-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9f5b3-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f5b3-118">Authorization</span></span>  | <span data-ttu-id="9f5b3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f5b3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f5b3-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f5b3-121">Request body</span></span>
<span data-ttu-id="9f5b3-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9f5b3-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9f5b3-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f5b3-125">Property</span></span>     | <span data-ttu-id="9f5b3-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9f5b3-126">Type</span></span>   |<span data-ttu-id="9f5b3-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9f5b3-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f5b3-128">majorUnit</span><span class="sxs-lookup"><span data-stu-id="9f5b3-128">majorUnit</span></span>|<span data-ttu-id="9f5b3-129">object</span><span class="sxs-lookup"><span data-stu-id="9f5b3-129">object</span></span>|<span data-ttu-id="9f5b3-p104">Обозначает интервал между двумя основными делениями. Можно указать в виде числового значения или пустой строки.  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="9f5b3-p104">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="9f5b3-133">maximum</span><span class="sxs-lookup"><span data-stu-id="9f5b3-133">maximum</span></span>|<span data-ttu-id="9f5b3-134">object</span><span class="sxs-lookup"><span data-stu-id="9f5b3-134">object</span></span>|<span data-ttu-id="9f5b3-p105">Представляет максимальное значение на оси значений.  Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси).  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="9f5b3-p105">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="9f5b3-138">minimum</span><span class="sxs-lookup"><span data-stu-id="9f5b3-138">minimum</span></span>|<span data-ttu-id="9f5b3-139">object</span><span class="sxs-lookup"><span data-stu-id="9f5b3-139">object</span></span>|<span data-ttu-id="9f5b3-p106">Представляет минимальное значение на оси значений. Ему можно присвоить числовое значение или пустую строку (для автоматически заданных значений оси). Всегда возвращает числовое значение.</span><span class="sxs-lookup"><span data-stu-id="9f5b3-p106">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="9f5b3-143">minorUnit</span><span class="sxs-lookup"><span data-stu-id="9f5b3-143">minorUnit</span></span>|<span data-ttu-id="9f5b3-144">object</span><span class="sxs-lookup"><span data-stu-id="9f5b3-144">object</span></span>|<span data-ttu-id="9f5b3-p107">Представляет интервал между двумя промежуточными делениями. Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси). Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="9f5b3-p107">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="9f5b3-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f5b3-148">Response</span></span>

<span data-ttu-id="9f5b3-149">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [ChartAxis](../resources/chartaxis.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f5b3-149">If successful, this method returns a `200 OK` response code and updated [ChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9f5b3-150">Пример</span><span class="sxs-lookup"><span data-stu-id="9f5b3-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f5b3-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f5b3-151">Request</span></span>
<span data-ttu-id="9f5b3-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f5b3-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxis"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```
##### <a name="response"></a><span data-ttu-id="9f5b3-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f5b3-153">Response</span></span>
<span data-ttu-id="9f5b3-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9f5b3-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartaxis"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxis",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->