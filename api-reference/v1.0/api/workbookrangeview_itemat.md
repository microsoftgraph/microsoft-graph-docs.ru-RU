# <a name="workbookrangeview-itemat"></a><span data-ttu-id="8a093-101">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="8a093-101">workbookRangeView: itemAt</span></span>


## <a name="permissions"></a><span data-ttu-id="8a093-102">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a093-102">Permissions</span></span>
<span data-ttu-id="8a093-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8a093-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8a093-105">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a093-105">Permission type</span></span>      | <span data-ttu-id="8a093-106">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a093-106">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a093-107">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a093-107">Delegated (work or school account)</span></span> | <span data-ttu-id="8a093-108">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a093-108">Files.ReadWrite</span></span> |
|<span data-ttu-id="8a093-109">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a093-109">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a093-110">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a093-110">Not supported.</span></span>    |
|<span data-ttu-id="8a093-111">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a093-111">Application</span></span> | <span data-ttu-id="8a093-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a093-112">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a093-113">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a093-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="8a093-114">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a093-114">Request headers</span></span>
| <span data-ttu-id="8a093-115">Имя</span><span class="sxs-lookup"><span data-stu-id="8a093-115">Name</span></span>       | <span data-ttu-id="8a093-116">Описание</span><span class="sxs-lookup"><span data-stu-id="8a093-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8a093-117">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a093-117">Authorization</span></span>  | <span data-ttu-id="8a093-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a093-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8a093-120">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8a093-120">Workbook-Session-Id</span></span>  | <span data-ttu-id="8a093-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8a093-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a093-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a093-123">Request body</span></span>
<span data-ttu-id="8a093-124">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="8a093-124">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="8a093-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="8a093-125">Parameter</span></span>    | <span data-ttu-id="8a093-126">Тип</span><span class="sxs-lookup"><span data-stu-id="8a093-126">Type</span></span>   |<span data-ttu-id="8a093-127">Описание</span><span class="sxs-lookup"><span data-stu-id="8a093-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a093-128">index</span><span class="sxs-lookup"><span data-stu-id="8a093-128">index</span></span>|<span data-ttu-id="8a093-129">Int32</span><span class="sxs-lookup"><span data-stu-id="8a093-129">Int32</span></span>|<span data-ttu-id="8a093-130">Индекс элемента, который нужно вернуть.</span><span class="sxs-lookup"><span data-stu-id="8a093-130">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="8a093-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a093-131">Response</span></span>

<span data-ttu-id="8a093-132">В случае успеха этот метод возвращает код отклика `200, OK` и объект [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8a093-132">If successful, this method returns `200, OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a093-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8a093-133">Example</span></span>
<span data-ttu-id="8a093-134">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8a093-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8a093-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a093-135">Request</span></span>
<span data-ttu-id="8a093-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a093-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="8a093-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a093-137">Response</span></span>
<span data-ttu-id="8a093-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8a093-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
