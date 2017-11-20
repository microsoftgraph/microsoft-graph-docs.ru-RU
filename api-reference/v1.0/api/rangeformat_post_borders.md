# <a name="create-rangeborder"></a><span data-ttu-id="3d999-101">Создание объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="3d999-101">Create RangeBorder</span></span>

<span data-ttu-id="3d999-102">С помощью этого API можно создать объект RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="3d999-102">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="3d999-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d999-103">Permissions</span></span>
<span data-ttu-id="3d999-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3d999-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3d999-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d999-106">Permission type</span></span>      | <span data-ttu-id="3d999-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d999-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d999-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d999-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3d999-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d999-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3d999-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d999-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d999-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d999-111">Not supported.</span></span>    |
|<span data-ttu-id="3d999-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d999-112">Application</span></span> | <span data-ttu-id="3d999-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d999-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d999-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d999-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="3d999-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d999-115">Request headers</span></span>
| <span data-ttu-id="3d999-116">Имя</span><span class="sxs-lookup"><span data-stu-id="3d999-116">Name</span></span>       | <span data-ttu-id="3d999-117">Описание</span><span class="sxs-lookup"><span data-stu-id="3d999-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3d999-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d999-118">Authorization</span></span>  | <span data-ttu-id="3d999-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d999-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3d999-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3d999-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="3d999-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="3d999-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d999-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d999-124">Request body</span></span>
<span data-ttu-id="3d999-125">Предоставьте в тексте запроса описание объекта [RangeBorder](../resources/rangeborder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d999-125">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3d999-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d999-126">Response</span></span>

<span data-ttu-id="3d999-127">В случае успеха этот метод возвращает код отклика `201 Created` и объект [RangeBorder](../resources/rangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3d999-127">If successful, this method returns `201 Created` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d999-128">Пример</span><span class="sxs-lookup"><span data-stu-id="3d999-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d999-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d999-129">Request</span></span>
<span data-ttu-id="3d999-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d999-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/borders
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
<span data-ttu-id="3d999-131">Предоставьте в тексте запроса описание объекта [RangeBorder](../resources/rangeborder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d999-131">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3d999-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d999-132">Response</span></span>
<span data-ttu-id="3d999-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3d999-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
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