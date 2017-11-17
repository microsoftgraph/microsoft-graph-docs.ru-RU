# <a name="list-columns"></a><span data-ttu-id="aa340-101">Список столбцов</span><span class="sxs-lookup"><span data-stu-id="aa340-101">List columns</span></span>

<span data-ttu-id="aa340-102">Получение списка объектов tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="aa340-102">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="aa340-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa340-103">Permissions</span></span>
<span data-ttu-id="aa340-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aa340-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aa340-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa340-106">Permission type</span></span>      | <span data-ttu-id="aa340-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa340-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa340-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa340-108">Delegated (work or school account)</span></span> | <span data-ttu-id="aa340-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa340-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aa340-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa340-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa340-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa340-111">Not supported.</span></span>    |
|<span data-ttu-id="aa340-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa340-112">Application</span></span> | <span data-ttu-id="aa340-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa340-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa340-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa340-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aa340-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aa340-115">Optional query parameters</span></span>
<span data-ttu-id="aa340-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aa340-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa340-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa340-117">Request headers</span></span>
| <span data-ttu-id="aa340-118">Имя</span><span class="sxs-lookup"><span data-stu-id="aa340-118">Name</span></span>      |<span data-ttu-id="aa340-119">Описание</span><span class="sxs-lookup"><span data-stu-id="aa340-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aa340-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aa340-120">Authorization</span></span>  | <span data-ttu-id="aa340-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa340-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa340-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa340-123">Request body</span></span>
<span data-ttu-id="aa340-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa340-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa340-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa340-125">Response</span></span>

<span data-ttu-id="aa340-126">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [TableColumn](../resources/tablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aa340-126">If successful, this method returns a `200 OK` response code and collection of [TableColumn](../resources/tablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aa340-127">Пример</span><span class="sxs-lookup"><span data-stu-id="aa340-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa340-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa340-128">Request</span></span>
<span data-ttu-id="aa340-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa340-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_columns"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
```
##### <a name="response"></a><span data-ttu-id="aa340-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa340-130">Response</span></span>
<span data-ttu-id="aa340-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="aa340-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 126

{
  "value": [
    {
      "id": 99,
      "name": "name-value",
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

> <span data-ttu-id="aa340-134">**Примечание.** Используйте параметры запросов [$top](https://developer.microsoft.com/en-us/graph/docs/concepts/query_parameters#top) и [$skip](https://developer.microsoft.com/en-us/graph/docs/concepts/query_parameters#top), чтобы просматривать постранично большое количество столбцов.</span><span class="sxs-lookup"><span data-stu-id="aa340-134">**Note:** Use the [$top](https://developer.microsoft.com/en-us/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/en-us/graph/docs/concepts/query_parameters#top) query parameters to page through large numbers of columns.</span></span>

<span data-ttu-id="aa340-135">Пример.</span><span class="sxs-lookup"><span data-stu-id="aa340-135">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List columns",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->