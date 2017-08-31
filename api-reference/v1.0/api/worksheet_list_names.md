# <a name="list-names"></a><span data-ttu-id="ee5d0-101">Перечисление имен</span><span class="sxs-lookup"><span data-stu-id="ee5d0-101">List names</span></span>

<span data-ttu-id="ee5d0-102">Получение списка именованных элементов, связанных с листом.</span><span class="sxs-lookup"><span data-stu-id="ee5d0-102">Retrieve a list of named item associated with the worksheet.</span></span> 
## <a name="permissions"></a><span data-ttu-id="ee5d0-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee5d0-103">Permissions</span></span>
<span data-ttu-id="ee5d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ee5d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ee5d0-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee5d0-106">Permission type</span></span>      | <span data-ttu-id="ee5d0-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee5d0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee5d0-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee5d0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ee5d0-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee5d0-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ee5d0-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee5d0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee5d0-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee5d0-111">Not supported.</span></span>    |
|<span data-ttu-id="ee5d0-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee5d0-112">Application</span></span> | <span data-ttu-id="ee5d0-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee5d0-113">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee5d0-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee5d0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets({id|name})/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ee5d0-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ee5d0-115">Optional query parameters</span></span>
<span data-ttu-id="ee5d0-116">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ee5d0-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee5d0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee5d0-117">Request headers</span></span>
| <span data-ttu-id="ee5d0-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ee5d0-118">Name</span></span>      |<span data-ttu-id="ee5d0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ee5d0-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ee5d0-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee5d0-120">Authorization</span></span>  | <span data-ttu-id="ee5d0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee5d0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee5d0-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee5d0-123">Request body</span></span>
<span data-ttu-id="ee5d0-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee5d0-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee5d0-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee5d0-125">Response</span></span>

<span data-ttu-id="ee5d0-126">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [NamedItem](../resources/nameditem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee5d0-126">If successful, this method returns a `200 OK` response code and collection of [NamedItem](../resources/nameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ee5d0-127">Пример</span><span class="sxs-lookup"><span data-stu-id="ee5d0-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee5d0-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee5d0-128">Request</span></span>
<span data-ttu-id="ee5d0-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee5d0-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tables"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/names
```
##### <a name="response"></a><span data-ttu-id="ee5d0-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee5d0-130">Response</span></span>
<span data-ttu-id="ee5d0-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ee5d0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "name": "myrange",
      "scope": "worksheet"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tables",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
