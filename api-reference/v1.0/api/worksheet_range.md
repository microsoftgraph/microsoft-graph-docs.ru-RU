# <a name="worksheet-range"></a><span data-ttu-id="34389-101">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="34389-101">Worksheet: Range</span></span>

<span data-ttu-id="34389-102">Возвращает объект диапазона, указанный по адресу или имени.</span><span class="sxs-lookup"><span data-stu-id="34389-102">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="34389-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34389-103">Permissions</span></span>
<span data-ttu-id="34389-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="34389-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="34389-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34389-106">Permission type</span></span>      | <span data-ttu-id="34389-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34389-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34389-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34389-108">Delegated (work or school account)</span></span> | <span data-ttu-id="34389-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34389-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="34389-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34389-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34389-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34389-111">Not supported.</span></span>    |
|<span data-ttu-id="34389-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34389-112">Application</span></span> | <span data-ttu-id="34389-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34389-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34389-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34389-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="34389-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34389-115">Request headers</span></span>
| <span data-ttu-id="34389-116">Имя</span><span class="sxs-lookup"><span data-stu-id="34389-116">Name</span></span>       | <span data-ttu-id="34389-117">Описание</span><span class="sxs-lookup"><span data-stu-id="34389-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="34389-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34389-118">Authorization</span></span>  | <span data-ttu-id="34389-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34389-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34389-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="34389-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="34389-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="34389-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="34389-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34389-124">Request body</span></span>
<span data-ttu-id="34389-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="34389-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="34389-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="34389-126">Parameter</span></span>    | <span data-ttu-id="34389-127">Тип</span><span class="sxs-lookup"><span data-stu-id="34389-127">Type</span></span>   |<span data-ttu-id="34389-128">Описание</span><span class="sxs-lookup"><span data-stu-id="34389-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34389-129">address</span><span class="sxs-lookup"><span data-stu-id="34389-129">address</span></span>|<span data-ttu-id="34389-130">string</span><span class="sxs-lookup"><span data-stu-id="34389-130">string</span></span>|<span data-ttu-id="34389-p104">Необязательный параметр. Адрес или имя диапазона. Если аргумент не указан, возвращается весь диапазон листа.</span><span class="sxs-lookup"><span data-stu-id="34389-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="34389-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="34389-134">Response</span></span>

<span data-ttu-id="34389-135">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="34389-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34389-136">Пример</span><span class="sxs-lookup"><span data-stu-id="34389-136">Example</span></span>
<span data-ttu-id="34389-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="34389-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="34389-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="34389-138">Request</span></span>
<span data-ttu-id="34389-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34389-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="34389-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="34389-140">Response</span></span>
<span data-ttu-id="34389-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="34389-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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