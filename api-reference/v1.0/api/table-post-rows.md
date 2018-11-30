---
title: Создание объекта TableRow
description: 'Добавляет строки в конец таблицы. Обратите внимание на то, что API может принимать несколько строк данных, с помощью этот интерфейс API. Добавление одной строке за раз может привести к снижению производительности. Рекомендуемый подход бы для пакетной обработки строк в один вызов, а не выполнив одну строку вставки. Для достижения наилучших результатов собирать строки, чтобы вставить в части приложения и выполнить отдельных строк добавьте операции. Поэкспериментируйте с номером строки, чтобы определить, идеальная число строк для использования в одном вызове API. '
ms.openlocfilehash: 67197eb8ba67bfc4f8406de5df2d7158409c85d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028109"
---
# <a name="create-tablerow"></a><span data-ttu-id="83602-108">Создание объекта TableRow</span><span class="sxs-lookup"><span data-stu-id="83602-108">Create TableRow</span></span>

<span data-ttu-id="83602-109">Добавляет строки в конец таблицы.</span><span class="sxs-lookup"><span data-stu-id="83602-109">Adds rows to the end of the table.</span></span> <span data-ttu-id="83602-110">Обратите внимание на то, что API может принимать несколько строк данных, с помощью этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="83602-110">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="83602-111">Добавление одной строке за раз может привести к снижению производительности.</span><span class="sxs-lookup"><span data-stu-id="83602-111">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="83602-112">Рекомендуемый подход бы для пакетной обработки строк в один вызов, а не выполнив одну строку вставки.</span><span class="sxs-lookup"><span data-stu-id="83602-112">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="83602-113">Для достижения наилучших результатов собирать строки, чтобы вставить в части приложения и выполнить отдельных строк добавьте операции.</span><span class="sxs-lookup"><span data-stu-id="83602-113">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="83602-114">Поэкспериментируйте с номером строки, чтобы определить, идеальная число строк для использования в одном вызове API.</span><span class="sxs-lookup"><span data-stu-id="83602-114">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="83602-115">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="83602-115">Error Handling</span></span>

<span data-ttu-id="83602-116">Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP.</span><span class="sxs-lookup"><span data-stu-id="83602-116">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="83602-117">В этом случае нужно повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="83602-117">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="83602-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="83602-118">Permissions</span></span>
<span data-ttu-id="83602-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83602-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83602-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83602-121">Permission type</span></span>      | <span data-ttu-id="83602-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="83602-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83602-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83602-123">Delegated (work or school account)</span></span> | <span data-ttu-id="83602-124">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83602-124">Files.ReadWrite</span></span>    |
|<span data-ttu-id="83602-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83602-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83602-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83602-126">Not supported.</span></span>    |
|<span data-ttu-id="83602-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83602-127">Application</span></span> | <span data-ttu-id="83602-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83602-128">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="83602-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83602-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="83602-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83602-130">Request headers</span></span>
| <span data-ttu-id="83602-131">Имя</span><span class="sxs-lookup"><span data-stu-id="83602-131">Name</span></span>       | <span data-ttu-id="83602-132">Описание</span><span class="sxs-lookup"><span data-stu-id="83602-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="83602-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83602-133">Authorization</span></span>  | <span data-ttu-id="83602-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83602-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="83602-136">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="83602-136">Workbook-Session-Id</span></span>  | <span data-ttu-id="83602-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="83602-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="83602-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83602-139">Request body</span></span>
<span data-ttu-id="83602-140">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="83602-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="83602-141">Параметр</span><span class="sxs-lookup"><span data-stu-id="83602-141">Parameter</span></span>    | <span data-ttu-id="83602-142">Тип</span><span class="sxs-lookup"><span data-stu-id="83602-142">Type</span></span>   |<span data-ttu-id="83602-143">Описание</span><span class="sxs-lookup"><span data-stu-id="83602-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83602-144">index</span><span class="sxs-lookup"><span data-stu-id="83602-144">index</span></span>|<span data-ttu-id="83602-145">number</span><span class="sxs-lookup"><span data-stu-id="83602-145">number</span></span>|<span data-ttu-id="83602-p107">Необязательный параметр. Определяет относительную позицию новой строки. Если параметру присвоено значение null, строка добавляется в конце. Все строки ниже вставляемой строки сдвигаются вниз. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="83602-p107">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="83602-151">values</span><span class="sxs-lookup"><span data-stu-id="83602-151">values</span></span>|<span data-ttu-id="83602-152">Json</span><span class="sxs-lookup"><span data-stu-id="83602-152">Json</span></span>|<span data-ttu-id="83602-153">Двухмерный массив неформатированные значений строк таблицы (логическое значение или строка или номер).</span><span class="sxs-lookup"><span data-stu-id="83602-153">A 2-dimensional array of unformatted values of the table rows (boolean or string or number).</span></span>|

## <a name="response"></a><span data-ttu-id="83602-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="83602-154">Response</span></span>

<span data-ttu-id="83602-155">В случае успеха этот метод возвращает код отклика `200 OK` и объект [TableRow](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="83602-155">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83602-156">Пример</span><span class="sxs-lookup"><span data-stu-id="83602-156">Example</span></span>
<span data-ttu-id="83602-157">В этом примере в конец таблицы вставляются двух строк данных.</span><span class="sxs-lookup"><span data-stu-id="83602-157">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="83602-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="83602-158">Request</span></span>
<span data-ttu-id="83602-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83602-159">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="83602-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="83602-160">Response</span></span>
<span data-ttu-id="83602-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="83602-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
