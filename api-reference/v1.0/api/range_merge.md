# <a name="range-merge"></a><span data-ttu-id="33b37-101">Range: merge</span><span class="sxs-lookup"><span data-stu-id="33b37-101">Range: merge</span></span>

<span data-ttu-id="33b37-102">Объединяет ячейки диапазона в одну область на листе.</span><span class="sxs-lookup"><span data-stu-id="33b37-102">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="33b37-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33b37-103">Permissions</span></span>
<span data-ttu-id="33b37-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="33b37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="33b37-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33b37-106">Permission type</span></span>      | <span data-ttu-id="33b37-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33b37-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33b37-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33b37-108">Delegated (work or school account)</span></span> | <span data-ttu-id="33b37-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33b37-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="33b37-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33b37-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33b37-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33b37-111">Not supported.</span></span>    |
|<span data-ttu-id="33b37-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33b37-112">Application</span></span> | <span data-ttu-id="33b37-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33b37-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="33b37-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33b37-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/merge
POST /workbook/worksheets/{id|name}/range(<address>)/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="33b37-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33b37-115">Request headers</span></span>
| <span data-ttu-id="33b37-116">Имя</span><span class="sxs-lookup"><span data-stu-id="33b37-116">Name</span></span>       | <span data-ttu-id="33b37-117">Описание</span><span class="sxs-lookup"><span data-stu-id="33b37-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="33b37-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33b37-118">Authorization</span></span>  | <span data-ttu-id="33b37-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33b37-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33b37-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33b37-121">Request body</span></span>
<span data-ttu-id="33b37-122">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="33b37-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="33b37-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="33b37-123">Parameter</span></span>    | <span data-ttu-id="33b37-124">Тип</span><span class="sxs-lookup"><span data-stu-id="33b37-124">Type</span></span>   |<span data-ttu-id="33b37-125">Описание</span><span class="sxs-lookup"><span data-stu-id="33b37-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33b37-126">across</span><span class="sxs-lookup"><span data-stu-id="33b37-126">across</span></span>|<span data-ttu-id="33b37-127">boolean</span><span class="sxs-lookup"><span data-stu-id="33b37-127">boolean</span></span>|<span data-ttu-id="33b37-p103">Необязательный параметр. Установите значение true, чтобы объединить ячейки в каждой строке заданного диапазона как отдельные объединенные ячейки. Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="33b37-p103">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="33b37-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="33b37-131">Response</span></span>

<span data-ttu-id="33b37-p104">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="33b37-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33b37-134">Пример</span><span class="sxs-lookup"><span data-stu-id="33b37-134">Example</span></span>
<span data-ttu-id="33b37-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="33b37-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="33b37-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="33b37-136">Request</span></span>
<span data-ttu-id="33b37-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33b37-137">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="33b37-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="33b37-138">Response</span></span>
<span data-ttu-id="33b37-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="33b37-139">Here is an example of the response.</span></span> 
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