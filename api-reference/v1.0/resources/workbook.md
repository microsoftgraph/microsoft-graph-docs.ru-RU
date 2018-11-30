---
title: Тип ресурса workbook
description: Workbook — это объект верхнего уровня, содержащий связанные объекты книг, например листы, таблицы, диапазоны и т. д.
ms.openlocfilehash: 6575cc2d49e4b30e78e07989f38600ae64d5c5a5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026436"
---
# <a name="workbook-resource-type"></a><span data-ttu-id="88b87-103">Тип ресурса workbook</span><span class="sxs-lookup"><span data-stu-id="88b87-103">Workbook resource type</span></span>

<span data-ttu-id="88b87-104">Workbook — это объект верхнего уровня, содержащий связанные объекты книг, например листы, таблицы, диапазоны и т. д.</span><span class="sxs-lookup"><span data-stu-id="88b87-104">Workbook is the top level object which contains related workbook objects such as worksheets, tables, ranges, etc.</span></span>

## <a name="json-representation"></a><span data-ttu-id="88b87-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88b87-105">JSON representation</span></span>

<span data-ttu-id="88b87-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="88b87-106">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbook"
}-->

```json
{
  "names": [{"@odata.type": "microsoft.graph.workbookNamedItem"}],
  "tables": [{"@odata.type": "microsoft.graph.workbookTable"}],
  "worksheets": [{"@odata.type": "microsoft.graph.workbookWorksheet"}]
}
```

## <a name="properties"></a><span data-ttu-id="88b87-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="88b87-107">Properties</span></span>
<span data-ttu-id="88b87-108">Нет</span><span class="sxs-lookup"><span data-stu-id="88b87-108">None</span></span>

## <a name="methods"></a><span data-ttu-id="88b87-109">Методы</span><span class="sxs-lookup"><span data-stu-id="88b87-109">Methods</span></span>

| <span data-ttu-id="88b87-110">Метод</span><span class="sxs-lookup"><span data-stu-id="88b87-110">Method</span></span>       | <span data-ttu-id="88b87-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="88b87-111">Return Type</span></span>  |<span data-ttu-id="88b87-112">Описание</span><span class="sxs-lookup"><span data-stu-id="88b87-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="88b87-113">Create Session</span><span class="sxs-lookup"><span data-stu-id="88b87-113">Create Session</span></span>](../api/workbook-createsession.md) | [<span data-ttu-id="88b87-114">workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="88b87-114">workbookSessionInfo</span></span>](workbooksessioninfo.md) |<span data-ttu-id="88b87-115">Создание сеанса книги для запуска сохраняемого или несохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="88b87-115">Create a workbook session to start a persistent or non-persistent session.</span></span>|
|[<span data-ttu-id="88b87-116">Close Session</span><span class="sxs-lookup"><span data-stu-id="88b87-116">Close Session</span></span>](../api/workbook-closesession.md) | <span data-ttu-id="88b87-117">Нет</span><span class="sxs-lookup"><span data-stu-id="88b87-117">None</span></span> |<span data-ttu-id="88b87-118">Закрытие существующего сеанса.</span><span class="sxs-lookup"><span data-stu-id="88b87-118">Close an existing session.</span></span>|
|[<span data-ttu-id="88b87-119">Refresh Session</span><span class="sxs-lookup"><span data-stu-id="88b87-119">Refresh Session</span></span>](../api/workbook-refreshsession.md) | <span data-ttu-id="88b87-120">Нет</span><span class="sxs-lookup"><span data-stu-id="88b87-120">None</span></span> |<span data-ttu-id="88b87-121">Обновление существующего сеанса.</span><span class="sxs-lookup"><span data-stu-id="88b87-121">Refresh an existing session.</span></span>|


## <a name="relationships"></a><span data-ttu-id="88b87-122">Связи</span><span class="sxs-lookup"><span data-stu-id="88b87-122">Relationships</span></span>
| <span data-ttu-id="88b87-123">Связь</span><span class="sxs-lookup"><span data-stu-id="88b87-123">Relationship</span></span> | <span data-ttu-id="88b87-124">Тип</span><span class="sxs-lookup"><span data-stu-id="88b87-124">Type</span></span>   |<span data-ttu-id="88b87-125">Описание</span><span class="sxs-lookup"><span data-stu-id="88b87-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88b87-126">names</span><span class="sxs-lookup"><span data-stu-id="88b87-126">names</span></span>|<span data-ttu-id="88b87-127">[WorkbookNamedItem](nameditem.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="88b87-127">[WorkbookNamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="88b87-p101">Представляет коллекцию именованных элементов в книге (именованные диапазоны и константы). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88b87-p101">Represents a collection of workbook scoped named items (named ranges and constants). Read-only.</span></span>|
|<span data-ttu-id="88b87-130">tables</span><span class="sxs-lookup"><span data-stu-id="88b87-130">tables</span></span>|<span data-ttu-id="88b87-131">[WorkbookTable](table.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="88b87-131">[WorkbookTable](table.md) collection</span></span>|<span data-ttu-id="88b87-p102">Представляет коллекцию таблиц, сопоставленных с книгой. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88b87-p102">Represents a collection of tables associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="88b87-134">worksheets</span><span class="sxs-lookup"><span data-stu-id="88b87-134">worksheets</span></span>|<span data-ttu-id="88b87-135">[WorkbookWorksheet](worksheet.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="88b87-135">[WorkbookWorksheet](worksheet.md) collection</span></span>|<span data-ttu-id="88b87-p103">Представляет коллекцию листов, сопоставленных с книгой. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88b87-p103">Represents a collection of worksheets associated with the workbook. Read-only.</span></span>|

## <a name="functions"></a><span data-ttu-id="88b87-138">Функции</span><span class="sxs-lookup"><span data-stu-id="88b87-138">Functions</span></span>

<span data-ttu-id="88b87-p104">[Функции Excel](#functions): вызов функции книги с использованием синтаксиса `POST /workbook/functions/{function-name}` и предоставление аргументов функции в основном тексте с помощью объекта JSON. Результирующее `value` функции и любые строки `error` возвращаются в объекте результата функции. Если значение `error` равно `null`, это свидетельствует об успешном выполнении функции.</span><span class="sxs-lookup"><span data-stu-id="88b87-p104">[Excel functions](#functions): Invoke a workbook function using the syntax `POST /workbook/functions/{function-name}` and providing the function argument(s) in the body using a JSON object. The function's resulting `value` and any `error` strings are returned in the function result object. The `error` value of `null` indicates successful execution of the function.</span></span> 

<span data-ttu-id="88b87-p105">Полный список поддерживаемых функций см. [здесь](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Имена определенных параметров и типы данных см. в сигнатуре функции.</span><span class="sxs-lookup"><span data-stu-id="88b87-p105">The complete list of supported functions are listed [here](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="88b87-144">_Важные примечания._</span><span class="sxs-lookup"><span data-stu-id="88b87-144">_Important notes:_</span></span> 
* <span data-ttu-id="88b87-145">Входной параметр range предоставляется с использованием объекта range вместо строки адреса range.</span><span class="sxs-lookup"><span data-stu-id="88b87-145">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="88b87-146">Параметр index индексируется с 1, а не с 0, как в большинстве API.</span><span class="sxs-lookup"><span data-stu-id="88b87-146">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span> 

<span data-ttu-id="88b87-147">Пример: **vlookup**.</span><span class="sxs-lookup"><span data-stu-id="88b87-147">Example: **vlookup**</span></span>

<span data-ttu-id="88b87-148">В электронной таблице Excel функция `vlookup` принимает следующие аргументы:</span><span class="sxs-lookup"><span data-stu-id="88b87-148">In an Excel spreadsheet, the `vlookup` function takes the following arguments:</span></span>

1. <span data-ttu-id="88b87-149">Значение, которое вы хотите найти. Его также называют искомым значением.</span><span class="sxs-lookup"><span data-stu-id="88b87-149">The value you want to look up, also called the lookup value.</span></span>
2. <span data-ttu-id="88b87-150">Диапазон, в котором находится искомое значение.</span><span class="sxs-lookup"><span data-stu-id="88b87-150">The range where the lookup value is located.</span></span> <span data-ttu-id="88b87-151">Помните, что искомое значение должно находиться всегда в первом столбце в диапазоне ВПР. В ином случае его обработка не будет выполняться правильно.</span><span class="sxs-lookup"><span data-stu-id="88b87-151">Remember that the lookup value should always be in the first column in the range for VLOOKUP to work correctly.</span></span> <span data-ttu-id="88b87-152">Например, если искомое значение находится в ячейке C2, диапазон должен начинаться с C.</span><span class="sxs-lookup"><span data-stu-id="88b87-152">For example, if your lookup value is in cell C2 then your range should start with C.</span></span>
3. <span data-ttu-id="88b87-153">Номер столбца в диапазоне, который содержит возвращаемое значение.</span><span class="sxs-lookup"><span data-stu-id="88b87-153">The column number in the range that contains the return value.</span></span> <span data-ttu-id="88b87-154">Например, если вы укажете в качестве диапазона B2:D11, B будет первым столбцом, C — вторым и т. д.
</span><span class="sxs-lookup"><span data-stu-id="88b87-154">For example, if you specify B2: D11 as the range, you should count B as the first column, C as the second, and so on.</span></span>
4. <span data-ttu-id="88b87-155">При желании вы можете указать TRUE, если нужно приблизительное совпадение, и FALSE, если нужно точное совпадение возвращаемого значения.</span><span class="sxs-lookup"><span data-stu-id="88b87-155">Optionally, you can specify TRUE if you want an approximate match or FALSE if you want an exact match of the return value.</span></span> <span data-ttu-id="88b87-156">Если вы ничего не укажете, значением по умолчанию будет TRUE (приблизительное совпадение).</span><span class="sxs-lookup"><span data-stu-id="88b87-156">If you don't specify anything, the default value will always be TRUE or approximate match.</span></span>

<span data-ttu-id="88b87-157">В ячейке функция `vlookup` выглядит так:</span><span class="sxs-lookup"><span data-stu-id="88b87-157">Inside a cell, the `vlookup` function looks like this:</span></span> 

<span data-ttu-id="88b87-158">=ВПР(искомое значение, диапазон с искомым значением, номер столбца в диапазоне с возвращаемым значением, необязательное значение TRUE для указания приблизительного значения или FALSE для указания точного совпадения)</span><span class="sxs-lookup"><span data-stu-id="88b87-158">=VLOOKUP(lookup value, range containing the lookup value, the column number in the range containing the return value, optionally specify TRUE for approximate match or FALSE for an exact match)</span></span>

<span data-ttu-id="88b87-159">(См. документацию по [функции ВПР в Excel](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span><span class="sxs-lookup"><span data-stu-id="88b87-159">(See the documentation for the [VLOOKUP Excel function](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span></span>

<span data-ttu-id="88b87-160">В приведенном ниже примере показано, как вызывать функцию `vlookup` и передавать эти параметры с помощью REST API для Excel.</span><span class="sxs-lookup"><span data-stu-id="88b87-160">The example below shows how to call the `vlookup` function and pass these parameters with the Excel REST API.</span></span>

<span data-ttu-id="88b87-161">Запрос:</span><span class="sxs-lookup"><span data-stu-id="88b87-161">Request:</span></span> 

```http 
POST https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/vlookup
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
    "lookupValue": "Temperature",
    "tableArray": { "Address": "Sheet1!E1:G5" },
    "colIndexNum": 2,
    "rangeLookup": false
}
```

<span data-ttu-id="88b87-162">Отклик:</span><span class="sxs-lookup"><span data-stu-id="88b87-162">Response:</span></span>

```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/vlookup()",
    "error": null,
    "value": "28.3"
}
```

<span data-ttu-id="88b87-163">Пример: `median`.</span><span class="sxs-lookup"><span data-stu-id="88b87-163">Example: `median`</span></span>

<span data-ttu-id="88b87-164">В электронной таблице Excel функция `median` принимает массив одного или нескольких диапазонов входных значений.</span><span class="sxs-lookup"><span data-stu-id="88b87-164">In an Excel spreadsheet, the `median` function takes an array of one or more input ranges.</span></span>

<span data-ttu-id="88b87-165">В ячейке функция `median` выглядит так, как показано в этом примере:</span><span class="sxs-lookup"><span data-stu-id="88b87-165">Inside a cell, the `median` function looks like this example:</span></span>

<span data-ttu-id="88b87-166">=МЕДИАНА(A2:A6)</span><span class="sxs-lookup"><span data-stu-id="88b87-166">=MEDIAN(A2:A6)</span></span>

<span data-ttu-id="88b87-167">(См. документацию по [функции МЕДИАНА в Excel](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span><span class="sxs-lookup"><span data-stu-id="88b87-167">(See the documentation for the [MEDIAN Excel function](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span></span>

<span data-ttu-id="88b87-168">В приведенном ниже примере показано, как вызывать функцию `median` и один или несколько диапазонов входных значений с помощью REST API для Excel.</span><span class="sxs-lookup"><span data-stu-id="88b87-168">The example below shows how to call the `median` function and one or more input ranges with the Excel REST API.</span></span> 

<span data-ttu-id="88b87-169">Запрос:</span><span class="sxs-lookup"><span data-stu-id="88b87-169">Request:</span></span> 

```http 
POST https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/median
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"values" :  [
        { "address": "Sheet2!A1:A5" },
        { "address": "Sheet2!B1:B5" },
      ] 
}
```

<span data-ttu-id="88b87-170">Отклик:</span><span class="sxs-lookup"><span data-stu-id="88b87-170">Response:</span></span>

```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
  "@odata.type": "#microsoft.graph.workbookFunctionResult",
  "@odata.id": "/users('2abcad6a-2fca-4b6e-9577-e358a757d77d')/drive/root/workbook/functions/median()",
  "error": null,
  "value": 30
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Workbook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
