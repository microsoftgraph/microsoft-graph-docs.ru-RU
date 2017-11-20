# <a name="rangeformat-autofitrows"></a><span data-ttu-id="49b60-101">RangeFormat: autofitRows</span><span class="sxs-lookup"><span data-stu-id="49b60-101">RangeFormat: autofitRows</span></span>

<span data-ttu-id="49b60-102">Изменяет высоту строк текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="49b60-102">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="49b60-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49b60-103">Permissions</span></span>
<span data-ttu-id="49b60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="49b60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="49b60-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49b60-106">Permission type</span></span>      | <span data-ttu-id="49b60-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49b60-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49b60-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49b60-108">Delegated (work or school account)</span></span> | <span data-ttu-id="49b60-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49b60-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="49b60-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49b60-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49b60-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49b60-111">Not supported.</span></span>    |
|<span data-ttu-id="49b60-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49b60-112">Application</span></span> | <span data-ttu-id="49b60-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49b60-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49b60-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49b60-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/autofitRows
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitRows
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitRows

```
## <a name="request-headers"></a><span data-ttu-id="49b60-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49b60-115">Request headers</span></span>
| <span data-ttu-id="49b60-116">Имя</span><span class="sxs-lookup"><span data-stu-id="49b60-116">Name</span></span>       | <span data-ttu-id="49b60-117">Описание</span><span class="sxs-lookup"><span data-stu-id="49b60-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="49b60-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49b60-118">Authorization</span></span>  | <span data-ttu-id="49b60-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49b60-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="49b60-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="49b60-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="49b60-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="49b60-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49b60-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49b60-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="49b60-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="49b60-125">Response</span></span>

<span data-ttu-id="49b60-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="49b60-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49b60-128">Пример</span><span class="sxs-lookup"><span data-stu-id="49b60-128">Example</span></span>
<span data-ttu-id="49b60-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="49b60-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="49b60-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="49b60-130">Request</span></span>
<span data-ttu-id="49b60-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49b60-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitrows"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/autofitRows
```

##### <a name="response"></a><span data-ttu-id="49b60-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="49b60-132">Response</span></span>
<span data-ttu-id="49b60-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="49b60-133">Here is an example of the response.</span></span> 
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
  "description": "RangeFormat: autofitRows",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->