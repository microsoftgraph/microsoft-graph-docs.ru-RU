# <a name="table-databodyrange"></a><span data-ttu-id="e0305-101">Table: DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="e0305-101">Table: DataBodyRange</span></span>

<span data-ttu-id="e0305-102">Получает объект диапазона, связанный с данными таблицы.</span><span class="sxs-lookup"><span data-stu-id="e0305-102">Gets the range object associated with the data body of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="e0305-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e0305-103">Permissions</span></span>
<span data-ttu-id="e0305-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e0305-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e0305-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0305-106">Permission type</span></span>      | <span data-ttu-id="e0305-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0305-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0305-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0305-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e0305-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0305-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e0305-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0305-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0305-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0305-111">Not supported.</span></span>    |
|<span data-ttu-id="e0305-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0305-112">Application</span></span> | <span data-ttu-id="e0305-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0305-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0305-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0305-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/dataBodyRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/dataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="e0305-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0305-115">Request headers</span></span>
| <span data-ttu-id="e0305-116">Имя</span><span class="sxs-lookup"><span data-stu-id="e0305-116">Name</span></span>       | <span data-ttu-id="e0305-117">Описание</span><span class="sxs-lookup"><span data-stu-id="e0305-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e0305-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0305-118">Authorization</span></span>  | <span data-ttu-id="e0305-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0305-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e0305-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e0305-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="e0305-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e0305-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0305-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e0305-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e0305-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0305-125">Response</span></span>

<span data-ttu-id="e0305-126">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e0305-126">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0305-127">Пример</span><span class="sxs-lookup"><span data-stu-id="e0305-127">Example</span></span>
<span data-ttu-id="e0305-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e0305-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e0305-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0305-129">Request</span></span>
<span data-ttu-id="e0305-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0305-130">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "table_databodyrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/dataBodyRange
```

##### <a name="response"></a><span data-ttu-id="e0305-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0305-131">Response</span></span>
<span data-ttu-id="e0305-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0305-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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
  "description": "Table: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->