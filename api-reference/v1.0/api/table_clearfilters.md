# <a name="table-clearfilters"></a><span data-ttu-id="bd530-101">Table: clearFilters</span><span class="sxs-lookup"><span data-stu-id="bd530-101">Table: clearFilters</span></span>

<span data-ttu-id="bd530-102">Очищает все фильтры, примененные к таблице.</span><span class="sxs-lookup"><span data-stu-id="bd530-102">Clears all the filters currently applied on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="bd530-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd530-103">Permissions</span></span>
<span data-ttu-id="bd530-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bd530-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bd530-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd530-106">Permission type</span></span>      | <span data-ttu-id="bd530-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd530-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd530-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd530-108">Delegated (work or school account)</span></span> | <span data-ttu-id="bd530-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd530-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bd530-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd530-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd530-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd530-111">Not supported.</span></span>    |
|<span data-ttu-id="bd530-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd530-112">Application</span></span> | <span data-ttu-id="bd530-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd530-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd530-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd530-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/clearFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/clearFilters

```
## <a name="request-headers"></a><span data-ttu-id="bd530-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd530-115">Request headers</span></span>
| <span data-ttu-id="bd530-116">Имя</span><span class="sxs-lookup"><span data-stu-id="bd530-116">Name</span></span>       | <span data-ttu-id="bd530-117">Описание</span><span class="sxs-lookup"><span data-stu-id="bd530-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bd530-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd530-118">Authorization</span></span>  | <span data-ttu-id="bd530-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd530-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd530-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd530-121">Request body</span></span>

## <a name="response"></a><span data-ttu-id="bd530-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd530-122">Response</span></span>

<span data-ttu-id="bd530-p103">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bd530-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd530-125">Пример</span><span class="sxs-lookup"><span data-stu-id="bd530-125">Example</span></span>
<span data-ttu-id="bd530-126">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="bd530-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bd530-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd530-127">Request</span></span>
<span data-ttu-id="bd530-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd530-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_clearfilters"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters
```

##### <a name="response"></a><span data-ttu-id="bd530-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd530-129">Response</span></span>
<span data-ttu-id="bd530-130">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bd530-130">Here is an example of the response.</span></span> 
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
  "description": "Table: clearFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->