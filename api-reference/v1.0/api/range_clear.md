# <a name="range-clear"></a><span data-ttu-id="679af-101">Range: clear</span><span class="sxs-lookup"><span data-stu-id="679af-101">Range: clear</span></span>

<span data-ttu-id="679af-102">Очищает формат, заливку, границу, значения диапазона и т. д.</span><span class="sxs-lookup"><span data-stu-id="679af-102">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="679af-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="679af-103">Permissions</span></span>
<span data-ttu-id="679af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="679af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="679af-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="679af-106">Permission type</span></span>      | <span data-ttu-id="679af-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="679af-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="679af-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="679af-108">Delegated (work or school account)</span></span> | <span data-ttu-id="679af-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="679af-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="679af-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="679af-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="679af-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="679af-111">Not supported.</span></span>    |
|<span data-ttu-id="679af-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="679af-112">Application</span></span> | <span data-ttu-id="679af-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="679af-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="679af-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="679af-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/clear
GET /workbook/worksheets/{id|name}/range(address='<address>')/clear
GET /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="679af-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="679af-115">Request headers</span></span>
| <span data-ttu-id="679af-116">Имя</span><span class="sxs-lookup"><span data-stu-id="679af-116">Name</span></span>       | <span data-ttu-id="679af-117">Описание</span><span class="sxs-lookup"><span data-stu-id="679af-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="679af-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="679af-118">Authorization</span></span>  | <span data-ttu-id="679af-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="679af-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="679af-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="679af-121">Request body</span></span>
<span data-ttu-id="679af-122">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="679af-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="679af-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="679af-123">Parameter</span></span>    | <span data-ttu-id="679af-124">Тип</span><span class="sxs-lookup"><span data-stu-id="679af-124">Type</span></span>   |<span data-ttu-id="679af-125">Описание</span><span class="sxs-lookup"><span data-stu-id="679af-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="679af-126">applyTo</span><span class="sxs-lookup"><span data-stu-id="679af-126">applyTo</span></span>|<span data-ttu-id="679af-127">string</span><span class="sxs-lookup"><span data-stu-id="679af-127">string</span></span>|<span data-ttu-id="679af-p103">Необязательный параметр. Определяет тип действия очистки.  Возможные значения: `All`, `Formats`, `Contents`.</span><span class="sxs-lookup"><span data-stu-id="679af-p103">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="679af-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="679af-131">Response</span></span>

<span data-ttu-id="679af-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="679af-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="679af-134">Пример</span><span class="sxs-lookup"><span data-stu-id="679af-134">Example</span></span>
<span data-ttu-id="679af-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="679af-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="679af-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="679af-136">Request</span></span>
<span data-ttu-id="679af-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="679af-137">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="679af-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="679af-138">Response</span></span>
<span data-ttu-id="679af-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="679af-139">Here is an example of the response.</span></span> 
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