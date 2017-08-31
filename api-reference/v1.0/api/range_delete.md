# <a name="range-delete"></a><span data-ttu-id="fc6ed-101">Range: delete</span><span class="sxs-lookup"><span data-stu-id="fc6ed-101">Range: delete</span></span>

<span data-ttu-id="fc6ed-102">Удаляет ячейки, связанные с диапазоном.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-102">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="fc6ed-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc6ed-103">Permissions</span></span>
<span data-ttu-id="fc6ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fc6ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fc6ed-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc6ed-106">Permission type</span></span>      | <span data-ttu-id="fc6ed-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc6ed-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc6ed-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc6ed-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fc6ed-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc6ed-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fc6ed-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc6ed-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc6ed-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-111">Not supported.</span></span>    |
|<span data-ttu-id="fc6ed-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc6ed-112">Application</span></span> | <span data-ttu-id="fc6ed-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc6ed-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc6ed-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(<address>)/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="fc6ed-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc6ed-115">Request headers</span></span>
| <span data-ttu-id="fc6ed-116">Имя</span><span class="sxs-lookup"><span data-stu-id="fc6ed-116">Name</span></span>       | <span data-ttu-id="fc6ed-117">Описание</span><span class="sxs-lookup"><span data-stu-id="fc6ed-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fc6ed-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc6ed-118">Authorization</span></span>  | <span data-ttu-id="fc6ed-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc6ed-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc6ed-121">Request body</span></span>
<span data-ttu-id="fc6ed-122">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fc6ed-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="fc6ed-123">Parameter</span></span>    | <span data-ttu-id="fc6ed-124">Тип</span><span class="sxs-lookup"><span data-stu-id="fc6ed-124">Type</span></span>   |<span data-ttu-id="fc6ed-125">Описание</span><span class="sxs-lookup"><span data-stu-id="fc6ed-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc6ed-126">shift</span><span class="sxs-lookup"><span data-stu-id="fc6ed-126">shift</span></span>|<span data-ttu-id="fc6ed-127">string</span><span class="sxs-lookup"><span data-stu-id="fc6ed-127">string</span></span>|<span data-ttu-id="fc6ed-p103">Указывает направление сдвига ячеек.  Возможные значения: `Up`, `Left`.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-p103">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="fc6ed-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc6ed-130">Response</span></span>

<span data-ttu-id="fc6ed-p104">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc6ed-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fc6ed-133">Example</span></span>
<span data-ttu-id="fc6ed-134">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fc6ed-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc6ed-135">Request</span></span>
<span data-ttu-id="fc6ed-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="fc6ed-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc6ed-137">Response</span></span>
<span data-ttu-id="fc6ed-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-138">Here is an example of the response.</span></span> 
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
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->