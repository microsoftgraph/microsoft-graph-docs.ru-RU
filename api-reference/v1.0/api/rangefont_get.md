# <a name="get-rangefont"></a><span data-ttu-id="b1778-101">Получение объекта RangeFont</span><span class="sxs-lookup"><span data-stu-id="b1778-101">Get RangeFont</span></span>

<span data-ttu-id="b1778-102">Получение свойств и связей объекта rangefont.</span><span class="sxs-lookup"><span data-stu-id="b1778-102">Retrieve the properties and relationships of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b1778-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1778-103">Permissions</span></span>
<span data-ttu-id="b1778-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b1778-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b1778-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1778-106">Permission type</span></span>      | <span data-ttu-id="b1778-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1778-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1778-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1778-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b1778-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1778-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b1778-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1778-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1778-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1778-111">Not supported.</span></span>    |
|<span data-ttu-id="b1778-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1778-112">Application</span></span> | <span data-ttu-id="b1778-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1778-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1778-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1778-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/format/font
GET /workbook/worksheets/{id|name}/range(<address>)/format/font
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b1778-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b1778-115">Optional query parameters</span></span>
<span data-ttu-id="b1778-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b1778-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1778-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1778-117">Request headers</span></span>
| <span data-ttu-id="b1778-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b1778-118">Name</span></span>      |<span data-ttu-id="b1778-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b1778-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b1778-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1778-120">Authorization</span></span>  | <span data-ttu-id="b1778-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1778-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1778-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1778-123">Request body</span></span>
<span data-ttu-id="b1778-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b1778-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1778-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1778-125">Response</span></span>

<span data-ttu-id="b1778-126">В случае успеха этот метод возвращает код отклика `200 OK` и объект [RangeFont](../resources/rangefont.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1778-126">If successful, this method returns a `200 OK` response code and [RangeFont](../resources/rangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b1778-127">Пример</span><span class="sxs-lookup"><span data-stu-id="b1778-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1778-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1778-128">Request</span></span>
<span data-ttu-id="b1778-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1778-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rangefont"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/font
```
##### <a name="response"></a><span data-ttu-id="b1778-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1778-130">Response</span></span>
<span data-ttu-id="b1778-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b1778-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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
  "description": "Get RangeFont",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->