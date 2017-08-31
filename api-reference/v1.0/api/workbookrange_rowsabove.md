# <a name="workbookrange-rowsabove"></a><span data-ttu-id="ae6b8-101">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="ae6b8-101">workbookRange: rowsAbove</span></span>

<span data-ttu-id="ae6b8-102">Возвращает определенное количество строк над заданным диапазоном.</span><span class="sxs-lookup"><span data-stu-id="ae6b8-102">Gets a certain number of rows above a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae6b8-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae6b8-103">Permissions</span></span>
<span data-ttu-id="ae6b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae6b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ae6b8-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae6b8-106">Permission type</span></span>      | <span data-ttu-id="ae6b8-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae6b8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae6b8-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae6b8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ae6b8-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae6b8-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ae6b8-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae6b8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae6b8-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae6b8-111">Not supported.</span></span>    |
|<span data-ttu-id="ae6b8-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae6b8-112">Application</span></span> | <span data-ttu-id="ae6b8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae6b8-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae6b8-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae6b8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=n)

```
## <a name="request-headers"></a><span data-ttu-id="ae6b8-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae6b8-115">Request headers</span></span>
| <span data-ttu-id="ae6b8-116">Имя</span><span class="sxs-lookup"><span data-stu-id="ae6b8-116">Name</span></span>       | <span data-ttu-id="ae6b8-117">Описание</span><span class="sxs-lookup"><span data-stu-id="ae6b8-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ae6b8-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae6b8-118">Authorization</span></span>  | <span data-ttu-id="ae6b8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae6b8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae6b8-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ae6b8-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="ae6b8-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ae6b8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="ae6b8-124">Параметры</span><span class="sxs-lookup"><span data-stu-id="ae6b8-124">Parameters</span></span>

| <span data-ttu-id="ae6b8-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="ae6b8-125">Parameter</span></span>    | <span data-ttu-id="ae6b8-126">Тип</span><span class="sxs-lookup"><span data-stu-id="ae6b8-126">Type</span></span>   |<span data-ttu-id="ae6b8-127">Описание</span><span class="sxs-lookup"><span data-stu-id="ae6b8-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae6b8-128">count</span><span class="sxs-lookup"><span data-stu-id="ae6b8-128">count</span></span>|<span data-ttu-id="ae6b8-129">Int32</span><span class="sxs-lookup"><span data-stu-id="ae6b8-129">Int32</span></span>|<span data-ttu-id="ae6b8-p104">Количество строк, которые нужно включить в результирующий диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете указать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. По умолчанию используется значение 1.</span><span class="sxs-lookup"><span data-stu-id="ae6b8-p104">The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae6b8-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ae6b8-134">Request body</span></span>

### <a name="response"></a><span data-ttu-id="ae6b8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae6b8-135">Response</span></span>
<span data-ttu-id="ae6b8-136">В случае успеха этот метод возвращает код отклика `200, OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ae6b8-136">If successful, this method returns `200, OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae6b8-137">Пример</span><span class="sxs-lookup"><span data-stu-id="ae6b8-137">Example</span></span>
<span data-ttu-id="ae6b8-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ae6b8-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ae6b8-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae6b8-139">Request</span></span>
<span data-ttu-id="ae6b8-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae6b8-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsAbove"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```

##### <a name="response"></a><span data-ttu-id="ae6b8-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="ae6b8-141">Response</span></span>
<span data-ttu-id="ae6b8-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ae6b8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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