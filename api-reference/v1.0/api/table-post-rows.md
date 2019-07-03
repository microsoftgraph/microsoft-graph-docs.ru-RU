---
title: Создание объекта TableRow
description: 'Добавляет строки в конец таблицы. Обратите внимание, что API может принимать несколько строк данных с помощью этого API. Добавление по одной строке за раз может привести к ухудшению производительности. Рекомендуемый подход заключается в пакетировании строк в одном вызове, а не при вставке одиночной строки. Для достижения лучших результатов Соберите строки, которые необходимо вставить на стороне приложения, и выполните операцию добавления отдельных строк. Поэкспериментируйте с количеством строк, чтобы определить оптимальное количество строк для использования в едином вызове API. '
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: a6f8ff3c282b687d836bff0add39f0b43f772b75
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450438"
---
# <a name="create-tablerow"></a><span data-ttu-id="a9546-108">Создание объекта TableRow</span><span class="sxs-lookup"><span data-stu-id="a9546-108">Create TableRow</span></span>

<span data-ttu-id="a9546-109">Добавляет строки в конец таблицы.</span><span class="sxs-lookup"><span data-stu-id="a9546-109">Adds rows to the end of the table.</span></span> <span data-ttu-id="a9546-110">Обратите внимание, что API может принимать несколько строк данных с помощью этого API.</span><span class="sxs-lookup"><span data-stu-id="a9546-110">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="a9546-111">Добавление по одной строке за раз может привести к ухудшению производительности.</span><span class="sxs-lookup"><span data-stu-id="a9546-111">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="a9546-112">Рекомендуемый подход заключается в пакетировании строк в одном вызове, а не при вставке одиночной строки.</span><span class="sxs-lookup"><span data-stu-id="a9546-112">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="a9546-113">Для достижения лучших результатов Соберите строки, которые необходимо вставить на стороне приложения, и выполните операцию добавления отдельных строк.</span><span class="sxs-lookup"><span data-stu-id="a9546-113">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="a9546-114">Поэкспериментируйте с количеством строк, чтобы определить оптимальное количество строк для использования в едином вызове API.</span><span class="sxs-lookup"><span data-stu-id="a9546-114">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="a9546-115">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="a9546-115">Error Handling</span></span>

<span data-ttu-id="a9546-116">Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP.</span><span class="sxs-lookup"><span data-stu-id="a9546-116">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="a9546-117">В этом случае нужно повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="a9546-117">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9546-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9546-118">Permissions</span></span>
<span data-ttu-id="a9546-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9546-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9546-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9546-121">Permission type</span></span>      | <span data-ttu-id="a9546-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9546-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9546-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9546-123">Delegated (work or school account)</span></span> | <span data-ttu-id="a9546-124">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9546-124">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a9546-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9546-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9546-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9546-126">Not supported.</span></span>    |
|<span data-ttu-id="a9546-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9546-127">Application</span></span> | <span data-ttu-id="a9546-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9546-128">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9546-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9546-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="a9546-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9546-130">Request headers</span></span>
| <span data-ttu-id="a9546-131">Имя</span><span class="sxs-lookup"><span data-stu-id="a9546-131">Name</span></span>       | <span data-ttu-id="a9546-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a9546-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a9546-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9546-133">Authorization</span></span>  | <span data-ttu-id="a9546-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9546-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a9546-136">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a9546-136">Workbook-Session-Id</span></span>  | <span data-ttu-id="a9546-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a9546-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9546-139">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a9546-139">Request body</span></span>
<span data-ttu-id="a9546-140">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a9546-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a9546-141">Параметр</span><span class="sxs-lookup"><span data-stu-id="a9546-141">Parameter</span></span>    | <span data-ttu-id="a9546-142">Тип</span><span class="sxs-lookup"><span data-stu-id="a9546-142">Type</span></span>   |<span data-ttu-id="a9546-143">Описание</span><span class="sxs-lookup"><span data-stu-id="a9546-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9546-144">index</span><span class="sxs-lookup"><span data-stu-id="a9546-144">index</span></span>|<span data-ttu-id="a9546-145">number</span><span class="sxs-lookup"><span data-stu-id="a9546-145">number</span></span>|<span data-ttu-id="a9546-p107">Необязательный параметр. Определяет относительную позицию новой строки. Если параметру присвоено значение null, строка добавляется в конце. Все строки ниже вставляемой строки сдвигаются вниз. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="a9546-p107">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="a9546-151">values</span><span class="sxs-lookup"><span data-stu-id="a9546-151">values</span></span>|<span data-ttu-id="a9546-152">Json</span><span class="sxs-lookup"><span data-stu-id="a9546-152">Json</span></span>|<span data-ttu-id="a9546-153">Двухмерный массив неформатированных значений строк таблицы (логическое значение или строка или число).</span><span class="sxs-lookup"><span data-stu-id="a9546-153">A 2-dimensional array of unformatted values of the table rows (boolean or string or number).</span></span>|

## <a name="response"></a><span data-ttu-id="a9546-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9546-154">Response</span></span>

<span data-ttu-id="a9546-155">В случае успеха этот метод возвращает код отклика `200 OK` и объект [TableRow](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a9546-155">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9546-156">Пример</span><span class="sxs-lookup"><span data-stu-id="a9546-156">Example</span></span>
<span data-ttu-id="a9546-157">В этом примере две строки данных вставляются в конец таблицы.</span><span class="sxs-lookup"><span data-stu-id="a9546-157">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="a9546-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9546-158">Request</span></span>
<span data-ttu-id="a9546-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9546-159">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a9546-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9546-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a9546-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="a9546-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a9546-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9546-162">Response</span></span>
<span data-ttu-id="a9546-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9546-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/table-post-rows.md/tablerowcollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Collection)) is a collection, while the table description type (microsoft.graph.Json) is not.",
    "Warning: /api-reference/v1.0/api/table-post-rows.md/tablerowcollection_add/values:
      Inconsistent types between parameter (Collection) and table (None)"
  ],
  "tocPath": ""
}-->
