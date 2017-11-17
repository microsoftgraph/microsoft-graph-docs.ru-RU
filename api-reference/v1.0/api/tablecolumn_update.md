# <a name="update-tablecolumn"></a><span data-ttu-id="c144e-101">Обновление объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="c144e-101">Update tablecolumn</span></span>

<span data-ttu-id="c144e-102">Обновление свойств объекта tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="c144e-102">Update the properties of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c144e-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c144e-103">Permissions</span></span>
<span data-ttu-id="c144e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c144e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c144e-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c144e-106">Permission type</span></span>      | <span data-ttu-id="c144e-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c144e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c144e-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c144e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c144e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c144e-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c144e-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c144e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c144e-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c144e-111">Not supported.</span></span>    |
|<span data-ttu-id="c144e-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c144e-112">Application</span></span> | <span data-ttu-id="c144e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c144e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c144e-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c144e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/columns/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="c144e-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c144e-115">Optional request headers</span></span>
| <span data-ttu-id="c144e-116">Имя</span><span class="sxs-lookup"><span data-stu-id="c144e-116">Name</span></span>       | <span data-ttu-id="c144e-117">Описание</span><span class="sxs-lookup"><span data-stu-id="c144e-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c144e-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c144e-118">Authorization</span></span>  | <span data-ttu-id="c144e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c144e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c144e-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c144e-121">Request body</span></span>
<span data-ttu-id="c144e-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c144e-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c144e-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="c144e-125">Property</span></span>     | <span data-ttu-id="c144e-126">Тип</span><span class="sxs-lookup"><span data-stu-id="c144e-126">Type</span></span>   |<span data-ttu-id="c144e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c144e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c144e-128">values</span><span class="sxs-lookup"><span data-stu-id="c144e-128">values</span></span>|<span data-ttu-id="c144e-129">json</span><span class="sxs-lookup"><span data-stu-id="c144e-129">json</span></span>|<span data-ttu-id="c144e-p104">Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="c144e-p104">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="c144e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c144e-133">Response</span></span>

<span data-ttu-id="c144e-134">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [TableColumn](../resources/tablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c144e-134">If successful, this method returns a `200 OK` response code and updated [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c144e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="c144e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c144e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="c144e-136">Request</span></span>
<span data-ttu-id="c144e-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c144e-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablecolumn"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
Content-type: application/json
Content-length: 81

{
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="c144e-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="c144e-138">Response</span></span>
<span data-ttu-id="c144e-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c144e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tablecolumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->