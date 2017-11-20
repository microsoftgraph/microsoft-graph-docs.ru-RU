# <a name="table-reapplyfilters"></a><span data-ttu-id="8219a-101">Table: reapplyFilters</span><span class="sxs-lookup"><span data-stu-id="8219a-101">Table: reapplyFilters</span></span>

<span data-ttu-id="8219a-102">Повторно применяет все текущие фильтры к таблице.</span><span class="sxs-lookup"><span data-stu-id="8219a-102">Reapplies all the filters currently on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="8219a-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8219a-103">Permissions</span></span>
<span data-ttu-id="8219a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8219a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8219a-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8219a-106">Permission type</span></span>      | <span data-ttu-id="8219a-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8219a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8219a-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8219a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8219a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8219a-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8219a-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8219a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8219a-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8219a-111">Not supported.</span></span>    |
|<span data-ttu-id="8219a-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8219a-112">Application</span></span> | <span data-ttu-id="8219a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8219a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8219a-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8219a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/reapplyFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/reapplyFilters

```
## <a name="request-headers"></a><span data-ttu-id="8219a-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8219a-115">Request headers</span></span>
| <span data-ttu-id="8219a-116">Имя</span><span class="sxs-lookup"><span data-stu-id="8219a-116">Name</span></span>       | <span data-ttu-id="8219a-117">Описание</span><span class="sxs-lookup"><span data-stu-id="8219a-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8219a-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8219a-118">Authorization</span></span>  | <span data-ttu-id="8219a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8219a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8219a-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8219a-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="8219a-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8219a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8219a-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8219a-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="8219a-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="8219a-125">Response</span></span>

<span data-ttu-id="8219a-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8219a-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8219a-128">Пример</span><span class="sxs-lookup"><span data-stu-id="8219a-128">Example</span></span>
<span data-ttu-id="8219a-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8219a-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8219a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8219a-130">Request</span></span>
<span data-ttu-id="8219a-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8219a-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_reapplyfilters"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/reapplyFilters
```

##### <a name="response"></a><span data-ttu-id="8219a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8219a-132">Response</span></span>
<span data-ttu-id="8219a-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8219a-133">Here is an example of the response.</span></span> 
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
  "description": "Table: reapplyFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->