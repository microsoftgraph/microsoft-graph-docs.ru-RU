# <a name="workbookrange-resizedrange"></a><span data-ttu-id="302e5-101">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="302e5-101">workbookRange: resizedRange</span></span>
<span data-ttu-id="302e5-102">Возвращает объект диапазона, подобный текущему объекту диапазона, но увеличенный (или уменьшенный) на некоторое количество строк и столбцов в правом нижнем углу.</span><span class="sxs-lookup"><span data-stu-id="302e5-102">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="302e5-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="302e5-103">Permissions</span></span>
<span data-ttu-id="302e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="302e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="302e5-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="302e5-106">Permission type</span></span>      | <span data-ttu-id="302e5-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="302e5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="302e5-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="302e5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="302e5-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="302e5-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="302e5-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="302e5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="302e5-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="302e5-111">Not supported.</span></span>    |
|<span data-ttu-id="302e5-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="302e5-112">Application</span></span> | <span data-ttu-id="302e5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="302e5-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="302e5-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="302e5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```
## <a name="request-headers"></a><span data-ttu-id="302e5-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="302e5-115">Request headers</span></span>
| <span data-ttu-id="302e5-116">Имя</span><span class="sxs-lookup"><span data-stu-id="302e5-116">Name</span></span>       | <span data-ttu-id="302e5-117">Описание</span><span class="sxs-lookup"><span data-stu-id="302e5-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="302e5-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="302e5-118">Authorization</span></span>  | <span data-ttu-id="302e5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="302e5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="302e5-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="302e5-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="302e5-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="302e5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="302e5-124">Параметры</span><span class="sxs-lookup"><span data-stu-id="302e5-124">Parameters</span></span>

| <span data-ttu-id="302e5-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="302e5-125">Parameter</span></span>    | <span data-ttu-id="302e5-126">Тип</span><span class="sxs-lookup"><span data-stu-id="302e5-126">Type</span></span>   |<span data-ttu-id="302e5-127">Описание</span><span class="sxs-lookup"><span data-stu-id="302e5-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="302e5-128">deltarows</span><span class="sxs-lookup"><span data-stu-id="302e5-128">deltarows</span></span>|<span data-ttu-id="302e5-129">Int32</span><span class="sxs-lookup"><span data-stu-id="302e5-129">Int32</span></span>|<span data-ttu-id="302e5-p104">Количество строк, добавляемых в правый нижний угол текущего диапазона. Используйте положительное число, чтобы расширить диапазон, или отрицательное число, чтобы уменьшить его.</span><span class="sxs-lookup"><span data-stu-id="302e5-p104">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="302e5-132">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="302e5-132">deltaColumns</span></span>|<span data-ttu-id="302e5-133">Int32</span><span class="sxs-lookup"><span data-stu-id="302e5-133">Int32</span></span>|<span data-ttu-id="302e5-p105">Количество столбцов, добавляемых в правый нижний угол, относительно текущего диапазона. Используйте положительное число, чтобы расширить диапазон или отрицательное число, чтобы уменьшить его.</span><span class="sxs-lookup"><span data-stu-id="302e5-p105">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-body"></a><span data-ttu-id="302e5-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="302e5-136">Request body</span></span>
<span data-ttu-id="302e5-137">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="302e5-137">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="302e5-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="302e5-138">Parameter</span></span>    | <span data-ttu-id="302e5-139">Тип</span><span class="sxs-lookup"><span data-stu-id="302e5-139">Type</span></span>   |<span data-ttu-id="302e5-140">Описание</span><span class="sxs-lookup"><span data-stu-id="302e5-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="302e5-141">deltaRows</span><span class="sxs-lookup"><span data-stu-id="302e5-141">deltaRows</span></span>|<span data-ttu-id="302e5-142">Int32</span><span class="sxs-lookup"><span data-stu-id="302e5-142">Int32</span></span>||
|<span data-ttu-id="302e5-143">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="302e5-143">deltaColumns</span></span>|<span data-ttu-id="302e5-144">Int32</span><span class="sxs-lookup"><span data-stu-id="302e5-144">Int32</span></span>||

### <a name="response"></a><span data-ttu-id="302e5-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="302e5-145">Response</span></span>
<span data-ttu-id="302e5-146">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="302e5-146">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="302e5-147">Пример</span><span class="sxs-lookup"><span data-stu-id="302e5-147">Example</span></span>
<span data-ttu-id="302e5-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="302e5-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="302e5-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="302e5-149">Request</span></span>
<span data-ttu-id="302e5-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="302e5-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_resizedrange"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range/resizedRange(deltarows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="302e5-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="302e5-151">Response</span></span>
<span data-ttu-id="302e5-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="302e5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
