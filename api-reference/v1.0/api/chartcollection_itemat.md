# <a name="chartcollection-itemat"></a><span data-ttu-id="9ef2a-101">ChartCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="9ef2a-101">ChartCollection: ItemAt</span></span>

<span data-ttu-id="9ef2a-102">Возвращает диаграмму на основании сведений о ее позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="9ef2a-102">Gets a chart based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="9ef2a-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ef2a-103">Permissions</span></span>
<span data-ttu-id="9ef2a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9ef2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9ef2a-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ef2a-106">Permission type</span></span>      | <span data-ttu-id="9ef2a-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ef2a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ef2a-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ef2a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9ef2a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ef2a-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9ef2a-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ef2a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ef2a-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ef2a-111">Not supported.</span></span>    |
|<span data-ttu-id="9ef2a-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ef2a-112">Application</span></span> | <span data-ttu-id="9ef2a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ef2a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ef2a-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ef2a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="9ef2a-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ef2a-115">Request headers</span></span>
| <span data-ttu-id="9ef2a-116">Имя</span><span class="sxs-lookup"><span data-stu-id="9ef2a-116">Name</span></span>       | <span data-ttu-id="9ef2a-117">Описание</span><span class="sxs-lookup"><span data-stu-id="9ef2a-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9ef2a-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ef2a-118">Authorization</span></span>  | <span data-ttu-id="9ef2a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ef2a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9ef2a-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9ef2a-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="9ef2a-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9ef2a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ef2a-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ef2a-124">Request body</span></span>
<span data-ttu-id="9ef2a-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9ef2a-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9ef2a-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="9ef2a-126">Parameter</span></span>    | <span data-ttu-id="9ef2a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="9ef2a-127">Type</span></span>   |<span data-ttu-id="9ef2a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="9ef2a-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ef2a-129">index</span><span class="sxs-lookup"><span data-stu-id="9ef2a-129">index</span></span>|<span data-ttu-id="9ef2a-130">number</span><span class="sxs-lookup"><span data-stu-id="9ef2a-130">number</span></span>|<span data-ttu-id="9ef2a-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="9ef2a-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="9ef2a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ef2a-133">Response</span></span>

<span data-ttu-id="9ef2a-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Chart](../resources/chart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9ef2a-134">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ef2a-135">Пример</span><span class="sxs-lookup"><span data-stu-id="9ef2a-135">Example</span></span>
<span data-ttu-id="9ef2a-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9ef2a-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9ef2a-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ef2a-137">Request</span></span>
<span data-ttu-id="9ef2a-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ef2a-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="9ef2a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ef2a-139">Response</span></span>
<span data-ttu-id="9ef2a-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9ef2a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->