# <a name="filter-clear"></a><span data-ttu-id="9d55c-101">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="9d55c-101">Filter: clear</span></span>

<span data-ttu-id="9d55c-102">Сброс фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="9d55c-102">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="9d55c-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d55c-103">Permissions</span></span>
<span data-ttu-id="9d55c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9d55c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9d55c-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d55c-106">Permission type</span></span>      | <span data-ttu-id="9d55c-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d55c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d55c-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d55c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9d55c-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d55c-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9d55c-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d55c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d55c-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d55c-111">Not supported.</span></span>    |
|<span data-ttu-id="9d55c-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d55c-112">Application</span></span> | <span data-ttu-id="9d55c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d55c-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d55c-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d55c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="9d55c-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d55c-115">Request headers</span></span>
| <span data-ttu-id="9d55c-116">Имя</span><span class="sxs-lookup"><span data-stu-id="9d55c-116">Name</span></span>       | <span data-ttu-id="9d55c-117">Описание</span><span class="sxs-lookup"><span data-stu-id="9d55c-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9d55c-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d55c-118">Authorization</span></span>  | <span data-ttu-id="9d55c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d55c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d55c-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d55c-121">Request body</span></span>
<span data-ttu-id="9d55c-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9d55c-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d55c-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d55c-123">Response</span></span>

<span data-ttu-id="9d55c-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9d55c-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d55c-126">Пример</span><span class="sxs-lookup"><span data-stu-id="9d55c-126">Example</span></span>
<span data-ttu-id="9d55c-127">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9d55c-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9d55c-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d55c-128">Request</span></span>
<span data-ttu-id="9d55c-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d55c-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <a name="response"></a><span data-ttu-id="9d55c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d55c-130">Response</span></span>
<span data-ttu-id="9d55c-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9d55c-131">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
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