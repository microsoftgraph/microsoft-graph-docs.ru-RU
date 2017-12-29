# <a name="workbook-resource-type"></a><span data-ttu-id="589a4-101">Тип ресурса workbook</span><span class="sxs-lookup"><span data-stu-id="589a4-101">Workbook resource type</span></span>

<span data-ttu-id="589a4-102">Workbook — это объект верхнего уровня, содержащий связанные объекты книг, например листы, таблицы, диапазоны и т. д.</span><span class="sxs-lookup"><span data-stu-id="589a4-102">Workbook is the top level object which contains related workbook objects such as worksheets, tables, ranges, etc.</span></span>

## <a name="properties"></a><span data-ttu-id="589a4-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="589a4-103">Properties</span></span>
<span data-ttu-id="589a4-104">Нет</span><span class="sxs-lookup"><span data-stu-id="589a4-104">None</span></span>

## <a name="methods"></a><span data-ttu-id="589a4-105">Методы</span><span class="sxs-lookup"><span data-stu-id="589a4-105">Methods</span></span>

| <span data-ttu-id="589a4-106">Метод</span><span class="sxs-lookup"><span data-stu-id="589a4-106">Method</span></span>       | <span data-ttu-id="589a4-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="589a4-107">Return Type</span></span>  |<span data-ttu-id="589a4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="589a4-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="589a4-109">Create Session</span><span class="sxs-lookup"><span data-stu-id="589a4-109">Create Session</span></span>](../api/workbook_createsession.md) | [<span data-ttu-id="589a4-110">workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="589a4-110">workbookSessionInfo</span></span>](workbooksessioninfo.md) |<span data-ttu-id="589a4-111">Создание сеанса книги для запуска сохраняемого или несохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="589a4-111">Create a workbook session to start a persistent or non-persistent session.</span></span>|
|[<span data-ttu-id="589a4-112">Close Session</span><span class="sxs-lookup"><span data-stu-id="589a4-112">Close Session</span></span>](../api/workbook_closesession.md) | <span data-ttu-id="589a4-113">Нет</span><span class="sxs-lookup"><span data-stu-id="589a4-113">None</span></span> |<span data-ttu-id="589a4-114">Закрытие существующего сеанса.</span><span class="sxs-lookup"><span data-stu-id="589a4-114">Close an existing session.</span></span>|
|[<span data-ttu-id="589a4-115">Refresh Session</span><span class="sxs-lookup"><span data-stu-id="589a4-115">Refresh Session</span></span>](../api/workbook_refreshsession.md) | <span data-ttu-id="589a4-116">Нет</span><span class="sxs-lookup"><span data-stu-id="589a4-116">None</span></span> |<span data-ttu-id="589a4-117">Обновление существующего сеанса.</span><span class="sxs-lookup"><span data-stu-id="589a4-117">Refresh an existing session.</span></span>|


## <a name="relationships"></a><span data-ttu-id="589a4-118">Связи</span><span class="sxs-lookup"><span data-stu-id="589a4-118">Relationships</span></span>
| <span data-ttu-id="589a4-119">Связь</span><span class="sxs-lookup"><span data-stu-id="589a4-119">Relationship</span></span> | <span data-ttu-id="589a4-120">Тип</span><span class="sxs-lookup"><span data-stu-id="589a4-120">Type</span></span>   |<span data-ttu-id="589a4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="589a4-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="589a4-122">names</span><span class="sxs-lookup"><span data-stu-id="589a4-122">names</span></span>|<span data-ttu-id="589a4-123">Коллекция объектов [NamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="589a4-123">[NamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="589a4-p101">Представляет коллекцию именованных элементов в книге (именованные диапазоны и константы). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="589a4-p101">Represents a collection of workbook scoped named items (named ranges and constants). Read-only.</span></span>|
|<span data-ttu-id="589a4-126">tables</span><span class="sxs-lookup"><span data-stu-id="589a4-126">tables</span></span>|<span data-ttu-id="589a4-127">Коллекция объектов [Table](table.md)</span><span class="sxs-lookup"><span data-stu-id="589a4-127">[Table](table.md) collection</span></span>|<span data-ttu-id="589a4-p102">Представляет коллекцию таблиц, сопоставленных с книгой. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="589a4-p102">Represents a collection of tables associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="589a4-130">worksheets</span><span class="sxs-lookup"><span data-stu-id="589a4-130">worksheets</span></span>|<span data-ttu-id="589a4-131">Коллекция объектов [Worksheet](worksheet.md)</span><span class="sxs-lookup"><span data-stu-id="589a4-131">[Worksheet](worksheet.md) collection</span></span>|<span data-ttu-id="589a4-p103">Представляет коллекцию листов, сопоставленных с книгой. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="589a4-p103">Represents a collection of worksheets associated with the workbook. Read-only.</span></span>|

## <a name="functions"></a><span data-ttu-id="589a4-134">Функции</span><span class="sxs-lookup"><span data-stu-id="589a4-134">Functions</span></span>

<span data-ttu-id="589a4-135">[Функции Excel](#functions): Вызов функции книги с использованием синтаксиса `POST /workbook/functions/{function-name}` и предоставление аргументов функции в теле с помощью объекта JSON.</span><span class="sxs-lookup"><span data-stu-id="589a4-135">[Excel functions](#functions): Invoke a workbook function using the syntax `POST /workbook/functions/{function-name}` and providing the function argument(s) in the body using a JSON object.</span></span> <span data-ttu-id="589a4-136">Результирующее `value` функции и все строки `error` возвращаются в объекте результата функции.</span><span class="sxs-lookup"><span data-stu-id="589a4-136">The function's resulting `value` and any `error` strings are returned in the function result object.</span></span> <span data-ttu-id="589a4-137">Если значение `error` равно `null`, это свидетельствует об успешном выполнении функции.</span><span class="sxs-lookup"><span data-stu-id="589a4-137">The `error` value of `null` indicates successful execution of the function.</span></span> 

<span data-ttu-id="589a4-138">Полный список поддерживаемых функций см. [здесь](https://support.office.com/ru-RU/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188).</span><span class="sxs-lookup"><span data-stu-id="589a4-138">The complete list of supported functions are listed [here](https://support.office.com/ru-RU/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188).</span></span> <span data-ttu-id="589a4-139">Имена определенных параметров и типы данных см. в сигнатуре функции.</span><span class="sxs-lookup"><span data-stu-id="589a4-139">Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="589a4-140">_Важные примечания._</span><span class="sxs-lookup"><span data-stu-id="589a4-140">_Important notes:_</span></span> 
* <span data-ttu-id="589a4-141">Входной параметр range предоставляется с использованием объекта range вместо строки адреса range.</span><span class="sxs-lookup"><span data-stu-id="589a4-141">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="589a4-142">Параметр index индексируется с 1, а не с 0, как в большинстве API.</span><span class="sxs-lookup"><span data-stu-id="589a4-142">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span> 

<span data-ttu-id="589a4-143">Пример: **vlookup**.</span><span class="sxs-lookup"><span data-stu-id="589a4-143">Example: **vlookup**</span></span>

<span data-ttu-id="589a4-144">В электронной таблице Excel функция `vlookup` принимает следующие аргументы:</span><span class="sxs-lookup"><span data-stu-id="589a4-144">In an Excel spreadsheet, the `vlookup` function takes the following arguments:</span></span>

1. <span data-ttu-id="589a4-145">Значение, которое вы хотите найти. Его также называют искомым значением.</span><span class="sxs-lookup"><span data-stu-id="589a4-145">The value you want to look up, also called the lookup value.</span></span>
2. <span data-ttu-id="589a4-146">Диапазон, в котором находится искомое значение.</span><span class="sxs-lookup"><span data-stu-id="589a4-146">The range where the lookup value is located.</span></span> <span data-ttu-id="589a4-147">Помните, что искомое значение должно находиться всегда в первом столбце в диапазоне ВПР. В ином случае его обработка не будет выполняться правильно.</span><span class="sxs-lookup"><span data-stu-id="589a4-147">Remember that the lookup value should always be in the first column in the range for VLOOKUP to work correctly.</span></span> <span data-ttu-id="589a4-148">Например, если искомое значение находится в ячейке C2, диапазон должен начинаться с C.</span><span class="sxs-lookup"><span data-stu-id="589a4-148">For example, if your lookup value is in cell C2 then your range should start with C.</span></span>
3. <span data-ttu-id="589a4-149">Номер столбца в диапазоне, который содержит возвращаемое значение.</span><span class="sxs-lookup"><span data-stu-id="589a4-149">The column number in the range that contains the return value.</span></span> <span data-ttu-id="589a4-150">Например, если вы укажете в качестве диапазона B2:D11, B будет первым столбцом, C — вторым, и т. д.</span><span class="sxs-lookup"><span data-stu-id="589a4-150">For example, if you specify B2: D11 as the range, you should count B as the first column, C as the second, and so on.</span></span>
4. <span data-ttu-id="589a4-151">При желании вы можете указать TRUE, если нужно приблизительное совпадение, и FALSE, если нужно точное совпадение возвращаемого значения.</span><span class="sxs-lookup"><span data-stu-id="589a4-151">Optionally, you can specify TRUE if you want an approximate match or FALSE if you want an exact match of the return value.</span></span> <span data-ttu-id="589a4-152">Если вы ничего не укажете, значением по умолчанию будет TRUE (приблизительное совпадение).</span><span class="sxs-lookup"><span data-stu-id="589a4-152">If you don't specify anything, the default value will always be TRUE or approximate match.</span></span>

<span data-ttu-id="589a4-153">В ячейке функция `vlookup` выглядит так:</span><span class="sxs-lookup"><span data-stu-id="589a4-153">Inside a cell, the `vlookup` function looks like this:</span></span> 

<span data-ttu-id="589a4-154">=ВПР(искомое значение, диапазон с искомым значением, номер столбца в диапазоне с возвращаемым значением, необязательное значение TRUE для указания приблизительного значения или FALSE для указания точного совпадения)</span><span class="sxs-lookup"><span data-stu-id="589a4-154">=VLOOKUP(lookup value, range containing the lookup value, the column number in the range containing the return value, optionally specify TRUE for approximate match or FALSE for an exact match)</span></span>

<span data-ttu-id="589a4-155">(См. документацию по [функции ВПР в Excel](https://support.office.com/ru-RU/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span><span class="sxs-lookup"><span data-stu-id="589a4-155">(See the documentation for the [VLOOKUP Excel function](https://support.office.com/ru-RU/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span></span>

<span data-ttu-id="589a4-156">В приведенном ниже примере показано, как вызывать функцию `vlookup` и передавать эти параметры с помощью REST API для Excel.</span><span class="sxs-lookup"><span data-stu-id="589a4-156">The example below shows how to call the `vlookup` function and pass these parameters with the Excel REST API.</span></span>

<span data-ttu-id="589a4-157">Запрос:</span><span class="sxs-lookup"><span data-stu-id="589a4-157">Request:</span></span> 

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

<span data-ttu-id="589a4-158">Отклик:</span><span class="sxs-lookup"><span data-stu-id="589a4-158">Response:</span></span>

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

<span data-ttu-id="589a4-159">Пример: `median`.</span><span class="sxs-lookup"><span data-stu-id="589a4-159">Example: `median`</span></span>

<span data-ttu-id="589a4-160">В электронной таблице Excel функция `median` принимает массив одного или нескольких диапазонов входных значений.</span><span class="sxs-lookup"><span data-stu-id="589a4-160">In an Excel spreadsheet, the `median` function takes an array of one or more input ranges.</span></span>

<span data-ttu-id="589a4-161">В ячейке функция `median` выглядит так, как показано в этом примере:</span><span class="sxs-lookup"><span data-stu-id="589a4-161">Inside a cell, the `median` function looks like this example:</span></span>

<span data-ttu-id="589a4-162">=МЕДИАНА(A2:A6)</span><span class="sxs-lookup"><span data-stu-id="589a4-162">=MEDIAN(A2:A6)</span></span>

<span data-ttu-id="589a4-163">(См. документацию по [функции МЕДИАНА в Excel](https://support.office.com/ru-RU/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span><span class="sxs-lookup"><span data-stu-id="589a4-163">(See the documentation for the [MEDIAN Excel function](https://support.office.com/ru-RU/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span></span>

<span data-ttu-id="589a4-164">В приведенном ниже примере показано, как вызывать функцию `median` и один или несколько диапазонов входных значений с помощью REST API для Excel.</span><span class="sxs-lookup"><span data-stu-id="589a4-164">The example below shows how to call the `median` function and one or more input ranges with the Excel REST API.</span></span> 

<span data-ttu-id="589a4-165">Запрос:</span><span class="sxs-lookup"><span data-stu-id="589a4-165">Request:</span></span> 

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

<span data-ttu-id="589a4-166">Отклик:</span><span class="sxs-lookup"><span data-stu-id="589a4-166">Response:</span></span>

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
