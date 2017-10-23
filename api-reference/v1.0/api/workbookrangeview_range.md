# <a name="workbookrangeview-range"></a><span data-ttu-id="8f57e-101">workbookRangeView: range</span><span class="sxs-lookup"><span data-stu-id="8f57e-101">workbookRangeView: range</span></span>
<span data-ttu-id="8f57e-102">Возвращение диапазона, связанного с ресурсом rangeView.</span><span class="sxs-lookup"><span data-stu-id="8f57e-102">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f57e-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f57e-103">Permissions</span></span>
<span data-ttu-id="8f57e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8f57e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="8f57e-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f57e-106">Permission type</span></span>      | <span data-ttu-id="8f57e-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f57e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f57e-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f57e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8f57e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f57e-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8f57e-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f57e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f57e-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f57e-111">Not supported.</span></span>    |
|<span data-ttu-id="8f57e-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f57e-112">Application</span></span> | <span data-ttu-id="8f57e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f57e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f57e-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f57e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="8f57e-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f57e-115">Request headers</span></span>
| <span data-ttu-id="8f57e-116">Имя</span><span class="sxs-lookup"><span data-stu-id="8f57e-116">Name</span></span>       | <span data-ttu-id="8f57e-117">Описание</span><span class="sxs-lookup"><span data-stu-id="8f57e-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8f57e-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f57e-118">Authorization</span></span>  | <span data-ttu-id="8f57e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f57e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f57e-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8f57e-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="8f57e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8f57e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f57e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f57e-124">Request body</span></span>

### <a name="response"></a><span data-ttu-id="8f57e-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f57e-125">Response</span></span>
<span data-ttu-id="8f57e-126">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8f57e-126">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f57e-127">Пример</span><span class="sxs-lookup"><span data-stu-id="8f57e-127">Example</span></span>
<span data-ttu-id="8f57e-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8f57e-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8f57e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f57e-129">Request</span></span>
<span data-ttu-id="8f57e-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f57e-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/range
```

##### <a name="response"></a><span data-ttu-id="8f57e-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f57e-131">Response</span></span>
<span data-ttu-id="8f57e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8f57e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
