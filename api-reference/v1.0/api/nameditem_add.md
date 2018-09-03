# <a name="add-named-item"></a><span data-ttu-id="f1003-101">Add Named Item</span><span class="sxs-lookup"><span data-stu-id="f1003-101">Add Named Item</span></span>

<span data-ttu-id="f1003-102">Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="f1003-102">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1003-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1003-103">Permissions</span></span>
<span data-ttu-id="f1003-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f1003-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f1003-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1003-106">Permission type</span></span>      | <span data-ttu-id="f1003-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1003-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1003-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1003-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f1003-109">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1003-109">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="f1003-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1003-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1003-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1003-111">Not supported.</span></span>    |
|<span data-ttu-id="f1003-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1003-112">Application</span></span> | <span data-ttu-id="f1003-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1003-113">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1003-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1003-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="f1003-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1003-115">Request headers</span></span>
| <span data-ttu-id="f1003-116">Имя</span><span class="sxs-lookup"><span data-stu-id="f1003-116">Name</span></span>       | <span data-ttu-id="f1003-117">Описание</span><span class="sxs-lookup"><span data-stu-id="f1003-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f1003-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1003-118">Authorization</span></span>  | <span data-ttu-id="f1003-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1003-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f1003-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f1003-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="f1003-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f1003-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1003-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1003-124">Request body</span></span>
<span data-ttu-id="f1003-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f1003-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f1003-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="f1003-126">Parameter</span></span>    | <span data-ttu-id="f1003-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f1003-127">Type</span></span>   |<span data-ttu-id="f1003-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f1003-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1003-129">name</span><span class="sxs-lookup"><span data-stu-id="f1003-129">name</span></span>|<span data-ttu-id="f1003-130">строка</span><span class="sxs-lookup"><span data-stu-id="f1003-130">string</span></span>|<span data-ttu-id="f1003-131">Имя именованного элемента.</span><span class="sxs-lookup"><span data-stu-id="f1003-131">The name of the named item.</span></span>|
|<span data-ttu-id="f1003-132">ссылка</span><span class="sxs-lookup"><span data-stu-id="f1003-132">reference</span></span>|<span data-ttu-id="f1003-133">Json</span><span class="sxs-lookup"><span data-stu-id="f1003-133">Json</span></span>|<span data-ttu-id="f1003-134">Формула или диапазон, на которые будет ссылаться имя.</span><span class="sxs-lookup"><span data-stu-id="f1003-134">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="f1003-135">примечание</span><span class="sxs-lookup"><span data-stu-id="f1003-135">comment</span></span>|<span data-ttu-id="f1003-136">строка</span><span class="sxs-lookup"><span data-stu-id="f1003-136">string</span></span>|<span data-ttu-id="f1003-137">Комментарий, связанный с именованным элементом</span><span class="sxs-lookup"><span data-stu-id="f1003-137">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="f1003-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1003-138">Response</span></span>

<span data-ttu-id="f1003-139">В случае успеха, этот метод  возвращает `200 OK`код ответа и объект [WorkbookNamedItem](../resources/NamedItem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f1003-139">If successful, this method returns `200 OK` response code and [groupSetting](../resources/NamedItem.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="f1003-140">Пример</span><span class="sxs-lookup"><span data-stu-id="f1003-140">Example</span></span>
<span data-ttu-id="f1003-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f1003-141">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f1003-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1003-142">Request</span></span>
<span data-ttu-id="f1003-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1003-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "test5",
  "reference": "=Sheet1!$F$15:$N$27",
  "comment": "Comment for the named item"
}


```

##### <a name="response"></a><span data-ttu-id="f1003-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1003-144">Response</span></span>
<span data-ttu-id="f1003-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1003-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test5%27)",
    "comment": "Comment for the named item",
    "name": "test5",
    "scope": "Workbook",
    "type": "Range",
    "value": "Sheet1!$F$15:$N$27",
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
  "suppressions": [
    "Warning: NamedItemcollection_add/value:
      Schemas type was 'Custom' which is not supported. Add a resource type to the definition of property: value"
  ],
  "tocPath": ""
}-->
