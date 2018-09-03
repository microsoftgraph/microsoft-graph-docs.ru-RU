# <a name="workbookrange-rowsabove"></a><span data-ttu-id="f5318-101">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="f5318-101">workbookRange: rowsAbove</span></span>

<span data-ttu-id="f5318-102">Возвращает определенное количество строк над заданным диапазоном.</span><span class="sxs-lookup"><span data-stu-id="f5318-102">Gets a certain number of rows above a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5318-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5318-103">Permissions</span></span>
<span data-ttu-id="f5318-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f5318-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f5318-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5318-106">Permission type</span></span>      | <span data-ttu-id="f5318-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5318-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5318-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5318-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f5318-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5318-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f5318-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5318-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5318-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5318-111">Not supported.</span></span>    |
|<span data-ttu-id="f5318-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5318-112">Application</span></span> | <span data-ttu-id="f5318-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5318-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5318-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5318-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=n)

```
## <a name="request-headers"></a><span data-ttu-id="f5318-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5318-115">Request headers</span></span>
| <span data-ttu-id="f5318-116">Имя</span><span class="sxs-lookup"><span data-stu-id="f5318-116">Name</span></span>       | <span data-ttu-id="f5318-117">Описание</span><span class="sxs-lookup"><span data-stu-id="f5318-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f5318-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5318-118">Authorization</span></span>  | <span data-ttu-id="f5318-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5318-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5318-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f5318-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="f5318-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f5318-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="f5318-124">Параметры</span><span class="sxs-lookup"><span data-stu-id="f5318-124">Parameters</span></span>

| <span data-ttu-id="f5318-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="f5318-125">Parameter</span></span>    | <span data-ttu-id="f5318-126">Тип</span><span class="sxs-lookup"><span data-stu-id="f5318-126">Type</span></span>   |<span data-ttu-id="f5318-127">Описание</span><span class="sxs-lookup"><span data-stu-id="f5318-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5318-128">count</span><span class="sxs-lookup"><span data-stu-id="f5318-128">count</span></span>|<span data-ttu-id="f5318-129">Int32</span><span class="sxs-lookup"><span data-stu-id="f5318-129">Int32</span></span>|<span data-ttu-id="f5318-130">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f5318-130">Optional.</span></span> <span data-ttu-id="f5318-131">Количество строк для включения в результирующий диапазон.</span><span class="sxs-lookup"><span data-stu-id="f5318-131">The number of rows to include in the resulting range.</span></span> <span data-ttu-id="f5318-132">В общем случае используйте положительное число для создания нового диапазона за пределами текущего.</span><span class="sxs-lookup"><span data-stu-id="f5318-132">In general, use a positive number to create a range outside the current range.</span></span> <span data-ttu-id="f5318-133">Отрицательное число можно использовать для создания нового диапазона в текущем.</span><span class="sxs-lookup"><span data-stu-id="f5318-133">You can also use a negative number to create a range within the current range.</span></span> <span data-ttu-id="f5318-134">1 — значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="f5318-134">The default value is 1.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5318-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5318-135">Request body</span></span>

### <a name="response"></a><span data-ttu-id="f5318-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5318-136">Response</span></span>
<span data-ttu-id="f5318-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f5318-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5318-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f5318-138">Example</span></span>
<span data-ttu-id="f5318-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f5318-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f5318-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5318-140">Request</span></span>
<span data-ttu-id="f5318-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5318-141">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```

##### <a name="response"></a><span data-ttu-id="f5318-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="f5318-142">Response</span></span>
<span data-ttu-id="f5318-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f5318-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="f5318-146">При вызове без дополнительного `count` параметра, эта функция возвращает одну строку над диапазоном.</span><span class="sxs-lookup"><span data-stu-id="f5318-146">If called without the optional `count` parameter, this function returns the single row above the range.</span></span>

##### <a name="request"></a><span data-ttu-id="f5318-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5318-147">Request</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove_nocount",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove
```

##### <a name="response"></a><span data-ttu-id="f5318-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="f5318-148">Response</span></span>
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