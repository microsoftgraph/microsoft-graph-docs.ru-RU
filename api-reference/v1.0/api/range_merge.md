# <a name="range-merge"></a><span data-ttu-id="fc6aa-101">Range: merge</span><span class="sxs-lookup"><span data-stu-id="fc6aa-101">Range: merge</span></span>

<span data-ttu-id="fc6aa-102">Объединяет ячейки диапазона в одну область на листе.</span><span class="sxs-lookup"><span data-stu-id="fc6aa-102">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="fc6aa-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc6aa-103">Permissions</span></span>
<span data-ttu-id="fc6aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fc6aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fc6aa-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc6aa-106">Permission type</span></span>      | <span data-ttu-id="fc6aa-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc6aa-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc6aa-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc6aa-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fc6aa-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc6aa-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fc6aa-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc6aa-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc6aa-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc6aa-111">Not supported.</span></span>    |
|<span data-ttu-id="fc6aa-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc6aa-112">Application</span></span> | <span data-ttu-id="fc6aa-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc6aa-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc6aa-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc6aa-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="fc6aa-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc6aa-115">Request headers</span></span>
| <span data-ttu-id="fc6aa-116">Имя</span><span class="sxs-lookup"><span data-stu-id="fc6aa-116">Name</span></span>       | <span data-ttu-id="fc6aa-117">Описание</span><span class="sxs-lookup"><span data-stu-id="fc6aa-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fc6aa-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc6aa-118">Authorization</span></span>  | <span data-ttu-id="fc6aa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc6aa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc6aa-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fc6aa-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="fc6aa-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="fc6aa-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc6aa-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc6aa-124">Request body</span></span>
<span data-ttu-id="fc6aa-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="fc6aa-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fc6aa-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="fc6aa-126">Parameter</span></span>    | <span data-ttu-id="fc6aa-127">Тип</span><span class="sxs-lookup"><span data-stu-id="fc6aa-127">Type</span></span>   |<span data-ttu-id="fc6aa-128">Описание</span><span class="sxs-lookup"><span data-stu-id="fc6aa-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc6aa-129">across</span><span class="sxs-lookup"><span data-stu-id="fc6aa-129">across</span></span>|<span data-ttu-id="fc6aa-130">boolean</span><span class="sxs-lookup"><span data-stu-id="fc6aa-130">boolean</span></span>|<span data-ttu-id="fc6aa-p104">Необязательный параметр. Установите значение true, чтобы объединить ячейки в каждой строке заданного диапазона как отдельные объединенные ячейки. Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="fc6aa-p104">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="fc6aa-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc6aa-134">Response</span></span>

<span data-ttu-id="fc6aa-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="fc6aa-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc6aa-137">Пример</span><span class="sxs-lookup"><span data-stu-id="fc6aa-137">Example</span></span>
<span data-ttu-id="fc6aa-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="fc6aa-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fc6aa-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc6aa-139">Request</span></span>
<span data-ttu-id="fc6aa-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc6aa-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="fc6aa-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc6aa-141">Response</span></span>
<span data-ttu-id="fc6aa-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fc6aa-142">Here is an example of the response.</span></span> 
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
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->