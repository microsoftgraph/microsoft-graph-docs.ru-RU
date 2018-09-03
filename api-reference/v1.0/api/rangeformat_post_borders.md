# <a name="create-rangeborder"></a><span data-ttu-id="80a7d-101">Создание объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="80a7d-101">Create RangeBorder</span></span>

<span data-ttu-id="80a7d-102">С помощью этого API можно создать объект RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="80a7d-102">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="80a7d-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80a7d-103">Permissions</span></span>
<span data-ttu-id="80a7d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="80a7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="80a7d-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80a7d-106">Permission type</span></span>      | <span data-ttu-id="80a7d-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80a7d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80a7d-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80a7d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="80a7d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80a7d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="80a7d-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80a7d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80a7d-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80a7d-111">Not supported.</span></span>    |
|<span data-ttu-id="80a7d-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80a7d-112">Application</span></span> | <span data-ttu-id="80a7d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80a7d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="80a7d-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80a7d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="80a7d-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80a7d-115">Request headers</span></span>
| <span data-ttu-id="80a7d-116">Имя</span><span class="sxs-lookup"><span data-stu-id="80a7d-116">Name</span></span>       | <span data-ttu-id="80a7d-117">Описание</span><span class="sxs-lookup"><span data-stu-id="80a7d-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="80a7d-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80a7d-118">Authorization</span></span>  | <span data-ttu-id="80a7d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80a7d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="80a7d-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="80a7d-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="80a7d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="80a7d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="80a7d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="80a7d-124">Request body</span></span>
<span data-ttu-id="80a7d-125">Предоставьте в тексте запроса описание объекта [WorkbookRangeBorder](../resources/rangeborder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80a7d-125">In the request body, supply a JSON representation of [directoryObject](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="80a7d-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="80a7d-126">Response</span></span>

<span data-ttu-id="80a7d-127">В случае успеха этот метод возвращает код отклика `201 Created` и обновленный объект [WorkbookRangeBorder](../resources/rangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="80a7d-127">If successful, this method returns `201 Created` response code and [groupSetting](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80a7d-128">Пример</span><span class="sxs-lookup"><span data-stu-id="80a7d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="80a7d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="80a7d-129">Request</span></span>
<span data-ttu-id="80a7d-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80a7d-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders
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
<span data-ttu-id="80a7d-131">Предоставьте в тексте запроса описание объекта [WorkbookRangeBorder](../resources/rangeborder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80a7d-131">In the request body, supply a JSON representation of [plannerPlan](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="80a7d-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="80a7d-132">Response</span></span>
<span data-ttu-id="80a7d-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="80a7d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->