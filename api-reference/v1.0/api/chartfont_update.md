# <a name="update-chartfont"></a><span data-ttu-id="3a48e-101">Обновление объекта ChartFont</span><span class="sxs-lookup"><span data-stu-id="3a48e-101">Update chartfont</span></span>

<span data-ttu-id="3a48e-102">Обновление свойств объекта chartfont.</span><span class="sxs-lookup"><span data-stu-id="3a48e-102">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a48e-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a48e-103">Permissions</span></span>
<span data-ttu-id="3a48e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3a48e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3a48e-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a48e-106">Permission type</span></span>      | <span data-ttu-id="3a48e-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a48e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a48e-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a48e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3a48e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a48e-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3a48e-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a48e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a48e-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a48e-111">Not supported.</span></span>    |
|<span data-ttu-id="3a48e-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a48e-112">Application</span></span> | <span data-ttu-id="3a48e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a48e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a48e-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a48e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="3a48e-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a48e-115">Optional request headers</span></span>
| <span data-ttu-id="3a48e-116">Имя</span><span class="sxs-lookup"><span data-stu-id="3a48e-116">Name</span></span>       | <span data-ttu-id="3a48e-117">Описание</span><span class="sxs-lookup"><span data-stu-id="3a48e-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3a48e-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a48e-118">Authorization</span></span>  | <span data-ttu-id="3a48e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a48e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a48e-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a48e-121">Request body</span></span>
<span data-ttu-id="3a48e-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3a48e-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3a48e-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a48e-125">Property</span></span>     | <span data-ttu-id="3a48e-126">Тип</span><span class="sxs-lookup"><span data-stu-id="3a48e-126">Type</span></span>   |<span data-ttu-id="3a48e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="3a48e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a48e-128">bold</span><span class="sxs-lookup"><span data-stu-id="3a48e-128">bold</span></span>|<span data-ttu-id="3a48e-129">boolean</span><span class="sxs-lookup"><span data-stu-id="3a48e-129">boolean</span></span>|<span data-ttu-id="3a48e-130">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="3a48e-130">Represents the bold status of font.</span></span>|
|<span data-ttu-id="3a48e-131">color</span><span class="sxs-lookup"><span data-stu-id="3a48e-131">color</span></span>|<span data-ttu-id="3a48e-132">string</span><span class="sxs-lookup"><span data-stu-id="3a48e-132">string</span></span>|<span data-ttu-id="3a48e-p104">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="3a48e-p104">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="3a48e-136">italic</span><span class="sxs-lookup"><span data-stu-id="3a48e-136">italic</span></span>|<span data-ttu-id="3a48e-137">boolean</span><span class="sxs-lookup"><span data-stu-id="3a48e-137">boolean</span></span>|<span data-ttu-id="3a48e-138">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="3a48e-138">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="3a48e-139">name</span><span class="sxs-lookup"><span data-stu-id="3a48e-139">name</span></span>|<span data-ttu-id="3a48e-140">string</span><span class="sxs-lookup"><span data-stu-id="3a48e-140">string</span></span>|<span data-ttu-id="3a48e-141">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="3a48e-141">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="3a48e-142">size</span><span class="sxs-lookup"><span data-stu-id="3a48e-142">size</span></span>|<span data-ttu-id="3a48e-143">Double</span><span class="sxs-lookup"><span data-stu-id="3a48e-143">double</span></span>|<span data-ttu-id="3a48e-144">Размер шрифта (например, 11)</span><span class="sxs-lookup"><span data-stu-id="3a48e-144">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="3a48e-145">underline</span><span class="sxs-lookup"><span data-stu-id="3a48e-145">underline</span></span>|<span data-ttu-id="3a48e-146">string</span><span class="sxs-lookup"><span data-stu-id="3a48e-146">string</span></span>|<span data-ttu-id="3a48e-p105">Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="3a48e-p105">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="3a48e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a48e-149">Response</span></span>

<span data-ttu-id="3a48e-150">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [ChartFont](../resources/chartfont.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3a48e-150">If successful, this method returns a `200 OK` response code and updated [ChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a48e-151">Пример</span><span class="sxs-lookup"><span data-stu-id="3a48e-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a48e-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a48e-152">Request</span></span>
<span data-ttu-id="3a48e-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a48e-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartfont"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```
##### <a name="response"></a><span data-ttu-id="3a48e-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a48e-154">Response</span></span>
<span data-ttu-id="3a48e-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3a48e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartfont",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->