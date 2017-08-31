# <a name="update-rangefill"></a><span data-ttu-id="30db7-101">Обновление объекта rangeFill</span><span class="sxs-lookup"><span data-stu-id="30db7-101">Update rangefill</span></span>

<span data-ttu-id="30db7-102">Обновление свойств объекта rangefill.</span><span class="sxs-lookup"><span data-stu-id="30db7-102">Update the properties of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="30db7-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30db7-103">Permissions</span></span>
<span data-ttu-id="30db7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="30db7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="30db7-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30db7-106">Permission type</span></span>      | <span data-ttu-id="30db7-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30db7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30db7-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30db7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="30db7-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30db7-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="30db7-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30db7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30db7-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30db7-111">Not supported.</span></span>    |
|<span data-ttu-id="30db7-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30db7-112">Application</span></span> | <span data-ttu-id="30db7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30db7-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="30db7-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30db7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/fill
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/fill
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-request-headers"></a><span data-ttu-id="30db7-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30db7-115">Optional request headers</span></span>
| <span data-ttu-id="30db7-116">Имя</span><span class="sxs-lookup"><span data-stu-id="30db7-116">Name</span></span>       | <span data-ttu-id="30db7-117">Описание</span><span class="sxs-lookup"><span data-stu-id="30db7-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="30db7-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30db7-118">Authorization</span></span>  | <span data-ttu-id="30db7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30db7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30db7-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30db7-121">Request body</span></span>
<span data-ttu-id="30db7-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="30db7-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="30db7-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="30db7-125">Property</span></span>     | <span data-ttu-id="30db7-126">Тип</span><span class="sxs-lookup"><span data-stu-id="30db7-126">Type</span></span>   |<span data-ttu-id="30db7-127">Описание</span><span class="sxs-lookup"><span data-stu-id="30db7-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30db7-128">color</span><span class="sxs-lookup"><span data-stu-id="30db7-128">color</span></span>|<span data-ttu-id="30db7-129">string</span><span class="sxs-lookup"><span data-stu-id="30db7-129">string</span></span>|<span data-ttu-id="30db7-130">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).</span><span class="sxs-lookup"><span data-stu-id="30db7-130">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="response"></a><span data-ttu-id="30db7-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="30db7-131">Response</span></span>

<span data-ttu-id="30db7-132">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [RangeFill](../resources/rangefill.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30db7-132">If successful, this method returns a `200 OK` response code and updated [RangeFill](../resources/rangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="30db7-133">Пример</span><span class="sxs-lookup"><span data-stu-id="30db7-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30db7-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="30db7-134">Request</span></span>
<span data-ttu-id="30db7-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30db7-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangefill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/fill
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="30db7-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="30db7-136">Response</span></span>
<span data-ttu-id="30db7-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="30db7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangefill",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->