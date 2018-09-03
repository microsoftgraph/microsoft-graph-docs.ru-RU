# <a name="workbookrange-rowsabove"></a><span data-ttu-id="2526b-101">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="2526b-101">workbookRange: rowsAbove</span></span>

<span data-ttu-id="2526b-102">Возвращает определенное количество строк над заданным диапазоном.</span><span class="sxs-lookup"><span data-stu-id="2526b-102">Gets a certain number of rows above a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="2526b-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2526b-103">Permissions</span></span>
<span data-ttu-id="2526b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2526b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2526b-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2526b-106">Permission type</span></span>      | <span data-ttu-id="2526b-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2526b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2526b-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2526b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2526b-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2526b-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2526b-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2526b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2526b-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2526b-111">Not supported.</span></span>    |
|<span data-ttu-id="2526b-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2526b-112">Application</span></span> | <span data-ttu-id="2526b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2526b-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2526b-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2526b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="2526b-115">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="2526b-115">Function parameters</span></span>

| <span data-ttu-id="2526b-116">Параметр</span><span class="sxs-lookup"><span data-stu-id="2526b-116">Parameter</span></span>    | <span data-ttu-id="2526b-117">Тип</span><span class="sxs-lookup"><span data-stu-id="2526b-117">Type</span></span>   |<span data-ttu-id="2526b-118">Описание</span><span class="sxs-lookup"><span data-stu-id="2526b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2526b-119">count</span><span class="sxs-lookup"><span data-stu-id="2526b-119">count</span></span>|<span data-ttu-id="2526b-120">Int32</span><span class="sxs-lookup"><span data-stu-id="2526b-120">Int32</span></span>|<span data-ttu-id="2526b-p102">Необязательный. Количество строк, включаемых в полученный диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете использовать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="2526b-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="2526b-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2526b-126">Request headers</span></span>
| <span data-ttu-id="2526b-127">Имя</span><span class="sxs-lookup"><span data-stu-id="2526b-127">Name</span></span>       | <span data-ttu-id="2526b-128">Описание</span><span class="sxs-lookup"><span data-stu-id="2526b-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2526b-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2526b-129">Authorization</span></span>  | <span data-ttu-id="2526b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2526b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2526b-132">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2526b-132">Workbook-Session-Id</span></span>  | <span data-ttu-id="2526b-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="2526b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2526b-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2526b-135">Request body</span></span>
<span data-ttu-id="2526b-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2526b-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2526b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2526b-137">Response</span></span>
<span data-ttu-id="2526b-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2526b-138">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2526b-139">Пример</span><span class="sxs-lookup"><span data-stu-id="2526b-139">Example</span></span>
<span data-ttu-id="2526b-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2526b-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2526b-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="2526b-141">Request</span></span>
<span data-ttu-id="2526b-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2526b-142">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```

##### <a name="response"></a><span data-ttu-id="2526b-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="2526b-143">Response</span></span>
<span data-ttu-id="2526b-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2526b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="2526b-147">При вызове без дополнительного `count` параметра, эта функция возвращает одну строку над диапазоном.</span><span class="sxs-lookup"><span data-stu-id="2526b-147">If called without the optional `count` parameter, this function returns the single row above the range.</span></span>

##### <a name="request"></a><span data-ttu-id="2526b-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="2526b-148">Request</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove_nocount",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove
```

##### <a name="response"></a><span data-ttu-id="2526b-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="2526b-149">Response</span></span>
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