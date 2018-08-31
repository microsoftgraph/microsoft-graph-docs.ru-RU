# <a name="workbookrange-resizedrange"></a><span data-ttu-id="6ea4d-101">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="6ea4d-101">workbookRange: resizedRange</span></span>
<span data-ttu-id="6ea4d-102">Возвращает объект диапазона, подобный текущему объекту диапазона, но увеличенный (или уменьшенный) на некоторое количество строк и столбцов в правом нижнем углу.</span><span class="sxs-lookup"><span data-stu-id="6ea4d-102">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ea4d-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ea4d-103">Permissions</span></span>
<span data-ttu-id="6ea4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6ea4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6ea4d-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ea4d-106">Permission type</span></span>      | <span data-ttu-id="6ea4d-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ea4d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ea4d-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ea4d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6ea4d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ea4d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6ea4d-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ea4d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ea4d-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ea4d-111">Not supported.</span></span>    |
|<span data-ttu-id="6ea4d-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ea4d-112">Application</span></span> | <span data-ttu-id="6ea4d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ea4d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ea4d-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ea4d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```
## <a name="request-headers"></a><span data-ttu-id="6ea4d-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ea4d-115">Request headers</span></span>
| <span data-ttu-id="6ea4d-116">Имя</span><span class="sxs-lookup"><span data-stu-id="6ea4d-116">Name</span></span>       | <span data-ttu-id="6ea4d-117">Описание</span><span class="sxs-lookup"><span data-stu-id="6ea4d-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6ea4d-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ea4d-118">Authorization</span></span>  | <span data-ttu-id="6ea4d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ea4d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6ea4d-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6ea4d-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="6ea4d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="6ea4d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="6ea4d-124">Параметры</span><span class="sxs-lookup"><span data-stu-id="6ea4d-124">Parameters</span></span>

| <span data-ttu-id="6ea4d-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="6ea4d-125">Parameter</span></span>    | <span data-ttu-id="6ea4d-126">Тип</span><span class="sxs-lookup"><span data-stu-id="6ea4d-126">Type</span></span>   |<span data-ttu-id="6ea4d-127">Описание</span><span class="sxs-lookup"><span data-stu-id="6ea4d-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ea4d-128">deltaRows</span><span class="sxs-lookup"><span data-stu-id="6ea4d-128">deltaRows</span></span>|<span data-ttu-id="6ea4d-129">Int32</span><span class="sxs-lookup"><span data-stu-id="6ea4d-129">Int32</span></span>|<span data-ttu-id="6ea4d-p104">Количество строк, добавляемых в правый нижний угол текущего диапазона. Используйте положительное число, чтобы расширить диапазон, или отрицательное число, чтобы уменьшить его.</span><span class="sxs-lookup"><span data-stu-id="6ea4d-p104">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="6ea4d-132">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="6ea4d-132">deltaColumns</span></span>|<span data-ttu-id="6ea4d-133">Int32</span><span class="sxs-lookup"><span data-stu-id="6ea4d-133">Int32</span></span>|<span data-ttu-id="6ea4d-134">Количество столбцов, на которое будет расширен нижний правый угол, относительно текущего диапазона.</span><span class="sxs-lookup"><span data-stu-id="6ea4d-134">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span> <span data-ttu-id="6ea4d-135">Используйте положительное число, чтобы расширить диапазон, или отрицательное значение, чтобы его уменьшить.</span><span class="sxs-lookup"><span data-stu-id="6ea4d-135">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

### <a name="response"></a><span data-ttu-id="6ea4d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ea4d-136">Response</span></span>
<span data-ttu-id="6ea4d-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6ea4d-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ea4d-138">Пример</span><span class="sxs-lookup"><span data-stu-id="6ea4d-138">Example</span></span>
<span data-ttu-id="6ea4d-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6ea4d-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6ea4d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ea4d-140">Request</span></span>
<span data-ttu-id="6ea4d-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ea4d-141">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_resizedrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="6ea4d-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ea4d-142">Response</span></span>
<span data-ttu-id="6ea4d-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ea4d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
