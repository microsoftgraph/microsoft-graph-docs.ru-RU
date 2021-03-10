---
title: Создание объекта TableRow
description: 'Добавляет строки в конец таблицы. Обратите внимание, что API может принимать данные нескольких строк с помощью этого API. Добавление одной строки одновременно может привести к снижению производительности. Рекомендуемый подход заключается в том, чтобы пакетить строки вместе в одном вызове, а не делать вставку одной строки. Чтобы получить наилучшие результаты, соберйте строки, которые будут вставлены на стороне приложения, и выполните операцию добавления одной строки. Поэкспериментируйте с количеством строк, чтобы определить идеальное число строк, которые можно использовать в одном вызове API. '
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1751b0cb7714cdd867306fb759f646b0d022cd34
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577179"
---
# <a name="create-tablerow"></a><span data-ttu-id="5f94f-108">Создание объекта TableRow</span><span class="sxs-lookup"><span data-stu-id="5f94f-108">Create TableRow</span></span>

<span data-ttu-id="5f94f-109">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f94f-109">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5f94f-110">Добавляет строки в конец таблицы.</span><span class="sxs-lookup"><span data-stu-id="5f94f-110">Adds rows to the end of the table.</span></span> <span data-ttu-id="5f94f-111">Обратите внимание, что API может принимать данные нескольких строк с помощью этого API.</span><span class="sxs-lookup"><span data-stu-id="5f94f-111">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="5f94f-112">Добавление одной строки одновременно может привести к снижению производительности.</span><span class="sxs-lookup"><span data-stu-id="5f94f-112">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="5f94f-113">Рекомендуемый подход заключается в том, чтобы пакетить строки вместе в одном вызове, а не делать вставку одной строки.</span><span class="sxs-lookup"><span data-stu-id="5f94f-113">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="5f94f-114">Чтобы получить наилучшие результаты, соберйте строки, которые будут вставлены на стороне приложения, и выполните операцию добавления одной строки.</span><span class="sxs-lookup"><span data-stu-id="5f94f-114">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="5f94f-115">Поэкспериментируйте с количеством строк, чтобы определить идеальное число строк, которые можно использовать в одном вызове API.</span><span class="sxs-lookup"><span data-stu-id="5f94f-115">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="5f94f-116">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="5f94f-116">Error Handling</span></span>

<span data-ttu-id="5f94f-117">Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP.</span><span class="sxs-lookup"><span data-stu-id="5f94f-117">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="5f94f-118">В этом случае нужно повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="5f94f-118">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f94f-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f94f-119">Permissions</span></span>
<span data-ttu-id="5f94f-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f94f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f94f-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f94f-122">Permission type</span></span>      | <span data-ttu-id="5f94f-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f94f-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f94f-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f94f-124">Delegated (work or school account)</span></span> | <span data-ttu-id="5f94f-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f94f-125">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5f94f-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f94f-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f94f-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f94f-127">Not supported.</span></span>    |
|<span data-ttu-id="5f94f-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f94f-128">Application</span></span> | <span data-ttu-id="5f94f-129">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f94f-129">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f94f-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f94f-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/rows/add
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/rows/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/rows/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="5f94f-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f94f-131">Request headers</span></span>
| <span data-ttu-id="5f94f-132">Имя</span><span class="sxs-lookup"><span data-stu-id="5f94f-132">Name</span></span>       | <span data-ttu-id="5f94f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="5f94f-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5f94f-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f94f-134">Authorization</span></span>  | <span data-ttu-id="5f94f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f94f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f94f-137">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5f94f-137">Workbook-Session-Id</span></span>  | <span data-ttu-id="5f94f-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="5f94f-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f94f-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f94f-140">Request body</span></span>
<span data-ttu-id="5f94f-141">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5f94f-141">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5f94f-142">Параметр</span><span class="sxs-lookup"><span data-stu-id="5f94f-142">Parameter</span></span>    | <span data-ttu-id="5f94f-143">Тип</span><span class="sxs-lookup"><span data-stu-id="5f94f-143">Type</span></span>   |<span data-ttu-id="5f94f-144">Описание</span><span class="sxs-lookup"><span data-stu-id="5f94f-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f94f-145">index</span><span class="sxs-lookup"><span data-stu-id="5f94f-145">index</span></span>|<span data-ttu-id="5f94f-146">number</span><span class="sxs-lookup"><span data-stu-id="5f94f-146">number</span></span>|<span data-ttu-id="5f94f-p107">Необязательный параметр. Определяет относительную позицию новой строки. Если параметру присвоено значение null, строка добавляется в конце. Все строки ниже вставляемой строки сдвигаются вниз. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="5f94f-p107">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="5f94f-152">values</span><span class="sxs-lookup"><span data-stu-id="5f94f-152">values</span></span>|<span data-ttu-id="5f94f-153">Json</span><span class="sxs-lookup"><span data-stu-id="5f94f-153">Json</span></span>|<span data-ttu-id="5f94f-154">Двухмерный массив неформатированные значения строк таблицы (boolean или string or number).</span><span class="sxs-lookup"><span data-stu-id="5f94f-154">A 2-dimensional array of unformatted values of the table rows (boolean or string or number).</span></span>|

## <a name="response"></a><span data-ttu-id="5f94f-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f94f-155">Response</span></span>

<span data-ttu-id="5f94f-156">В случае успеха этот метод возвращает код отклика `200 OK` и объект [TableRow](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5f94f-156">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f94f-157">Пример</span><span class="sxs-lookup"><span data-stu-id="5f94f-157">Example</span></span>
<span data-ttu-id="5f94f-158">В этом примере в конце таблицы вставляются два ряда данных.</span><span class="sxs-lookup"><span data-stu-id="5f94f-158">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="5f94f-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f94f-159">Request</span></span>
<span data-ttu-id="5f94f-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f94f-160">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5f94f-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f94f-161">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="5f94f-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f94f-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="5f94f-163">C#</span><span class="sxs-lookup"><span data-stu-id="5f94f-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablerowcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5f94f-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f94f-164">Response</span></span>
<span data-ttu-id="5f94f-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5f94f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ],
  "tocPath": ""
}-->

