# <a name="create-table"></a><span data-ttu-id="9a130-101">Создание объекта Table</span><span class="sxs-lookup"><span data-stu-id="9a130-101">Create Table</span></span>

<span data-ttu-id="9a130-102">С помощью этого API можно создать объект Table.</span><span class="sxs-lookup"><span data-stu-id="9a130-102">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a130-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a130-103">Permissions</span></span>
<span data-ttu-id="9a130-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a130-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9a130-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a130-106">Permission type</span></span>      | <span data-ttu-id="9a130-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a130-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a130-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a130-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9a130-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a130-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9a130-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a130-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a130-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a130-111">Not supported.</span></span>    |
|<span data-ttu-id="9a130-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a130-112">Application</span></span> | <span data-ttu-id="9a130-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a130-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a130-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a130-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/$/add

```
## <a name="request-headers"></a><span data-ttu-id="9a130-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a130-115">Request headers</span></span>
| <span data-ttu-id="9a130-116">Имя</span><span class="sxs-lookup"><span data-stu-id="9a130-116">Name</span></span>       | <span data-ttu-id="9a130-117">Описание</span><span class="sxs-lookup"><span data-stu-id="9a130-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9a130-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a130-118">Authorization</span></span>  | <span data-ttu-id="9a130-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a130-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a130-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a130-121">Request body</span></span>
<span data-ttu-id="9a130-122">Предоставьте в тексте запроса описание объекта [Table](../resources/table.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a130-122">In the request body, supply a JSON representation of [Table](../resources/table.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9a130-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a130-123">Response</span></span>

<span data-ttu-id="9a130-124">В случае успеха этот метод возвращает код ответа `201 Created` и объект [Table](../resources/table.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9a130-124">If successful, this method returns `201 Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a130-125">Пример</span><span class="sxs-lookup"><span data-stu-id="9a130-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a130-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a130-126">Request</span></span>
<span data-ttu-id="9a130-127">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a130-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_workbook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/$/add
Content-type: application/json
Content-length: 109

{
  "id": 99,
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
<span data-ttu-id="9a130-128">Предоставьте в тексте запроса описание объекта [Table](../resources/table.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a130-128">In the request body, supply a JSON representation of [Table](../resources/table.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9a130-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a130-129">Response</span></span>
<span data-ttu-id="9a130-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9a130-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
