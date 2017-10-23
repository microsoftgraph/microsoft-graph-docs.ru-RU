# <a name="tablecolumn-delete"></a><span data-ttu-id="e585f-101">TableColumn: delete</span><span class="sxs-lookup"><span data-stu-id="e585f-101">TableColumn: delete</span></span>

<span data-ttu-id="e585f-102">Удаляет столбец из таблицы.</span><span class="sxs-lookup"><span data-stu-id="e585f-102">Deletes the column from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="e585f-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e585f-103">Permissions</span></span>
<span data-ttu-id="e585f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e585f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e585f-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e585f-106">Permission type</span></span>      | <span data-ttu-id="e585f-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e585f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e585f-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e585f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e585f-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e585f-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e585f-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e585f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e585f-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e585f-111">Not supported.</span></span>    |
|<span data-ttu-id="e585f-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e585f-112">Application</span></span> | <span data-ttu-id="e585f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e585f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e585f-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e585f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="e585f-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e585f-115">Request headers</span></span>
| <span data-ttu-id="e585f-116">Имя</span><span class="sxs-lookup"><span data-stu-id="e585f-116">Name</span></span>       | <span data-ttu-id="e585f-117">Описание</span><span class="sxs-lookup"><span data-stu-id="e585f-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e585f-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e585f-118">Authorization</span></span>  | <span data-ttu-id="e585f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e585f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e585f-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e585f-121">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e585f-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="e585f-122">Response</span></span>

<span data-ttu-id="e585f-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e585f-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e585f-125">Пример</span><span class="sxs-lookup"><span data-stu-id="e585f-125">Example</span></span>
<span data-ttu-id="e585f-126">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e585f-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e585f-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="e585f-127">Request</span></span>
<span data-ttu-id="e585f-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e585f-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumn_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/delete
```

##### <a name="response"></a><span data-ttu-id="e585f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e585f-129">Response</span></span>
<span data-ttu-id="e585f-130">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e585f-130">Here is an example of the response.</span></span> 
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
  "description": "TableColumn: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->