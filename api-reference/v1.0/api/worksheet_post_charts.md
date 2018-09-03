# <a name="create-chart"></a><span data-ttu-id="02d9e-101">Создание объекта Chart</span><span class="sxs-lookup"><span data-stu-id="02d9e-101">Create Chart</span></span>

<span data-ttu-id="02d9e-102">С помощью этого API можно создать объект Chart.</span><span class="sxs-lookup"><span data-stu-id="02d9e-102">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="02d9e-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02d9e-103">Permissions</span></span>
<span data-ttu-id="02d9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="02d9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="02d9e-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02d9e-106">Permission type</span></span>      | <span data-ttu-id="02d9e-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02d9e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02d9e-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02d9e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="02d9e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02d9e-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="02d9e-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02d9e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02d9e-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02d9e-111">Not supported.</span></span>    |
|<span data-ttu-id="02d9e-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02d9e-112">Application</span></span> | <span data-ttu-id="02d9e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02d9e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02d9e-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02d9e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="02d9e-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02d9e-115">Request headers</span></span>
| <span data-ttu-id="02d9e-116">Имя</span><span class="sxs-lookup"><span data-stu-id="02d9e-116">Name</span></span>       | <span data-ttu-id="02d9e-117">Описание</span><span class="sxs-lookup"><span data-stu-id="02d9e-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="02d9e-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02d9e-118">Authorization</span></span>  | <span data-ttu-id="02d9e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02d9e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="02d9e-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="02d9e-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="02d9e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="02d9e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02d9e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="02d9e-124">Request body</span></span>
<span data-ttu-id="02d9e-125">В тексте запроса укажите представление JSON объекта [WorkbookChart](../resources/chart.md).</span><span class="sxs-lookup"><span data-stu-id="02d9e-125">In the request body, supply a JSON representation of [directoryObject](../resources/chart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="02d9e-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="02d9e-126">Response</span></span>

<span data-ttu-id="02d9e-127">В случае успеха этот метод возвращает`201 Created` код ответа и объект [WorkbookChart](../resources/chart.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="02d9e-127">If successful, this method returns `201 Created` response code and [groupSetting](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02d9e-128">Пример</span><span class="sxs-lookup"><span data-stu-id="02d9e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02d9e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="02d9e-129">Request</span></span>
<span data-ttu-id="02d9e-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02d9e-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chart_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
<span data-ttu-id="02d9e-131">В тексте запроса укажите представление JSON объекта [WorkbookChart](../resources/chart.md).</span><span class="sxs-lookup"><span data-stu-id="02d9e-131">In the request body, supply a JSON representation of [plannerPlan](../resources/chart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="02d9e-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="02d9e-132">Response</span></span>
<span data-ttu-id="02d9e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02d9e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->