# <a name="chartpointscollection-itemat"></a><span data-ttu-id="53d5d-101">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="53d5d-101">ChartPointsCollection: ItemAt</span></span>

<span data-ttu-id="53d5d-102">Получение точки на основании сведений о ее позиции в ряду.</span><span class="sxs-lookup"><span data-stu-id="53d5d-102">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="53d5d-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53d5d-103">Permissions</span></span>
<span data-ttu-id="53d5d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="53d5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="53d5d-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53d5d-106">Permission type</span></span>      | <span data-ttu-id="53d5d-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53d5d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53d5d-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53d5d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="53d5d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53d5d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="53d5d-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53d5d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53d5d-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53d5d-111">Not supported.</span></span>    |
|<span data-ttu-id="53d5d-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53d5d-112">Application</span></span> | <span data-ttu-id="53d5d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53d5d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="53d5d-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53d5d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="53d5d-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53d5d-115">Request headers</span></span>
| <span data-ttu-id="53d5d-116">Имя</span><span class="sxs-lookup"><span data-stu-id="53d5d-116">Name</span></span>       | <span data-ttu-id="53d5d-117">Описание</span><span class="sxs-lookup"><span data-stu-id="53d5d-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="53d5d-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53d5d-118">Authorization</span></span>  | <span data-ttu-id="53d5d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53d5d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53d5d-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53d5d-121">Request body</span></span>
<span data-ttu-id="53d5d-122">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="53d5d-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="53d5d-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="53d5d-123">Parameter</span></span>    | <span data-ttu-id="53d5d-124">Тип</span><span class="sxs-lookup"><span data-stu-id="53d5d-124">Type</span></span>   |<span data-ttu-id="53d5d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="53d5d-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53d5d-126">index</span><span class="sxs-lookup"><span data-stu-id="53d5d-126">index</span></span>|<span data-ttu-id="53d5d-127">number</span><span class="sxs-lookup"><span data-stu-id="53d5d-127">number</span></span>|<span data-ttu-id="53d5d-p103">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="53d5d-p103">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="53d5d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="53d5d-130">Response</span></span>

<span data-ttu-id="53d5d-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [ChartPoint](../resources/chartpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="53d5d-131">If successful, this method returns `200 OK` response code and [ChartPoint](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53d5d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="53d5d-132">Example</span></span>
<span data-ttu-id="53d5d-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="53d5d-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="53d5d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="53d5d-134">Request</span></span>
<span data-ttu-id="53d5d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53d5d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartpointscollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="53d5d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="53d5d-136">Response</span></span>
<span data-ttu-id="53d5d-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="53d5d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 20

{
  "value": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointsCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->