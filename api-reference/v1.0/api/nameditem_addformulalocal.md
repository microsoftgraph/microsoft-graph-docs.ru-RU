# <a name="add-named-item-formulalocal"></a><span data-ttu-id="6ed03-101">Add Named Item FormulaLocal</span><span class="sxs-lookup"><span data-stu-id="6ed03-101">Add Named Item FormulaLocal</span></span>
<span data-ttu-id="6ed03-102">Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="6ed03-102">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ed03-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ed03-103">Permissions</span></span>
<span data-ttu-id="6ed03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6ed03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6ed03-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ed03-106">Permission type</span></span>      | <span data-ttu-id="6ed03-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ed03-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ed03-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ed03-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6ed03-109">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ed03-109">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="6ed03-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ed03-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ed03-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ed03-111">Not supported.</span></span>    |
|<span data-ttu-id="6ed03-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ed03-112">Application</span></span> | <span data-ttu-id="6ed03-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ed03-113">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ed03-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ed03-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="6ed03-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ed03-115">Request headers</span></span>
| <span data-ttu-id="6ed03-116">Имя</span><span class="sxs-lookup"><span data-stu-id="6ed03-116">Name</span></span>       | <span data-ttu-id="6ed03-117">Описание</span><span class="sxs-lookup"><span data-stu-id="6ed03-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6ed03-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ed03-118">Authorization</span></span>  | <span data-ttu-id="6ed03-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ed03-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6ed03-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6ed03-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="6ed03-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="6ed03-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ed03-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ed03-124">Request body</span></span>
<span data-ttu-id="6ed03-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6ed03-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6ed03-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="6ed03-126">Parameter</span></span>    | <span data-ttu-id="6ed03-127">Тип</span><span class="sxs-lookup"><span data-stu-id="6ed03-127">Type</span></span>   |<span data-ttu-id="6ed03-128">Описание</span><span class="sxs-lookup"><span data-stu-id="6ed03-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ed03-129">name</span><span class="sxs-lookup"><span data-stu-id="6ed03-129">name</span></span>|<span data-ttu-id="6ed03-130">string</span><span class="sxs-lookup"><span data-stu-id="6ed03-130">string</span></span>|<span data-ttu-id="6ed03-131">Имя именованного элемента.</span><span class="sxs-lookup"><span data-stu-id="6ed03-131">The name of the named item.</span></span>|
|<span data-ttu-id="6ed03-132">формула</span><span class="sxs-lookup"><span data-stu-id="6ed03-132">formula</span></span>|<span data-ttu-id="6ed03-133">string</span><span class="sxs-lookup"><span data-stu-id="6ed03-133">string</span></span>|<span data-ttu-id="6ed03-134">Формула или диапазон, на которые будет ссылаться имя.</span><span class="sxs-lookup"><span data-stu-id="6ed03-134">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="6ed03-135">примечание</span><span class="sxs-lookup"><span data-stu-id="6ed03-135">comment</span></span>|<span data-ttu-id="6ed03-136">string</span><span class="sxs-lookup"><span data-stu-id="6ed03-136">string</span></span>|<span data-ttu-id="6ed03-137">Комментарий, связанный с именованным элементом</span><span class="sxs-lookup"><span data-stu-id="6ed03-137">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="6ed03-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ed03-138">Response</span></span>

<span data-ttu-id="6ed03-139">В случае успеха этот метод возвращает `200 OK` код отклика и объект [WorkbookNamedItem](../resources/NamedItem.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6ed03-139">If successful, this method returns `200 OK` response code and [groupSetting](../resources/NamedItem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ed03-140">Пример</span><span class="sxs-lookup"><span data-stu-id="6ed03-140">Example</span></span>
<span data-ttu-id="6ed03-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6ed03-141">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6ed03-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ed03-142">Request</span></span>
<span data-ttu-id="6ed03-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ed03-143">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/addFormulaLocal
Content-type: application/json
Content-length: 54

{
  "name": "test7",
  "formula": "=SUM(Sheet2!$A$1+Sheet2!$A$2)",
  "comment": "Comment for the named item"
}
```

##### <a name="response"></a><span data-ttu-id="6ed03-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ed03-144">Response</span></span>
<span data-ttu-id="6ed03-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ed03-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookNamedItem",
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test7%27)",
    "comment": "Comment for the named item",
    "name": "test7",
    "scope": "Workbook",
    "type": "String",
    "value": "0",
    "visible": true
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
