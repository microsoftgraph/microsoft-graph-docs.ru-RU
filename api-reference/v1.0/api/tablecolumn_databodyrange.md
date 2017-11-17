# <a name="tablecolumn-databodyrange"></a><span data-ttu-id="87273-101">TableColumn: DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="87273-101">TableColumn: DataBodyRange</span></span>

<span data-ttu-id="87273-102">Получает объект диапазона, связанный с данными столбца.</span><span class="sxs-lookup"><span data-stu-id="87273-102">Gets the range object associated with the data body of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="87273-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87273-103">Permissions</span></span>
<span data-ttu-id="87273-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="87273-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="87273-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87273-106">Permission type</span></span>      | <span data-ttu-id="87273-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87273-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87273-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87273-108">Delegated (work or school account)</span></span> | <span data-ttu-id="87273-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87273-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="87273-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87273-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87273-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87273-111">Not supported.</span></span>    |
|<span data-ttu-id="87273-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87273-112">Application</span></span> | <span data-ttu-id="87273-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87273-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87273-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87273-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/DataBodyRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/DataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="87273-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87273-115">Request headers</span></span>
| <span data-ttu-id="87273-116">Имя</span><span class="sxs-lookup"><span data-stu-id="87273-116">Name</span></span>       | <span data-ttu-id="87273-117">Описание</span><span class="sxs-lookup"><span data-stu-id="87273-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="87273-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87273-118">Authorization</span></span>  | <span data-ttu-id="87273-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87273-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87273-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87273-121">Request body</span></span>

## <a name="response"></a><span data-ttu-id="87273-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="87273-122">Response</span></span>

<span data-ttu-id="87273-123">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="87273-123">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87273-124">Пример</span><span class="sxs-lookup"><span data-stu-id="87273-124">Example</span></span>
<span data-ttu-id="87273-125">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="87273-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="87273-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="87273-126">Request</span></span>
<span data-ttu-id="87273-127">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87273-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumn_databodyrange"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/DataBodyRange
```

##### <a name="response"></a><span data-ttu-id="87273-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="87273-128">Response</span></span>
<span data-ttu-id="87273-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="87273-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumn: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->