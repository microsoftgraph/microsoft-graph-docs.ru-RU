# <a name="create-rangeborder"></a><span data-ttu-id="e06a8-101">Создание объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="e06a8-101">Create RangeBorder</span></span>

<span data-ttu-id="e06a8-102">С помощью этого API можно создать объект RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="e06a8-102">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="e06a8-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e06a8-103">Permissions</span></span>
<span data-ttu-id="e06a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e06a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e06a8-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e06a8-106">Permission type</span></span>      | <span data-ttu-id="e06a8-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e06a8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e06a8-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e06a8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e06a8-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e06a8-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e06a8-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e06a8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e06a8-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e06a8-111">Not supported.</span></span>    |
|<span data-ttu-id="e06a8-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e06a8-112">Application</span></span> | <span data-ttu-id="e06a8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e06a8-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e06a8-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e06a8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/borders
POST /workbook/worksheets/{id|name}/range(<address>)/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="e06a8-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e06a8-115">Request headers</span></span>
| <span data-ttu-id="e06a8-116">Имя</span><span class="sxs-lookup"><span data-stu-id="e06a8-116">Name</span></span>       | <span data-ttu-id="e06a8-117">Описание</span><span class="sxs-lookup"><span data-stu-id="e06a8-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e06a8-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e06a8-118">Authorization</span></span>  | <span data-ttu-id="e06a8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e06a8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e06a8-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e06a8-121">Request body</span></span>
<span data-ttu-id="e06a8-122">Предоставьте в тексте запроса описание объекта [RangeBorder](../resources/rangeborder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e06a8-122">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e06a8-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="e06a8-123">Response</span></span>

<span data-ttu-id="e06a8-124">В случае успеха этот метод возвращает код отклика `201, Created` и объект [RangeBorder](../resources/rangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e06a8-124">If successful, this method returns `201, Created` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e06a8-125">Пример</span><span class="sxs-lookup"><span data-stu-id="e06a8-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e06a8-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="e06a8-126">Request</span></span>
<span data-ttu-id="e06a8-127">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e06a8-127">Here is an example of the request.</span></span>
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
<span data-ttu-id="e06a8-128">Предоставьте в тексте запроса описание объекта [RangeBorder](../resources/rangeborder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e06a8-128">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e06a8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e06a8-129">Response</span></span>
<span data-ttu-id="e06a8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e06a8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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