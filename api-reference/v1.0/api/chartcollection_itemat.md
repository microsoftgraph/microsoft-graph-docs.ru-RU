# <a name="chartcollection-itemat"></a><span data-ttu-id="03e1b-101">ChartCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="03e1b-101">ChartCollection: ItemAt</span></span>

<span data-ttu-id="03e1b-102">Возвращает диаграмму на основании сведений о ее позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="03e1b-102">Gets a chart based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="03e1b-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03e1b-103">Permissions</span></span>
<span data-ttu-id="03e1b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="03e1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="03e1b-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03e1b-106">Permission type</span></span>      | <span data-ttu-id="03e1b-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03e1b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03e1b-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03e1b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="03e1b-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03e1b-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="03e1b-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03e1b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03e1b-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03e1b-111">Not supported.</span></span>    |
|<span data-ttu-id="03e1b-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03e1b-112">Application</span></span> | <span data-ttu-id="03e1b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03e1b-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="03e1b-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03e1b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="03e1b-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03e1b-115">Request headers</span></span>
| <span data-ttu-id="03e1b-116">Имя</span><span class="sxs-lookup"><span data-stu-id="03e1b-116">Name</span></span>       | <span data-ttu-id="03e1b-117">Описание</span><span class="sxs-lookup"><span data-stu-id="03e1b-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="03e1b-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03e1b-118">Authorization</span></span>  | <span data-ttu-id="03e1b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03e1b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03e1b-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03e1b-121">Request body</span></span>
<span data-ttu-id="03e1b-122">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="03e1b-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="03e1b-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="03e1b-123">Parameter</span></span>    | <span data-ttu-id="03e1b-124">Тип</span><span class="sxs-lookup"><span data-stu-id="03e1b-124">Type</span></span>   |<span data-ttu-id="03e1b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="03e1b-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03e1b-126">index</span><span class="sxs-lookup"><span data-stu-id="03e1b-126">index</span></span>|<span data-ttu-id="03e1b-127">number</span><span class="sxs-lookup"><span data-stu-id="03e1b-127">number</span></span>|<span data-ttu-id="03e1b-p103">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="03e1b-p103">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="03e1b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="03e1b-130">Response</span></span>

<span data-ttu-id="03e1b-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Chart](../resources/chart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03e1b-131">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03e1b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="03e1b-132">Example</span></span>
<span data-ttu-id="03e1b-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="03e1b-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="03e1b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="03e1b-134">Request</span></span>
<span data-ttu-id="03e1b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03e1b-135">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="03e1b-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="03e1b-136">Response</span></span>
<span data-ttu-id="03e1b-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="03e1b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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