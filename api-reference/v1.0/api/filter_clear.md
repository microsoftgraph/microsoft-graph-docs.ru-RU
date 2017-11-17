# <a name="filter-clear"></a><span data-ttu-id="d8759-101">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="d8759-101">Filter: clear</span></span>

<span data-ttu-id="d8759-102">Сброс фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="d8759-102">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="d8759-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8759-103">Permissions</span></span>
<span data-ttu-id="d8759-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d8759-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d8759-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8759-106">Permission type</span></span>      | <span data-ttu-id="d8759-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8759-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8759-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8759-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d8759-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8759-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d8759-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8759-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8759-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8759-111">Not supported.</span></span>    |
|<span data-ttu-id="d8759-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8759-112">Application</span></span> | <span data-ttu-id="d8759-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8759-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8759-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8759-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="d8759-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8759-115">Request headers</span></span>
| <span data-ttu-id="d8759-116">Имя</span><span class="sxs-lookup"><span data-stu-id="d8759-116">Name</span></span>       | <span data-ttu-id="d8759-117">Описание</span><span class="sxs-lookup"><span data-stu-id="d8759-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d8759-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8759-118">Authorization</span></span>  | <span data-ttu-id="d8759-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8759-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8759-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8759-121">Request body</span></span>
<span data-ttu-id="d8759-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8759-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8759-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8759-123">Response</span></span>

<span data-ttu-id="d8759-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d8759-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8759-126">Пример</span><span class="sxs-lookup"><span data-stu-id="d8759-126">Example</span></span>
<span data-ttu-id="d8759-127">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d8759-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d8759-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8759-128">Request</span></span>
<span data-ttu-id="d8759-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8759-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <a name="response"></a><span data-ttu-id="d8759-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8759-130">Response</span></span>
<span data-ttu-id="d8759-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d8759-131">Here is an example of the response.</span></span> 
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
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->