---
title: 'TableRowCollection: add'
description: 'Добавляет строки в конец таблицы. Обратите внимание на то, что API может принимать несколько строк данных, с помощью этот интерфейс API. Добавление одной строке за раз может привести к снижению производительности. Рекомендуемый подход бы для пакетной обработки строк в один вызов, а не выполнив одну строку вставки. Для достижения наилучших результатов собирать строки, чтобы вставить в части приложения и выполнить отдельных строк добавьте операции. Поэкспериментируйте с номером строки, чтобы определить, идеальная число строк для использования в одном вызове API. '
ms.openlocfilehash: fc2b89a25ade4b9d85844716370d95d52689de9d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025925"
---
# <a name="tablerowcollection-add"></a><span data-ttu-id="1da0b-108">TableRowCollection: add</span><span class="sxs-lookup"><span data-stu-id="1da0b-108">TableRowCollection: add</span></span>

<span data-ttu-id="1da0b-109">Добавляет строки в конец таблицы.</span><span class="sxs-lookup"><span data-stu-id="1da0b-109">Adds rows to the end of the table.</span></span> <span data-ttu-id="1da0b-110">Обратите внимание на то, что API может принимать несколько строк данных, с помощью этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="1da0b-110">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="1da0b-111">Добавление одной строке за раз может привести к снижению производительности.</span><span class="sxs-lookup"><span data-stu-id="1da0b-111">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="1da0b-112">Рекомендуемый подход бы для пакетной обработки строк в один вызов, а не выполнив одну строку вставки.</span><span class="sxs-lookup"><span data-stu-id="1da0b-112">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="1da0b-113">Для достижения наилучших результатов собирать строки, чтобы вставить в части приложения и выполнить отдельных строк добавьте операции.</span><span class="sxs-lookup"><span data-stu-id="1da0b-113">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="1da0b-114">Поэкспериментируйте с номером строки, чтобы определить, идеальная число строк для использования в одном вызове API.</span><span class="sxs-lookup"><span data-stu-id="1da0b-114">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="1da0b-115">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="1da0b-115">Error Handling</span></span>

<span data-ttu-id="1da0b-116">Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP.</span><span class="sxs-lookup"><span data-stu-id="1da0b-116">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="1da0b-117">В этом случае нужно повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="1da0b-117">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="1da0b-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1da0b-118">Permissions</span></span>
<span data-ttu-id="1da0b-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1da0b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1da0b-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1da0b-121">Permission type</span></span>      | <span data-ttu-id="1da0b-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1da0b-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1da0b-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1da0b-123">Delegated (work or school account)</span></span> | <span data-ttu-id="1da0b-124">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1da0b-124">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1da0b-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1da0b-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1da0b-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1da0b-126">Not supported.</span></span>    |
|<span data-ttu-id="1da0b-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1da0b-127">Application</span></span> | <span data-ttu-id="1da0b-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1da0b-128">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1da0b-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1da0b-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="1da0b-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1da0b-130">Request headers</span></span>
| <span data-ttu-id="1da0b-131">Имя</span><span class="sxs-lookup"><span data-stu-id="1da0b-131">Name</span></span>       | <span data-ttu-id="1da0b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1da0b-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1da0b-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1da0b-133">Authorization</span></span>  | <span data-ttu-id="1da0b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1da0b-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1da0b-136">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1da0b-136">Workbook-Session-Id</span></span>  | <span data-ttu-id="1da0b-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="1da0b-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1da0b-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1da0b-139">Request body</span></span>
<span data-ttu-id="1da0b-140">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1da0b-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1da0b-141">Параметр</span><span class="sxs-lookup"><span data-stu-id="1da0b-141">Parameter</span></span>    | <span data-ttu-id="1da0b-142">Тип</span><span class="sxs-lookup"><span data-stu-id="1da0b-142">Type</span></span>   |<span data-ttu-id="1da0b-143">Описание</span><span class="sxs-lookup"><span data-stu-id="1da0b-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1da0b-144">index</span><span class="sxs-lookup"><span data-stu-id="1da0b-144">index</span></span>|<span data-ttu-id="1da0b-145">Int32</span><span class="sxs-lookup"><span data-stu-id="1da0b-145">Int32</span></span>|<span data-ttu-id="1da0b-p107">Необязательный параметр. Определяет относительную позицию новой строки. Если параметру присвоено значение null, строка добавляется в конце. Все строки ниже вставляемой строки сдвигаются вниз. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="1da0b-p107">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="1da0b-151">values</span><span class="sxs-lookup"><span data-stu-id="1da0b-151">values</span></span>|<span data-ttu-id="1da0b-152">Json</span><span class="sxs-lookup"><span data-stu-id="1da0b-152">Json</span></span>|<span data-ttu-id="1da0b-p108">Необязательный параметр. Двухмерный массив неформатированных значений строки таблицы.</span><span class="sxs-lookup"><span data-stu-id="1da0b-p108">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="1da0b-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="1da0b-155">Response</span></span>

<span data-ttu-id="1da0b-156">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [WorkbookTableRow](../resources/tablerow.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1da0b-156">If successful, this method returns `200 OK` response code and [WorkbookTableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1da0b-157">Пример</span><span class="sxs-lookup"><span data-stu-id="1da0b-157">Example</span></span>
<span data-ttu-id="1da0b-158">В этом примере в конец таблицы вставляются двух строк данных.</span><span class="sxs-lookup"><span data-stu-id="1da0b-158">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="1da0b-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="1da0b-159">Request</span></span>
<span data-ttu-id="1da0b-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1da0b-160">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="1da0b-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="1da0b-161">Response</span></span>
<span data-ttu-id="1da0b-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="1da0b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Warning: /api-reference/v1.0/api/tablerowcollection-add.md/tablerowcollection_add/values:
      Inconsistent types between parameter (Collection) and table (None)",
    "Error: /api-reference/v1.0/api/tablerowcollection-add.md/tablerowcollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Collection)) is a collection, while the table description type (microsoft.graph.Json) is not."
  ],
  "tocPath": ""
}-->
