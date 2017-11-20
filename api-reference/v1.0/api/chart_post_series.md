# <a name="create-chartseries"></a><span data-ttu-id="40112-101">Создание объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="40112-101">Create ChartSeries</span></span>

<span data-ttu-id="40112-102">С помощью этого API можно создать объект ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="40112-102">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="40112-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40112-103">Permissions</span></span>
<span data-ttu-id="40112-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="40112-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="40112-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40112-106">Permission type</span></span>      | <span data-ttu-id="40112-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40112-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40112-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40112-108">Delegated (work or school account)</span></span> | <span data-ttu-id="40112-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40112-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="40112-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40112-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40112-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40112-111">Not supported.</span></span>    |
|<span data-ttu-id="40112-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40112-112">Application</span></span> | <span data-ttu-id="40112-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40112-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40112-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40112-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series

```
## <a name="request-headers"></a><span data-ttu-id="40112-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40112-115">Request headers</span></span>
| <span data-ttu-id="40112-116">Имя</span><span class="sxs-lookup"><span data-stu-id="40112-116">Name</span></span>       | <span data-ttu-id="40112-117">Описание</span><span class="sxs-lookup"><span data-stu-id="40112-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="40112-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40112-118">Authorization</span></span>  | <span data-ttu-id="40112-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40112-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="40112-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="40112-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="40112-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="40112-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40112-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40112-124">Request body</span></span>
<span data-ttu-id="40112-125">Предоставьте в тексте запроса описание объекта [ChartSeries](../resources/chartseries.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40112-125">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="40112-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="40112-126">Response</span></span>

<span data-ttu-id="40112-127">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ChartSeries](../resources/chartseries.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40112-127">If successful, this method returns `201 Created` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40112-128">Пример</span><span class="sxs-lookup"><span data-stu-id="40112-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40112-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="40112-129">Request</span></span>
<span data-ttu-id="40112-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40112-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
<span data-ttu-id="40112-131">Предоставьте в тексте запроса описание объекта [ChartSeries](../resources/chartseries.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40112-131">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="40112-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="40112-132">Response</span></span>
<span data-ttu-id="40112-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="40112-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->