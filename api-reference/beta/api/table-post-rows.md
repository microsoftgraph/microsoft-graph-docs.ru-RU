---
title: Создание объекта TableRow
description: 'Добавляет строки в конец таблицы. Обратите внимание, что API может принимать несколько строк данных с помощью этого API. Добавление по одной строке за раз может привести к ухудшению производительности. Рекомендуемый подход заключается в пакетировании строк в одном вызове, а не при вставке одиночной строки. Для достижения лучших результатов Соберите строки, которые необходимо вставить на стороне приложения, и выполните операцию добавления отдельных строк. Поэкспериментируйте с количеством строк, чтобы определить оптимальное количество строк для использования в едином вызове API. '
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a2e7fdf3cbe3eabb575d256f405f565e1bec151e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452815"
---
# <a name="create-tablerow"></a><span data-ttu-id="dc8a2-108">Создание объекта TableRow</span><span class="sxs-lookup"><span data-stu-id="dc8a2-108">Create TableRow</span></span>

<span data-ttu-id="dc8a2-109">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc8a2-109">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc8a2-110">Добавляет строки в конец таблицы.</span><span class="sxs-lookup"><span data-stu-id="dc8a2-110">Adds rows to the end of the table.</span></span> <span data-ttu-id="dc8a2-111">Обратите внимание, что API может принимать несколько строк данных с помощью этого API.</span><span class="sxs-lookup"><span data-stu-id="dc8a2-111">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="dc8a2-112">Добавление по одной строке за раз может привести к ухудшению производительности.</span><span class="sxs-lookup"><span data-stu-id="dc8a2-112">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="dc8a2-113">Рекомендуемый подход заключается в пакетировании строк в одном вызове, а не при вставке одиночной строки.</span><span class="sxs-lookup"><span data-stu-id="dc8a2-113">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="dc8a2-114">Для достижения лучших результатов Соберите строки, которые необходимо вставить на стороне приложения, и выполните операцию добавления отдельных строк.</span><span class="sxs-lookup"><span data-stu-id="dc8a2-114">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="dc8a2-115">Поэкспериментируйте с количеством строк, чтобы определить оптимальное количество строк для использования в едином вызове API.</span><span class="sxs-lookup"><span data-stu-id="dc8a2-115">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="dc8a2-116">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="dc8a2-116">Error Handling</span></span>

<span data-ttu-id="dc8a2-117">Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP.</span><span class="sxs-lookup"><span data-stu-id="dc8a2-117">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="dc8a2-118">В этом случае нужно повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="dc8a2-118">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc8a2-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc8a2-119">Permissions</span></span>
<span data-ttu-id="dc8a2-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc8a2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc8a2-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc8a2-122">Permission type</span></span>      | <span data-ttu-id="dc8a2-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc8a2-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc8a2-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc8a2-124">Delegated (work or school account)</span></span> | <span data-ttu-id="dc8a2-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc8a2-125">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dc8a2-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc8a2-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc8a2-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc8a2-127">Not supported.</span></span>    |
|<span data-ttu-id="dc8a2-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc8a2-128">Application</span></span> | <span data-ttu-id="dc8a2-129">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc8a2-129">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc8a2-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc8a2-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="dc8a2-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc8a2-131">Request headers</span></span>
| <span data-ttu-id="dc8a2-132">Имя</span><span class="sxs-lookup"><span data-stu-id="dc8a2-132">Name</span></span>       | <span data-ttu-id="dc8a2-133">Описание</span><span class="sxs-lookup"><span data-stu-id="dc8a2-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dc8a2-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc8a2-134">Authorization</span></span>  | <span data-ttu-id="dc8a2-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc8a2-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dc8a2-137">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dc8a2-137">Workbook-Session-Id</span></span>  | <span data-ttu-id="dc8a2-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="dc8a2-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc8a2-140">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dc8a2-140">Request body</span></span>
<span data-ttu-id="dc8a2-141">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="dc8a2-141">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dc8a2-142">Параметр</span><span class="sxs-lookup"><span data-stu-id="dc8a2-142">Parameter</span></span>    | <span data-ttu-id="dc8a2-143">Тип</span><span class="sxs-lookup"><span data-stu-id="dc8a2-143">Type</span></span>   |<span data-ttu-id="dc8a2-144">Описание</span><span class="sxs-lookup"><span data-stu-id="dc8a2-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc8a2-145">index</span><span class="sxs-lookup"><span data-stu-id="dc8a2-145">index</span></span>|<span data-ttu-id="dc8a2-146">number</span><span class="sxs-lookup"><span data-stu-id="dc8a2-146">number</span></span>|<span data-ttu-id="dc8a2-p107">Необязательный параметр. Определяет относительную позицию новой строки. Если параметру присвоено значение null, строка добавляется в конце. Все строки ниже вставляемой строки сдвигаются вниз. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="dc8a2-p107">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="dc8a2-152">values</span><span class="sxs-lookup"><span data-stu-id="dc8a2-152">values</span></span>|<span data-ttu-id="dc8a2-153">(логическая или числовая) коллекция</span><span class="sxs-lookup"><span data-stu-id="dc8a2-153">(boolean or string or number) collection</span></span>|<span data-ttu-id="dc8a2-154">Двухмерный массив неформатированных значений строк таблицы.</span><span class="sxs-lookup"><span data-stu-id="dc8a2-154">A 2-dimensional array of unformatted values of the table rows.</span></span>|

## <a name="response"></a><span data-ttu-id="dc8a2-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc8a2-155">Response</span></span>

<span data-ttu-id="dc8a2-156">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбуктаблеров](../resources/workbooktablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dc8a2-156">If successful, this method returns `200 OK` response code and [workbookTableRow](../resources/workbooktablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc8a2-157">Пример</span><span class="sxs-lookup"><span data-stu-id="dc8a2-157">Example</span></span>
<span data-ttu-id="dc8a2-158">В этом примере две строки данных вставляются в конец таблицы.</span><span class="sxs-lookup"><span data-stu-id="dc8a2-158">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="dc8a2-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc8a2-159">Request</span></span>
<span data-ttu-id="dc8a2-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc8a2-160">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dc8a2-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc8a2-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="dc8a2-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc8a2-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="dc8a2-163">C#</span><span class="sxs-lookup"><span data-stu-id="dc8a2-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablerowcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dc8a2-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc8a2-164">Response</span></span>
<span data-ttu-id="dc8a2-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc8a2-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
