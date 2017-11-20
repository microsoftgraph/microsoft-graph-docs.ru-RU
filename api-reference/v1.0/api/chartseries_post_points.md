# <a name="create-chartpoints"></a><span data-ttu-id="3e641-101">Создание объекта ChartPoints</span><span class="sxs-lookup"><span data-stu-id="3e641-101">Create ChartPoints</span></span>

<span data-ttu-id="3e641-102">С помощью этого API можно создать объект ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="3e641-102">Use this API to create a new ChartPoints.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e641-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e641-103">Permissions</span></span>
<span data-ttu-id="3e641-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3e641-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3e641-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e641-106">Permission type</span></span>      | <span data-ttu-id="3e641-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e641-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e641-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e641-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3e641-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e641-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3e641-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e641-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e641-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e641-111">Not supported.</span></span>    |
|<span data-ttu-id="3e641-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e641-112">Application</span></span> | <span data-ttu-id="3e641-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e641-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e641-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e641-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points

```
## <a name="request-headers"></a><span data-ttu-id="3e641-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e641-115">Request headers</span></span>
| <span data-ttu-id="3e641-116">Имя</span><span class="sxs-lookup"><span data-stu-id="3e641-116">Name</span></span>       | <span data-ttu-id="3e641-117">Описание</span><span class="sxs-lookup"><span data-stu-id="3e641-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3e641-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e641-118">Authorization</span></span>  | <span data-ttu-id="3e641-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e641-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e641-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3e641-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="3e641-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="3e641-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e641-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e641-124">Request body</span></span>
<span data-ttu-id="3e641-125">Предоставьте в тексте запроса описание объекта [ChartPoints](../resources/chartpoint.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e641-125">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3e641-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e641-126">Response</span></span>

<span data-ttu-id="3e641-127">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ChartPoints](../resources/chartpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3e641-127">If successful, this method returns `201 Created` response code and [ChartPoints](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e641-128">Пример</span><span class="sxs-lookup"><span data-stu-id="3e641-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e641-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e641-129">Request</span></span>
<span data-ttu-id="3e641-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e641-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartpoints_from_chartseries"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
Content-type: application/json
Content-length: 3

{
}
```
<span data-ttu-id="3e641-131">Предоставьте в тексте запроса описание объекта [ChartPoints](../resources/chartpoint.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e641-131">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3e641-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e641-132">Response</span></span>
<span data-ttu-id="3e641-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3e641-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 3

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartPoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->