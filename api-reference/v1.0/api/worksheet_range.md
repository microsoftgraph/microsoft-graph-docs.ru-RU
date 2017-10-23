# <a name="worksheet-range"></a><span data-ttu-id="0c78b-101">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="0c78b-101">Worksheet: Range</span></span>

<span data-ttu-id="0c78b-102">Возвращает объект диапазона, указанный по адресу или имени.</span><span class="sxs-lookup"><span data-stu-id="0c78b-102">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="0c78b-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c78b-103">Permissions</span></span>
<span data-ttu-id="0c78b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0c78b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0c78b-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c78b-106">Permission type</span></span>      | <span data-ttu-id="0c78b-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c78b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c78b-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c78b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0c78b-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c78b-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0c78b-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c78b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c78b-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c78b-111">Not supported.</span></span>    |
|<span data-ttu-id="0c78b-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c78b-112">Application</span></span> | <span data-ttu-id="0c78b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c78b-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c78b-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c78b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="0c78b-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c78b-115">Request headers</span></span>
| <span data-ttu-id="0c78b-116">Имя</span><span class="sxs-lookup"><span data-stu-id="0c78b-116">Name</span></span>       | <span data-ttu-id="0c78b-117">Описание</span><span class="sxs-lookup"><span data-stu-id="0c78b-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0c78b-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c78b-118">Authorization</span></span>  | <span data-ttu-id="0c78b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c78b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c78b-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c78b-121">Request body</span></span>
<span data-ttu-id="0c78b-122">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0c78b-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0c78b-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="0c78b-123">Parameter</span></span>    | <span data-ttu-id="0c78b-124">Тип</span><span class="sxs-lookup"><span data-stu-id="0c78b-124">Type</span></span>   |<span data-ttu-id="0c78b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="0c78b-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c78b-126">address</span><span class="sxs-lookup"><span data-stu-id="0c78b-126">address</span></span>|<span data-ttu-id="0c78b-127">string</span><span class="sxs-lookup"><span data-stu-id="0c78b-127">string</span></span>|<span data-ttu-id="0c78b-p103">Необязательный параметр. Адрес или имя диапазона. Если аргумент не указан, возвращается весь диапазон листа.</span><span class="sxs-lookup"><span data-stu-id="0c78b-p103">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="0c78b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c78b-131">Response</span></span>

<span data-ttu-id="0c78b-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0c78b-132">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c78b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0c78b-133">Example</span></span>
<span data-ttu-id="0c78b-134">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0c78b-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0c78b-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c78b-135">Request</span></span>
<span data-ttu-id="0c78b-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c78b-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/Range
Content-type: application/json
Content-length: 32

{
  "address": "address-value"
}
```

##### <a name="response"></a><span data-ttu-id="0c78b-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c78b-137">Response</span></span>
<span data-ttu-id="0c78b-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0c78b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->