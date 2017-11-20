# <a name="rangebordercollection-itemat"></a><span data-ttu-id="75a9d-101">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="75a9d-101">RangeBorderCollection: ItemAt</span></span>

<span data-ttu-id="75a9d-102">Возвращает объект границы, указанный по индексу.</span><span class="sxs-lookup"><span data-stu-id="75a9d-102">Gets a border object using its index</span></span>
## <a name="permissions"></a><span data-ttu-id="75a9d-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75a9d-103">Permissions</span></span>
<span data-ttu-id="75a9d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="75a9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="75a9d-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75a9d-106">Permission type</span></span>      | <span data-ttu-id="75a9d-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75a9d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75a9d-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75a9d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="75a9d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75a9d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="75a9d-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75a9d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75a9d-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75a9d-111">Not supported.</span></span>    |
|<span data-ttu-id="75a9d-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75a9d-112">Application</span></span> | <span data-ttu-id="75a9d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75a9d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75a9d-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75a9d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/borders/ItemAt
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/ItemAt
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="75a9d-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75a9d-115">Request headers</span></span>
| <span data-ttu-id="75a9d-116">Имя</span><span class="sxs-lookup"><span data-stu-id="75a9d-116">Name</span></span>       | <span data-ttu-id="75a9d-117">Описание</span><span class="sxs-lookup"><span data-stu-id="75a9d-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="75a9d-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75a9d-118">Authorization</span></span>  | <span data-ttu-id="75a9d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75a9d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="75a9d-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="75a9d-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="75a9d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="75a9d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75a9d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75a9d-124">Request body</span></span>
<span data-ttu-id="75a9d-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="75a9d-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="75a9d-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="75a9d-126">Parameter</span></span>    | <span data-ttu-id="75a9d-127">Тип</span><span class="sxs-lookup"><span data-stu-id="75a9d-127">Type</span></span>   |<span data-ttu-id="75a9d-128">Описание</span><span class="sxs-lookup"><span data-stu-id="75a9d-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75a9d-129">index</span><span class="sxs-lookup"><span data-stu-id="75a9d-129">index</span></span>|<span data-ttu-id="75a9d-130">number</span><span class="sxs-lookup"><span data-stu-id="75a9d-130">number</span></span>|<span data-ttu-id="75a9d-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="75a9d-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="75a9d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="75a9d-133">Response</span></span>

<span data-ttu-id="75a9d-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [RangeBorder](../resources/rangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75a9d-134">If successful, this method returns `200 OK` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75a9d-135">Пример</span><span class="sxs-lookup"><span data-stu-id="75a9d-135">Example</span></span>
<span data-ttu-id="75a9d-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="75a9d-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="75a9d-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="75a9d-137">Request</span></span>
<span data-ttu-id="75a9d-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75a9d-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangebordercollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/borders/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="75a9d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="75a9d-139">Response</span></span>
<span data-ttu-id="75a9d-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="75a9d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorderCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->