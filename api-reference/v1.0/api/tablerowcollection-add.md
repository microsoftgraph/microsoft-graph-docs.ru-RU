---
title: 'TableRowCollection: add'
description: 'Добавляет строки в конец таблицы. Обратите внимание, что API может принимать данные нескольких строк с помощью этого API. Добавление одной строки одновременно может привести к снижению производительности. Рекомендуемый подход заключается в том, чтобы пакетить строки вместе в одном вызове, а не делать вставку одной строки. Чтобы получить наилучшие результаты, соберйте строки, которые будут вставлены на стороне приложения, и выполните операцию добавления одной строки. Поэкспериментируйте с количеством строк, чтобы определить идеальное число строк, которые можно использовать в одном вызове API. '
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b968d33be6c37bb5f8008805a7a29370a2dde0be
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577564"
---
# <a name="tablerowcollection-add"></a><span data-ttu-id="8ebb8-108">TableRowCollection: add</span><span class="sxs-lookup"><span data-stu-id="8ebb8-108">TableRowCollection: add</span></span>

<span data-ttu-id="8ebb8-109">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ebb8-109">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8ebb8-110">Добавляет строки в конец таблицы.</span><span class="sxs-lookup"><span data-stu-id="8ebb8-110">Adds rows to the end of the table.</span></span> <span data-ttu-id="8ebb8-111">Обратите внимание, что API может принимать данные нескольких строк с помощью этого API.</span><span class="sxs-lookup"><span data-stu-id="8ebb8-111">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="8ebb8-112">Добавление одной строки одновременно может привести к снижению производительности.</span><span class="sxs-lookup"><span data-stu-id="8ebb8-112">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="8ebb8-113">Рекомендуемый подход заключается в том, чтобы пакетить строки вместе в одном вызове, а не делать вставку одной строки.</span><span class="sxs-lookup"><span data-stu-id="8ebb8-113">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="8ebb8-114">Чтобы получить наилучшие результаты, соберйте строки, которые будут вставлены на стороне приложения, и выполните операцию добавления одной строки.</span><span class="sxs-lookup"><span data-stu-id="8ebb8-114">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="8ebb8-115">Поэкспериментируйте с количеством строк, чтобы определить идеальное число строк, которые можно использовать в одном вызове API.</span><span class="sxs-lookup"><span data-stu-id="8ebb8-115">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="8ebb8-116">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="8ebb8-116">Error Handling</span></span>

<span data-ttu-id="8ebb8-117">Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP.</span><span class="sxs-lookup"><span data-stu-id="8ebb8-117">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="8ebb8-118">В этом случае нужно повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="8ebb8-118">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ebb8-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ebb8-119">Permissions</span></span>
<span data-ttu-id="8ebb8-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ebb8-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ebb8-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ebb8-122">Permission type</span></span>      | <span data-ttu-id="8ebb8-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ebb8-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ebb8-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ebb8-124">Delegated (work or school account)</span></span> | <span data-ttu-id="8ebb8-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ebb8-125">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8ebb8-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ebb8-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ebb8-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ebb8-127">Not supported.</span></span>    |
|<span data-ttu-id="8ebb8-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ebb8-128">Application</span></span> | <span data-ttu-id="8ebb8-129">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ebb8-129">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ebb8-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ebb8-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/rows/add
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/rows/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/rows/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="8ebb8-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ebb8-131">Request headers</span></span>
| <span data-ttu-id="8ebb8-132">Имя</span><span class="sxs-lookup"><span data-stu-id="8ebb8-132">Name</span></span>       | <span data-ttu-id="8ebb8-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8ebb8-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8ebb8-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ebb8-134">Authorization</span></span>  | <span data-ttu-id="8ebb8-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ebb8-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8ebb8-137">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8ebb8-137">Workbook-Session-Id</span></span>  | <span data-ttu-id="8ebb8-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8ebb8-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ebb8-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ebb8-140">Request body</span></span>
<span data-ttu-id="8ebb8-141">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8ebb8-141">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8ebb8-142">Параметр</span><span class="sxs-lookup"><span data-stu-id="8ebb8-142">Parameter</span></span>    | <span data-ttu-id="8ebb8-143">Тип</span><span class="sxs-lookup"><span data-stu-id="8ebb8-143">Type</span></span>   |<span data-ttu-id="8ebb8-144">Описание</span><span class="sxs-lookup"><span data-stu-id="8ebb8-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ebb8-145">index</span><span class="sxs-lookup"><span data-stu-id="8ebb8-145">index</span></span>|<span data-ttu-id="8ebb8-146">Int32</span><span class="sxs-lookup"><span data-stu-id="8ebb8-146">Int32</span></span>|<span data-ttu-id="8ebb8-p107">Необязательный параметр. Определяет относительную позицию новой строки. Если параметру присвоено значение null, строка добавляется в конце. Все строки ниже вставляемой строки сдвигаются вниз. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="8ebb8-p107">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="8ebb8-152">values</span><span class="sxs-lookup"><span data-stu-id="8ebb8-152">values</span></span>|<span data-ttu-id="8ebb8-153">Json</span><span class="sxs-lookup"><span data-stu-id="8ebb8-153">Json</span></span>|<span data-ttu-id="8ebb8-p108">Необязательный параметр. Двухмерный массив неформатированных значений строки таблицы.</span><span class="sxs-lookup"><span data-stu-id="8ebb8-p108">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="8ebb8-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ebb8-156">Response</span></span>

<span data-ttu-id="8ebb8-157">В случае успеха этот метод возвращает код отклика и `200 OK` [объект WorkbookTableRow](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8ebb8-157">If successful, this method returns `200 OK` response code and [WorkbookTableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ebb8-158">Пример</span><span class="sxs-lookup"><span data-stu-id="8ebb8-158">Example</span></span>
<span data-ttu-id="8ebb8-159">В этом примере в конце таблицы вставляются два ряда данных.</span><span class="sxs-lookup"><span data-stu-id="8ebb8-159">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="8ebb8-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ebb8-160">Request</span></span>
<span data-ttu-id="8ebb8-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ebb8-161">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8ebb8-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ebb8-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": 5,
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="8ebb8-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ebb8-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="8ebb8-164">C#</span><span class="sxs-lookup"><span data-stu-id="8ebb8-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablerowcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8ebb8-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ebb8-165">Response</span></span>
<span data-ttu-id="8ebb8-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ebb8-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

