# <a name="table-headerrowrange"></a><span data-ttu-id="290c5-101">Table: HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="290c5-101">Table: HeaderRowRange</span></span>

<span data-ttu-id="290c5-102">Получает объект диапазона, связанный со строкой заголовков таблицы.</span><span class="sxs-lookup"><span data-stu-id="290c5-102">Gets the range object associated with header row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="290c5-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="290c5-103">Permissions</span></span>
<span data-ttu-id="290c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="290c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="290c5-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="290c5-106">Permission type</span></span>      | <span data-ttu-id="290c5-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="290c5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="290c5-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="290c5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="290c5-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="290c5-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="290c5-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="290c5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="290c5-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="290c5-111">Not supported.</span></span>    |
|<span data-ttu-id="290c5-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="290c5-112">Application</span></span> | <span data-ttu-id="290c5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="290c5-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="290c5-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="290c5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/HeaderRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/HeaderRowRange

```
## <a name="request-headers"></a><span data-ttu-id="290c5-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="290c5-115">Request headers</span></span>
| <span data-ttu-id="290c5-116">Имя</span><span class="sxs-lookup"><span data-stu-id="290c5-116">Name</span></span>       | <span data-ttu-id="290c5-117">Описание</span><span class="sxs-lookup"><span data-stu-id="290c5-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="290c5-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="290c5-118">Authorization</span></span>  | <span data-ttu-id="290c5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="290c5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="290c5-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="290c5-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="290c5-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="290c5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="290c5-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="290c5-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="290c5-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="290c5-125">Response</span></span>

<span data-ttu-id="290c5-126">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="290c5-126">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="290c5-127">Пример</span><span class="sxs-lookup"><span data-stu-id="290c5-127">Example</span></span>
<span data-ttu-id="290c5-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="290c5-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="290c5-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="290c5-129">Request</span></span>
<span data-ttu-id="290c5-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="290c5-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_headerrowrange"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/HeaderRowRange
```

##### <a name="response"></a><span data-ttu-id="290c5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="290c5-131">Response</span></span>
<span data-ttu-id="290c5-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="290c5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->