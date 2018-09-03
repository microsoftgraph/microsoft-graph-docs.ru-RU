# <a name="workbookrange-columnsafter"></a><span data-ttu-id="74e60-101">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="74e60-101">workbookRange: columnsAfter</span></span>

<span data-ttu-id="74e60-102">Возвращает определенное количество столбцов справа от заданного диапазона.</span><span class="sxs-lookup"><span data-stu-id="74e60-102">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="74e60-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74e60-103">Permissions</span></span>
<span data-ttu-id="74e60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="74e60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="74e60-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74e60-106">Permission type</span></span>      | <span data-ttu-id="74e60-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74e60-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74e60-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74e60-108">Delegated (work or school account)</span></span> | <span data-ttu-id="74e60-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74e60-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="74e60-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74e60-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74e60-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74e60-111">Not supported.</span></span>    |
|<span data-ttu-id="74e60-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74e60-112">Application</span></span> | <span data-ttu-id="74e60-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74e60-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="74e60-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74e60-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="74e60-115">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="74e60-115">Function parameters</span></span>

| <span data-ttu-id="74e60-116">Параметр</span><span class="sxs-lookup"><span data-stu-id="74e60-116">Parameter</span></span>    | <span data-ttu-id="74e60-117">Тип</span><span class="sxs-lookup"><span data-stu-id="74e60-117">Type</span></span>   |<span data-ttu-id="74e60-118">Описание</span><span class="sxs-lookup"><span data-stu-id="74e60-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74e60-119">count</span><span class="sxs-lookup"><span data-stu-id="74e60-119">count</span></span>|<span data-ttu-id="74e60-120">Int32</span><span class="sxs-lookup"><span data-stu-id="74e60-120">Int32</span></span>|<span data-ttu-id="74e60-121">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="74e60-121">Optional.</span></span> <span data-ttu-id="74e60-122">Количество столбцов для включения в результирующий диапазон.</span><span class="sxs-lookup"><span data-stu-id="74e60-122">The number of rows to include in the resulting range.</span></span> <span data-ttu-id="74e60-123">В общем случае используйте положительное число для создания нового диапазона за пределами текущего.</span><span class="sxs-lookup"><span data-stu-id="74e60-123">In general, use a positive number to create a range outside the current range.</span></span> <span data-ttu-id="74e60-124">Отрицательное число можно использовать для создания нового диапазона в текущем.</span><span class="sxs-lookup"><span data-stu-id="74e60-124">You can also use a negative number to create a range within the current range.</span></span> <span data-ttu-id="74e60-125">1 — значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="74e60-125">The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="74e60-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74e60-126">Request headers</span></span>
| <span data-ttu-id="74e60-127">Имя</span><span class="sxs-lookup"><span data-stu-id="74e60-127">Name</span></span>       | <span data-ttu-id="74e60-128">Описание</span><span class="sxs-lookup"><span data-stu-id="74e60-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="74e60-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74e60-129">Authorization</span></span>  | <span data-ttu-id="74e60-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74e60-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="74e60-132">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="74e60-132">Workbook-Session-Id</span></span>  | <span data-ttu-id="74e60-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="74e60-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="74e60-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74e60-135">Request body</span></span>
<span data-ttu-id="74e60-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="74e60-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74e60-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="74e60-137">Response</span></span>
<span data-ttu-id="74e60-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="74e60-138">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74e60-139">Пример</span><span class="sxs-lookup"><span data-stu-id="74e60-139">Example</span></span>
<span data-ttu-id="74e60-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="74e60-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="74e60-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="74e60-141">Request</span></span>
<span data-ttu-id="74e60-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74e60-142">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_columnsafter",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```

##### <a name="response"></a><span data-ttu-id="74e60-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="74e60-143">Response</span></span>
<span data-ttu-id="74e60-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="74e60-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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
