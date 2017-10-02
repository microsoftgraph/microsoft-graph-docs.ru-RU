# <a name="worksheet-usedrange"></a><span data-ttu-id="4b41c-101">Worksheet: UsedRange</span><span class="sxs-lookup"><span data-stu-id="4b41c-101">Worksheet: UsedRange</span></span>

<span data-ttu-id="4b41c-p101">Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.</span><span class="sxs-lookup"><span data-stu-id="4b41c-p101">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="4b41c-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b41c-104">Permissions</span></span>
<span data-ttu-id="4b41c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4b41c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4b41c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b41c-107">Permission type</span></span>      | <span data-ttu-id="4b41c-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b41c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b41c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b41c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="4b41c-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b41c-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4b41c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b41c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b41c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b41c-112">Not supported.</span></span>    |
|<span data-ttu-id="4b41c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b41c-113">Application</span></span> | <span data-ttu-id="4b41c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b41c-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b41c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b41c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/UsedRange

```

## <a name="optional-request-parameter"></a><span data-ttu-id="4b41c-116">Необязательный параметр запросов</span><span class="sxs-lookup"><span data-stu-id="4b41c-116">Optional request parameter</span></span>
<span data-ttu-id="4b41c-117">В URL-адресе запроса предоставьте необязательный параметр запросов.</span><span class="sxs-lookup"><span data-stu-id="4b41c-117">In the request URL, provide an optional query parameter.</span></span>

| <span data-ttu-id="4b41c-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="4b41c-118">Parameter</span></span>    | <span data-ttu-id="4b41c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="4b41c-119">Type</span></span>   |<span data-ttu-id="4b41c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4b41c-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b41c-121">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="4b41c-121">valuesOnly</span></span>|<span data-ttu-id="4b41c-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b41c-122">Boolean</span></span>|<span data-ttu-id="4b41c-p103">Необязательный параметр. Учитывает только ячейки со значениями (игнорирует форматирование).</span><span class="sxs-lookup"><span data-stu-id="4b41c-p103">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="4b41c-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b41c-125">Request headers</span></span>
| <span data-ttu-id="4b41c-126">Имя</span><span class="sxs-lookup"><span data-stu-id="4b41c-126">Name</span></span>       | <span data-ttu-id="4b41c-127">Описание</span><span class="sxs-lookup"><span data-stu-id="4b41c-127">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4b41c-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b41c-128">Authorization</span></span>  | <span data-ttu-id="4b41c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b41c-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4b41c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b41c-131">Response</span></span>

<span data-ttu-id="4b41c-132">В случае успеха этот метод возвращает код отклика `200, OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4b41c-132">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b41c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4b41c-133">Example</span></span>
<span data-ttu-id="4b41c-134">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4b41c-134">Here is an example that shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4b41c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b41c-135">Request</span></span>
<span data-ttu-id="4b41c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b41c-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange(valuesOnly=true)
Content-type: application/json

```

##### <a name="response"></a><span data-ttu-id="4b41c-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b41c-137">Response</span></span>
<span data-ttu-id="4b41c-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4b41c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "addressLocal": "addressLocal-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
