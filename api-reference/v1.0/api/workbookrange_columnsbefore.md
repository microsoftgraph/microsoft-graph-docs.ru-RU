# <a name="workbookrange-columnsbefore"></a><span data-ttu-id="b9a46-101">workbookRange: columnsBefore</span><span class="sxs-lookup"><span data-stu-id="b9a46-101">workbookRange: columnsBefore</span></span>

<span data-ttu-id="b9a46-102">Возвращает определенное количество столбцов слева от заданного диапазона.</span><span class="sxs-lookup"><span data-stu-id="b9a46-102">Gets a certain number of columns to the left of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9a46-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9a46-103">Permissions</span></span>
<span data-ttu-id="b9a46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b9a46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b9a46-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9a46-106">Permission type</span></span>      | <span data-ttu-id="b9a46-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9a46-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9a46-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9a46-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b9a46-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9a46-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b9a46-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9a46-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9a46-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9a46-111">Not supported.</span></span>    |
|<span data-ttu-id="b9a46-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9a46-112">Application</span></span> | <span data-ttu-id="b9a46-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9a46-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9a46-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9a46-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="b9a46-115">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="b9a46-115">Function parameters</span></span>

| <span data-ttu-id="b9a46-116">Параметр</span><span class="sxs-lookup"><span data-stu-id="b9a46-116">Parameter</span></span>    | <span data-ttu-id="b9a46-117">Тип</span><span class="sxs-lookup"><span data-stu-id="b9a46-117">Type</span></span>   |<span data-ttu-id="b9a46-118">Описание</span><span class="sxs-lookup"><span data-stu-id="b9a46-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9a46-119">count</span><span class="sxs-lookup"><span data-stu-id="b9a46-119">count</span></span>|<span data-ttu-id="b9a46-120">Int32</span><span class="sxs-lookup"><span data-stu-id="b9a46-120">Int32</span></span>|<span data-ttu-id="b9a46-p102">Необязательный. Количество столбцов, включаемых в полученный диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете использовать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="b9a46-p102">Optional. The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="b9a46-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9a46-126">Request headers</span></span>
| <span data-ttu-id="b9a46-127">Имя</span><span class="sxs-lookup"><span data-stu-id="b9a46-127">Name</span></span>       | <span data-ttu-id="b9a46-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b9a46-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b9a46-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9a46-129">Authorization</span></span>  | <span data-ttu-id="b9a46-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9a46-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9a46-132">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b9a46-132">Workbook-Session-Id</span></span>  | <span data-ttu-id="b9a46-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b9a46-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9a46-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9a46-135">Request body</span></span>
<span data-ttu-id="b9a46-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9a46-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9a46-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9a46-137">Response</span></span>
<span data-ttu-id="b9a46-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b9a46-138">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9a46-139">Пример</span><span class="sxs-lookup"><span data-stu-id="b9a46-139">Example</span></span>
<span data-ttu-id="b9a46-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b9a46-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b9a46-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9a46-141">Request</span></span>
<span data-ttu-id="b9a46-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9a46-142">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_columnsbefore",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)
```

##### <a name="response"></a><span data-ttu-id="b9a46-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9a46-143">Response</span></span>
<span data-ttu-id="b9a46-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9a46-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
