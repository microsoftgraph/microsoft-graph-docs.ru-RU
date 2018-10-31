# <a name="update-nameditem"></a><span data-ttu-id="15c81-101">Обновление объекта NamedItem</span><span class="sxs-lookup"><span data-stu-id="15c81-101">Update nameditem</span></span>

<span data-ttu-id="15c81-102">Обновление свойств объекта nameditem.</span><span class="sxs-lookup"><span data-stu-id="15c81-102">Update the properties of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="15c81-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15c81-103">Permissions</span></span>
<span data-ttu-id="15c81-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="15c81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="15c81-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15c81-106">Permission type</span></span>      | <span data-ttu-id="15c81-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15c81-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15c81-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15c81-108">Delegated (work or school account)</span></span> | <span data-ttu-id="15c81-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15c81-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="15c81-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15c81-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15c81-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15c81-111">Not supported.</span></span>    |
|<span data-ttu-id="15c81-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15c81-112">Application</span></span> | <span data-ttu-id="15c81-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15c81-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="15c81-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15c81-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="15c81-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15c81-115">Optional request headers</span></span>
| <span data-ttu-id="15c81-116">Имя</span><span class="sxs-lookup"><span data-stu-id="15c81-116">Name</span></span>       | <span data-ttu-id="15c81-117">Описание</span><span class="sxs-lookup"><span data-stu-id="15c81-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="15c81-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15c81-118">Authorization</span></span>  | <span data-ttu-id="15c81-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15c81-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15c81-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="15c81-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="15c81-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="15c81-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="15c81-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15c81-124">Request body</span></span>
<span data-ttu-id="15c81-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="15c81-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="15c81-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="15c81-128">Property</span></span>     | <span data-ttu-id="15c81-129">Тип</span><span class="sxs-lookup"><span data-stu-id="15c81-129">Type</span></span>   |<span data-ttu-id="15c81-130">Описание</span><span class="sxs-lookup"><span data-stu-id="15c81-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15c81-131">видимый</span><span class="sxs-lookup"><span data-stu-id="15c81-131">visible</span></span>|<span data-ttu-id="15c81-132">логический</span><span class="sxs-lookup"><span data-stu-id="15c81-132">boolean</span></span>|<span data-ttu-id="15c81-133">Определяет, является ли объект видимым.</span><span class="sxs-lookup"><span data-stu-id="15c81-133">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="15c81-134">комментарий</span><span class="sxs-lookup"><span data-stu-id="15c81-134">comment</span></span>|   <span data-ttu-id="15c81-135">строка</span><span class="sxs-lookup"><span data-stu-id="15c81-135">string</span></span>  |<span data-ttu-id="15c81-136">Представляет примечание, связанное с этим именем.</span><span class="sxs-lookup"><span data-stu-id="15c81-136">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="15c81-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="15c81-137">Response</span></span>

<span data-ttu-id="15c81-138">В случае`200 OK`   успеха этот метод возвращает код отклика  и обновленный объект WorkbookNamedItem в тексте отклика.[](../resources/nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="15c81-138">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/nameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="15c81-139">Пример</span><span class="sxs-lookup"><span data-stu-id="15c81-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15c81-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="15c81-140">Request</span></span>
<span data-ttu-id="15c81-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15c81-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_nameditem"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}
Content-type: application/json
Content-length: 87

{
  "type": "type-value",
  "scope": "scope-value",
  "comment": "comment-value",
  "value": {
  },
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="15c81-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="15c81-142">Response</span></span>
<span data-ttu-id="15c81-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15c81-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 87

{
  "name": "name-value",
  "type": "type-value",
  "value": {
  },
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update nameditem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
