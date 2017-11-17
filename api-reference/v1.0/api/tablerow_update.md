# <a name="update-tablerow"></a><span data-ttu-id="85072-101">Обновление объекта tableRow</span><span class="sxs-lookup"><span data-stu-id="85072-101">Update tablerow</span></span>

<span data-ttu-id="85072-102">Обновление свойств объекта tablerow.</span><span class="sxs-lookup"><span data-stu-id="85072-102">Update the properties of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="85072-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85072-103">Permissions</span></span>
<span data-ttu-id="85072-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="85072-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="85072-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85072-106">Permission type</span></span>      | <span data-ttu-id="85072-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85072-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85072-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85072-108">Delegated (work or school account)</span></span> | <span data-ttu-id="85072-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85072-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="85072-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85072-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85072-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85072-111">Not supported.</span></span>    |
|<span data-ttu-id="85072-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85072-112">Application</span></span> | <span data-ttu-id="85072-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85072-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85072-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85072-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/rows(<index>)
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="85072-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85072-115">Optional request headers</span></span>
| <span data-ttu-id="85072-116">Имя</span><span class="sxs-lookup"><span data-stu-id="85072-116">Name</span></span>       | <span data-ttu-id="85072-117">Описание</span><span class="sxs-lookup"><span data-stu-id="85072-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="85072-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85072-118">Authorization</span></span>  | <span data-ttu-id="85072-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85072-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85072-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85072-121">Request body</span></span>
<span data-ttu-id="85072-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="85072-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="85072-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="85072-125">Property</span></span>     | <span data-ttu-id="85072-126">Тип</span><span class="sxs-lookup"><span data-stu-id="85072-126">Type</span></span>   |<span data-ttu-id="85072-127">Описание</span><span class="sxs-lookup"><span data-stu-id="85072-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85072-128">values</span><span class="sxs-lookup"><span data-stu-id="85072-128">values</span></span>|<span data-ttu-id="85072-129">json</span><span class="sxs-lookup"><span data-stu-id="85072-129">json</span></span>|<span data-ttu-id="85072-p104">Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="85072-p104">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="85072-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="85072-133">Response</span></span>

<span data-ttu-id="85072-134">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [tableRow](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85072-134">If successful, this method returns a `200 OK` response code and updated [TableRow](../resources/tablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="85072-135">Пример</span><span class="sxs-lookup"><span data-stu-id="85072-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85072-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="85072-136">Request</span></span>
<span data-ttu-id="85072-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85072-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablerow"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="85072-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="85072-138">Response</span></span>
<span data-ttu-id="85072-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="85072-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tablerow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->