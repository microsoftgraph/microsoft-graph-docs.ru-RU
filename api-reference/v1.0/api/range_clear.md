# <a name="range-clear"></a><span data-ttu-id="aa233-101">Range: clear</span><span class="sxs-lookup"><span data-stu-id="aa233-101">Range: clear</span></span>

<span data-ttu-id="aa233-102">Очищает формат, заливку, границу, значения диапазона и т. д.</span><span class="sxs-lookup"><span data-stu-id="aa233-102">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="aa233-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa233-103">Permissions</span></span>
<span data-ttu-id="aa233-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aa233-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aa233-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa233-106">Permission type</span></span>      | <span data-ttu-id="aa233-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa233-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa233-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa233-108">Delegated (work or school account)</span></span> | <span data-ttu-id="aa233-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa233-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aa233-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa233-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa233-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa233-111">Not supported.</span></span>    |
|<span data-ttu-id="aa233-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa233-112">Application</span></span> | <span data-ttu-id="aa233-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa233-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa233-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa233-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/clear
GET /workbook/worksheets/{id|name}/range(address='<address>')/clear
GET /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="aa233-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa233-115">Request headers</span></span>
| <span data-ttu-id="aa233-116">Имя</span><span class="sxs-lookup"><span data-stu-id="aa233-116">Name</span></span>       | <span data-ttu-id="aa233-117">Описание</span><span class="sxs-lookup"><span data-stu-id="aa233-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aa233-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aa233-118">Authorization</span></span>  | <span data-ttu-id="aa233-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa233-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aa233-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="aa233-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="aa233-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="aa233-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa233-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa233-124">Request body</span></span>
<span data-ttu-id="aa233-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="aa233-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aa233-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="aa233-126">Parameter</span></span>    | <span data-ttu-id="aa233-127">Тип</span><span class="sxs-lookup"><span data-stu-id="aa233-127">Type</span></span>   |<span data-ttu-id="aa233-128">Описание</span><span class="sxs-lookup"><span data-stu-id="aa233-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa233-129">applyTo</span><span class="sxs-lookup"><span data-stu-id="aa233-129">applyTo</span></span>|<span data-ttu-id="aa233-130">string</span><span class="sxs-lookup"><span data-stu-id="aa233-130">string</span></span>|<span data-ttu-id="aa233-p104">Необязательный параметр. Определяет тип действия очистки.  Возможные значения: `All`, `Formats`, `Contents`.</span><span class="sxs-lookup"><span data-stu-id="aa233-p104">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="aa233-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa233-134">Response</span></span>

<span data-ttu-id="aa233-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="aa233-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa233-137">Пример</span><span class="sxs-lookup"><span data-stu-id="aa233-137">Example</span></span>
<span data-ttu-id="aa233-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="aa233-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="aa233-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa233-139">Request</span></span>
<span data-ttu-id="aa233-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa233-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <a name="response"></a><span data-ttu-id="aa233-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa233-141">Response</span></span>
<span data-ttu-id="aa233-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="aa233-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->