# <a name="workbookrange-visibleview"></a><span data-ttu-id="531c5-101">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="531c5-101">workbookRange: visibleView</span></span>


## <a name="permissions"></a><span data-ttu-id="531c5-102">Разрешения</span><span class="sxs-lookup"><span data-stu-id="531c5-102">Permissions</span></span>
<span data-ttu-id="531c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="531c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="531c5-105">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="531c5-105">Permission type</span></span>      | <span data-ttu-id="531c5-106">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="531c5-106">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="531c5-107">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="531c5-107">Delegated (work or school account)</span></span> | <span data-ttu-id="531c5-108">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="531c5-108">Files.ReadWrite</span></span>    |
|<span data-ttu-id="531c5-109">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="531c5-109">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="531c5-110">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="531c5-110">Not supported.</span></span>    |
|<span data-ttu-id="531c5-111">Для приложений</span><span class="sxs-lookup"><span data-stu-id="531c5-111">Application</span></span> | <span data-ttu-id="531c5-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="531c5-112">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="531c5-113">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="531c5-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="531c5-114">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="531c5-114">Request headers</span></span>
| <span data-ttu-id="531c5-115">Имя</span><span class="sxs-lookup"><span data-stu-id="531c5-115">Name</span></span>       | <span data-ttu-id="531c5-116">Описание</span><span class="sxs-lookup"><span data-stu-id="531c5-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="531c5-117">Авторизация</span><span class="sxs-lookup"><span data-stu-id="531c5-117">Authorization</span></span>  | <span data-ttu-id="531c5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="531c5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="531c5-120">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="531c5-120">Workbook-Session-Id</span></span>  | <span data-ttu-id="531c5-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="531c5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="531c5-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="531c5-123">Request body</span></span>

### <a name="response"></a><span data-ttu-id="531c5-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="531c5-124">Response</span></span>
<span data-ttu-id="531c5-125">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="531c5-125">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="531c5-126">Пример</span><span class="sxs-lookup"><span data-stu-id="531c5-126">Example</span></span>
<span data-ttu-id="531c5-127">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="531c5-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="531c5-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="531c5-128">Request</span></span>
<span data-ttu-id="531c5-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="531c5-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView
```

##### <a name="response"></a><span data-ttu-id="531c5-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="531c5-130">Response</span></span>
<span data-ttu-id="531c5-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="531c5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "cellAddresses": "cellAddresses-value",
  "columnCount": 99,
  "formulas": "formulas-value",
  "formulasLocal": "formulasLocal-value",
  "formulasR1C1": "formulasR1C1-value",
  "index": 99
}
```