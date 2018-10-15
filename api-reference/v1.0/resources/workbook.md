# <a name="workbook-resource-type"></a><span data-ttu-id="38273-101">Тип ресурса workbook</span><span class="sxs-lookup"><span data-stu-id="38273-101">Workbook resource type</span></span>

<span data-ttu-id="38273-102">Workbook — это объект верхнего уровня, содержащий связанные объекты книг, например листы, таблицы, диапазоны и т. д.</span><span class="sxs-lookup"><span data-stu-id="38273-102">Workbook is the top level object which contains related workbook objects such as worksheets, tables, ranges, etc.</span></span>

## <a name="json-representation"></a><span data-ttu-id="38273-103">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38273-103">JSON representation</span></span>

<span data-ttu-id="38273-104">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="38273-104">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="38273-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="38273-105">Properties</span></span>
<span data-ttu-id="38273-106">Нет</span><span class="sxs-lookup"><span data-stu-id="38273-106">None</span></span>

## <a name="methods"></a><span data-ttu-id="38273-107">Методы</span><span class="sxs-lookup"><span data-stu-id="38273-107">Methods</span></span>

| <span data-ttu-id="38273-108">Метод</span><span class="sxs-lookup"><span data-stu-id="38273-108">Method</span></span>       | <span data-ttu-id="38273-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="38273-109">Return Type</span></span>  |<span data-ttu-id="38273-110">Описание</span><span class="sxs-lookup"><span data-stu-id="38273-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="38273-111">Create Session</span><span class="sxs-lookup"><span data-stu-id="38273-111">Create Session</span></span>](../api/workbook_createsession.md) | [<span data-ttu-id="38273-112">workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="38273-112">workbookSessionInfo</span></span>](workbooksessioninfo.md) |<span data-ttu-id="38273-113">Создание сеанса книги для запуска сохраняемого или несохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="38273-113">Create a workbook session to start a persistent or non-persistent session.</span></span>|
|[<span data-ttu-id="38273-114">Close Session</span><span class="sxs-lookup"><span data-stu-id="38273-114">Close Session</span></span>](../api/workbook_closesession.md) | <span data-ttu-id="38273-115">Нет</span><span class="sxs-lookup"><span data-stu-id="38273-115">None</span></span> |<span data-ttu-id="38273-116">Закрытие существующего сеанса.</span><span class="sxs-lookup"><span data-stu-id="38273-116">Close an existing session.</span></span>|
|[<span data-ttu-id="38273-117">Refresh Session</span><span class="sxs-lookup"><span data-stu-id="38273-117">Refresh Session</span></span>](../api/workbook_refreshsession.md) | <span data-ttu-id="38273-118">Нет</span><span class="sxs-lookup"><span data-stu-id="38273-118">None</span></span> |<span data-ttu-id="38273-119">Обновление существующего сеанса.</span><span class="sxs-lookup"><span data-stu-id="38273-119">Refresh an existing session.</span></span>|


## <a name="relationships"></a><span data-ttu-id="38273-120">Связи</span><span class="sxs-lookup"><span data-stu-id="38273-120">Relationships</span></span>
| <span data-ttu-id="38273-121">Связь</span><span class="sxs-lookup"><span data-stu-id="38273-121">Relationship</span></span> | <span data-ttu-id="38273-122">Тип</span><span class="sxs-lookup"><span data-stu-id="38273-122">Type</span></span>   |<span data-ttu-id="38273-123">Описание</span><span class="sxs-lookup"><span data-stu-id="38273-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38273-124">names</span><span class="sxs-lookup"><span data-stu-id="38273-124">names</span></span>|<span data-ttu-id="38273-125">Коллекция [WorkbookNamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="38273-125">[WorkbookNamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="38273-p101">Представляет коллекцию именованных элементов в книге (именованные диапазоны и константы). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38273-p101">Represents a collection of workbook scoped named items (named ranges and constants). Read-only.</span></span>|
|<span data-ttu-id="38273-128">tables</span><span class="sxs-lookup"><span data-stu-id="38273-128">tables</span></span>|<span data-ttu-id="38273-129">Коллекция [WorkbookTable](table.md)</span><span class="sxs-lookup"><span data-stu-id="38273-129">[WorkbookTable](table.md) collection</span></span>|<span data-ttu-id="38273-p102">Представляет коллекцию таблиц, сопоставленных с книгой. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38273-p102">Represents a collection of tables associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="38273-132">worksheets</span><span class="sxs-lookup"><span data-stu-id="38273-132">worksheets</span></span>|<span data-ttu-id="38273-133">Коллекция [WorkbookWorksheet](worksheet.md)</span><span class="sxs-lookup"><span data-stu-id="38273-133">[WorkbookWorksheet](worksheet.md) collection</span></span>|<span data-ttu-id="38273-p103">Представляет коллекцию листов, связанных с книгой. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38273-p103">Represents a collection of worksheets associated with the workbook. Read-only.</span></span>|

## <a name="functions"></a><span data-ttu-id="38273-136">Функции</span><span class="sxs-lookup"><span data-stu-id="38273-136">Functions</span></span>

<span data-ttu-id="38273-p104">[Функции Excel](#functions): вызов функции книги с использованием синтаксиса `POST /workbook/functions/{function-name}` и предоставление аргументов функции в основном тексте с помощью объекта JSON. Результирующее `value` функции и любые строки `error` возвращаются в объекте результата функции. Если значение `error` равно `null`, это свидетельствует об успешном выполнении функции.</span><span class="sxs-lookup"><span data-stu-id="38273-p104">[Excel functions](#functions): Invoke a workbook function using the syntax `POST /workbook/functions/{function-name}` and providing the function argument(s) in the body using a JSON object. The function's resulting `value` and any `error` strings are returned in the function result object. The `error` value of `null` indicates successful execution of the function.</span></span> 

<span data-ttu-id="38273-p105">Полный список поддерживаемых функций см. [здесь](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Имена определенных параметров и типы данных см. в сигнатуре функции.</span><span class="sxs-lookup"><span data-stu-id="38273-p105">The complete list of supported functions are listed [here](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="38273-142">_Важные примечания._</span><span class="sxs-lookup"><span data-stu-id="38273-142">_Important notes:_</span></span> 
* <span data-ttu-id="38273-143">Входной параметр range предоставляется с использованием объекта range вместо строки адреса range.</span><span class="sxs-lookup"><span data-stu-id="38273-143">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="38273-144">Параметр index индексируется с 1, а не с 0, как в большинстве API.</span><span class="sxs-lookup"><span data-stu-id="38273-144">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span> 

<span data-ttu-id="38273-145">Пример: **vlookup**.</span><span class="sxs-lookup"><span data-stu-id="38273-145">Example: **vlookup**</span></span>

<span data-ttu-id="38273-146">В электронной таблице Excel функция `vlookup` принимает следующие аргументы:</span><span class="sxs-lookup"><span data-stu-id="38273-146">In an Excel spreadsheet, the `vlookup` function takes the following arguments:</span></span>

1. <span data-ttu-id="38273-147">Значение, которое вы хотите найти. Его также называют искомым значением.</span><span class="sxs-lookup"><span data-stu-id="38273-147">The value you want to look up, also called the lookup value.</span></span>
2. <span data-ttu-id="38273-148">Диапазон, в котором находится искомое значение.</span><span class="sxs-lookup"><span data-stu-id="38273-148">The range where the lookup value is located.</span></span> <span data-ttu-id="38273-149">Помните, что искомое значение должно находиться всегда в первом столбце в диапазоне ВПР. В ином случае его обработка не будет выполняться правильно.</span><span class="sxs-lookup"><span data-stu-id="38273-149">Remember that the lookup value should always be in the first column in the range for VLOOKUP to work correctly.</span></span> <span data-ttu-id="38273-150">Например, если искомое значение находится в ячейке C2, диапазон должен начинаться с C.</span><span class="sxs-lookup"><span data-stu-id="38273-150">For example, if your lookup value is in cell C2 then your range should start with C.</span></span>
3. <span data-ttu-id="38273-151">Номер столбца в диапазоне, который содержит возвращаемое значение.</span><span class="sxs-lookup"><span data-stu-id="38273-151">The column number in the range that contains the return value.</span></span> <span data-ttu-id="38273-152">Например, если вы укажете в качестве диапазона B2:D11, B будет первым столбцом, C — вторым и т. д.</span><span class="sxs-lookup"><span data-stu-id="38273-152">For example, if you specify B2: D11 as the range, you should count B as the first column, C as the second, and so on.</span></span>
4. <span data-ttu-id="38273-153">При желании вы можете указать TRUE, если нужно приблизительное совпадение, и FALSE, если нужно точное совпадение возвращаемого значения.</span><span class="sxs-lookup"><span data-stu-id="38273-153">Optionally, you can specify TRUE if you want an approximate match or FALSE if you want an exact match of the return value.</span></span> <span data-ttu-id="38273-154">Если вы ничего не укажете, значением по умолчанию будет TRUE (приблизительное совпадение).</span><span class="sxs-lookup"><span data-stu-id="38273-154">If you don't specify anything, the default value will always be TRUE or approximate match.</span></span>

<span data-ttu-id="38273-155">В ячейке функция `vlookup` выглядит так:</span><span class="sxs-lookup"><span data-stu-id="38273-155">Inside a cell, the `vlookup` function looks like this:</span></span> 

<span data-ttu-id="38273-156">=ВПР(искомое значение, диапазон с искомым значением, номер столбца в диапазоне с возвращаемым значением, необязательное значение TRUE для указания приблизительного значения или FALSE для указания точного совпадения)</span><span class="sxs-lookup"><span data-stu-id="38273-156">=VLOOKUP(lookup value, range containing the lookup value, the column number in the range containing the return value, optionally specify TRUE for approximate match or FALSE for an exact match)</span></span>

<span data-ttu-id="38273-157">(См. документацию по [функции ВПР в Excel](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span><span class="sxs-lookup"><span data-stu-id="38273-157">(See the documentation for the [VLOOKUP Excel function](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span></span>

<span data-ttu-id="38273-158">В приведенном ниже примере показано, как вызывать функцию `vlookup` и передавать эти параметры с помощью REST API для Excel.</span><span class="sxs-lookup"><span data-stu-id="38273-158">The example below shows how to call the `vlookup` function and pass these parameters with the Excel REST API.</span></span>

<span data-ttu-id="38273-159">Запрос:</span><span class="sxs-lookup"><span data-stu-id="38273-159">Request:</span></span> 

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

<span data-ttu-id="38273-160">Отклик:</span><span class="sxs-lookup"><span data-stu-id="38273-160">Response:</span></span>

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

<span data-ttu-id="38273-161">Пример: `median`. `median`</span><span class="sxs-lookup"><span data-stu-id="38273-161">Example: `median`</span></span>

<span data-ttu-id="38273-162">В электронной таблице Excel функция `median` принимает массив одного или нескольких диапазонов входных значений.</span><span class="sxs-lookup"><span data-stu-id="38273-162">In an Excel spreadsheet, the `median` function takes an array of one or more input ranges.</span></span>

<span data-ttu-id="38273-163">В ячейке функция `median` выглядит так, как показано в этом примере:</span><span class="sxs-lookup"><span data-stu-id="38273-163">Inside a cell, the `median` function looks like this example:</span></span>

<span data-ttu-id="38273-164">=МЕДИАНА(A2:A6)</span><span class="sxs-lookup"><span data-stu-id="38273-164">=MEDIAN(A2:A6)</span></span>

<span data-ttu-id="38273-165">(См. документацию по [функции МЕДИАНА в Excel](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span><span class="sxs-lookup"><span data-stu-id="38273-165">(See the documentation for the [MEDIAN Excel function](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span></span>

<span data-ttu-id="38273-166">В приведенном ниже примере показано, как вызывать функцию `median` и один или несколько диапазонов входных значений с помощью REST API для Excel.</span><span class="sxs-lookup"><span data-stu-id="38273-166">The example below shows how to call the `median` function and one or more input ranges with the Excel REST API.</span></span> 

<span data-ttu-id="38273-167">Запрос:</span><span class="sxs-lookup"><span data-stu-id="38273-167">Request:</span></span> 

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

<span data-ttu-id="38273-168">Отклик:</span><span class="sxs-lookup"><span data-stu-id="38273-168">Response:</span></span>

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
