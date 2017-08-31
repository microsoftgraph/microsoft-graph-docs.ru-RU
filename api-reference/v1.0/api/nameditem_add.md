# <a name="add-named-item"></a><span data-ttu-id="04b78-101">Add Named Item</span><span class="sxs-lookup"><span data-stu-id="04b78-101">Add Named Item</span></span>

<span data-ttu-id="04b78-102">Добавляет новое имя в определенную коллекцию, применяя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="04b78-102">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="04b78-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04b78-103">Permissions</span></span>
<span data-ttu-id="04b78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="04b78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="04b78-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04b78-106">Permission type</span></span>      | <span data-ttu-id="04b78-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04b78-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04b78-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04b78-108">Delegated (work or school account)</span></span> | <span data-ttu-id="04b78-109">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b78-109">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="04b78-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04b78-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04b78-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04b78-111">Not supported.</span></span>    |
|<span data-ttu-id="04b78-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04b78-112">Application</span></span> | <span data-ttu-id="04b78-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b78-113">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04b78-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04b78-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="04b78-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04b78-115">Request headers</span></span>
| <span data-ttu-id="04b78-116">Имя</span><span class="sxs-lookup"><span data-stu-id="04b78-116">Name</span></span>       | <span data-ttu-id="04b78-117">Описание</span><span class="sxs-lookup"><span data-stu-id="04b78-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="04b78-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04b78-118">Authorization</span></span>  | <span data-ttu-id="04b78-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04b78-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04b78-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04b78-121">Request body</span></span>
<span data-ttu-id="04b78-122">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="04b78-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="04b78-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="04b78-123">Parameter</span></span>    | <span data-ttu-id="04b78-124">Тип</span><span class="sxs-lookup"><span data-stu-id="04b78-124">Type</span></span>   |<span data-ttu-id="04b78-125">Описание</span><span class="sxs-lookup"><span data-stu-id="04b78-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04b78-126">name</span><span class="sxs-lookup"><span data-stu-id="04b78-126">name</span></span>|<span data-ttu-id="04b78-127">строка</span><span class="sxs-lookup"><span data-stu-id="04b78-127">string</span></span>|<span data-ttu-id="04b78-128">Имя именованного элемента.</span><span class="sxs-lookup"><span data-stu-id="04b78-128">The name of the named item.</span></span>|
|<span data-ttu-id="04b78-129">ссылка</span><span class="sxs-lookup"><span data-stu-id="04b78-129">reference</span></span>|<span data-ttu-id="04b78-130">string</span><span class="sxs-lookup"><span data-stu-id="04b78-130">string</span></span>|<span data-ttu-id="04b78-131">Формула или диапазон, на которые будет ссылаться имя.</span><span class="sxs-lookup"><span data-stu-id="04b78-131">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="04b78-132">примечание</span><span class="sxs-lookup"><span data-stu-id="04b78-132">comment</span></span>|<span data-ttu-id="04b78-133">string</span><span class="sxs-lookup"><span data-stu-id="04b78-133">string</span></span>|<span data-ttu-id="04b78-134">Комментарий, связанный с именованным элементом</span><span class="sxs-lookup"><span data-stu-id="04b78-134">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="04b78-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="04b78-135">Response</span></span>

<span data-ttu-id="04b78-136">В случае успеха этот метод возвращает код отклика `200, OK` и объект [NamedItem](../resources/NamedItem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04b78-136">If successful, this method returns `200, OK` response code and [NamedItem](../resources/NamedItem.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="04b78-137">Пример</span><span class="sxs-lookup"><span data-stu-id="04b78-137">Example</span></span>
<span data-ttu-id="04b78-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="04b78-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="04b78-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="04b78-139">Request</span></span>
<span data-ttu-id="04b78-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04b78-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="04b78-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="04b78-141">Response</span></span>
<span data-ttu-id="04b78-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="04b78-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
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
  "tocPath": ""
}-->
