# <a name="range-row"></a><span data-ttu-id="78f28-101">Range: Row</span><span class="sxs-lookup"><span data-stu-id="78f28-101">Range: Row</span></span>

<span data-ttu-id="78f28-102">Возвращает строку из диапазона.</span><span class="sxs-lookup"><span data-stu-id="78f28-102">Gets a row contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="78f28-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="78f28-103">Permissions</span></span>
<span data-ttu-id="78f28-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="78f28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="78f28-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78f28-106">Permission type</span></span>      | <span data-ttu-id="78f28-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="78f28-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78f28-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78f28-108">Delegated (work or school account)</span></span> | <span data-ttu-id="78f28-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78f28-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="78f28-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78f28-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78f28-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78f28-111">Not supported.</span></span>    |
|<span data-ttu-id="78f28-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="78f28-112">Application</span></span> | <span data-ttu-id="78f28-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78f28-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="78f28-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78f28-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/Row
POST /workbook/worksheets/{id|name}/range(<address>)/Row
POST /workbook/tables/{id|name}/columns/{id|name}/range/Row

```
## <a name="request-headers"></a><span data-ttu-id="78f28-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78f28-115">Request headers</span></span>
| <span data-ttu-id="78f28-116">Имя</span><span class="sxs-lookup"><span data-stu-id="78f28-116">Name</span></span>       | <span data-ttu-id="78f28-117">Описание</span><span class="sxs-lookup"><span data-stu-id="78f28-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="78f28-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="78f28-118">Authorization</span></span>  | <span data-ttu-id="78f28-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78f28-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78f28-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="78f28-121">Request body</span></span>
<span data-ttu-id="78f28-122">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="78f28-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="78f28-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="78f28-123">Parameter</span></span>    | <span data-ttu-id="78f28-124">Тип</span><span class="sxs-lookup"><span data-stu-id="78f28-124">Type</span></span>   |<span data-ttu-id="78f28-125">Описание</span><span class="sxs-lookup"><span data-stu-id="78f28-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78f28-126">row</span><span class="sxs-lookup"><span data-stu-id="78f28-126">row</span></span>|<span data-ttu-id="78f28-127">number</span><span class="sxs-lookup"><span data-stu-id="78f28-127">number</span></span>|<span data-ttu-id="78f28-p103">Номер строки диапазона, который требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="78f28-p103">Row number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="78f28-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="78f28-130">Response</span></span>

<span data-ttu-id="78f28-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="78f28-131">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78f28-132">Пример</span><span class="sxs-lookup"><span data-stu-id="78f28-132">Example</span></span>
<span data-ttu-id="78f28-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="78f28-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="78f28-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="78f28-134">Request</span></span>
<span data-ttu-id="78f28-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78f28-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_row"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/Row
Content-type: application/json
Content-length: 18

{
  "row": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="78f28-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="78f28-136">Response</span></span>
<span data-ttu-id="78f28-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="78f28-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Row",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->