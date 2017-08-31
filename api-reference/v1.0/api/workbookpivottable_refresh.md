# <a name="workbookpivottable-refresh"></a><span data-ttu-id="75403-101">workbookPivotTable: refresh</span><span class="sxs-lookup"><span data-stu-id="75403-101">workbookPivotTable: refresh</span></span>

<span data-ttu-id="75403-102">Обновляет сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="75403-102">Refreshes the PivotTable.</span></span>


## <a name="permissions"></a><span data-ttu-id="75403-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75403-103">Permissions</span></span>
<span data-ttu-id="75403-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="75403-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="75403-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75403-106">Permission type</span></span>      | <span data-ttu-id="75403-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75403-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75403-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75403-108">Delegated (work or school account)</span></span> | <span data-ttu-id="75403-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75403-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="75403-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75403-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75403-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75403-111">Not supported.</span></span>    |
|<span data-ttu-id="75403-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75403-112">Application</span></span> | <span data-ttu-id="75403-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75403-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75403-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75403-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a><span data-ttu-id="75403-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75403-115">Request headers</span></span>
| <span data-ttu-id="75403-116">Имя</span><span class="sxs-lookup"><span data-stu-id="75403-116">Name</span></span>       | <span data-ttu-id="75403-117">Описание</span><span class="sxs-lookup"><span data-stu-id="75403-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="75403-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75403-118">Authorization</span></span>  | <span data-ttu-id="75403-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75403-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="75403-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="75403-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="75403-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="75403-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75403-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75403-124">Request body</span></span>

### <a name="response"></a><span data-ttu-id="75403-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="75403-125">Response</span></span>
<span data-ttu-id="75403-p104">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="75403-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75403-128">Пример</span><span class="sxs-lookup"><span data-stu-id="75403-128">Example</span></span>
<span data-ttu-id="75403-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="75403-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="75403-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="75403-130">Request</span></span>
<span data-ttu-id="75403-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75403-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```

##### <a name="response"></a><span data-ttu-id="75403-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="75403-132">Response</span></span>
<span data-ttu-id="75403-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="75403-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
