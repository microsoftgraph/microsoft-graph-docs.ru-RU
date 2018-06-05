# <a name="use-workbook-functions-in-excel-with-microsoft-graph"></a><span data-ttu-id="c8b50-101">Использование функций книг в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c8b50-101">Use workbook functions in Excel with Microsoft Graph</span></span>

<span data-ttu-id="c8b50-102">Вы можете вызвать любую функцию книги, используя следующий синтаксис: `POST /workbook/functions/{function-name}`.</span><span class="sxs-lookup"><span data-stu-id="c8b50-102">You can invoke any workbook function by using the following syntax: `POST /workbook/functions/{function-name}`.</span></span> <span data-ttu-id="c8b50-103">Укажите аргументы функции в теле запроса с помощью объекта JSON.</span><span class="sxs-lookup"><span data-stu-id="c8b50-103">You provide the function argument(s) in the body using a JSON object.</span></span> <span data-ttu-id="c8b50-104">Система возвращает `value`, полученное в результате выполнения функции, и все строки `error` в объекте результата выполнения функции.</span><span class="sxs-lookup"><span data-stu-id="c8b50-104">The function's resulting `value` and any `error` strings are returned in the function result object.</span></span> <span data-ttu-id="c8b50-105">Если значение `error` равно `null`, это свидетельствует об успешном выполнении функции.</span><span class="sxs-lookup"><span data-stu-id="c8b50-105">The `error` value of `null` indicates successful execution of the function.</span></span>

<span data-ttu-id="c8b50-106">Полный список поддерживаемых функций см. [здесь](https://support.office.com/ru-RU/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188).</span><span class="sxs-lookup"><span data-stu-id="c8b50-106">The complete list of supported functions are listed [here](https://support.office.com/ru-RU/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188).</span></span> <span data-ttu-id="c8b50-107">Имена определенных параметров и типы данных см. в сигнатуре функции.</span><span class="sxs-lookup"><span data-stu-id="c8b50-107">Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="c8b50-108">_Важные примечания._</span><span class="sxs-lookup"><span data-stu-id="c8b50-108">_Important notes:_</span></span>
* <span data-ttu-id="c8b50-109">Входной параметр range предоставляется с использованием объекта range вместо строки адреса range.</span><span class="sxs-lookup"><span data-stu-id="c8b50-109">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="c8b50-110">Параметр index индексируется с 1, а не с 0, как в большинстве API.</span><span class="sxs-lookup"><span data-stu-id="c8b50-110">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span>

<span data-ttu-id="c8b50-111">Пример: **vlookup**.</span><span class="sxs-lookup"><span data-stu-id="c8b50-111">Example: **vlookup**</span></span>

<span data-ttu-id="c8b50-112">В электронной таблице Excel функция `vlookup` принимает следующие аргументы:</span><span class="sxs-lookup"><span data-stu-id="c8b50-112">In an Excel spreadsheet, the `vlookup` function takes the following arguments:</span></span>

1. <span data-ttu-id="c8b50-113">**lookup_value** (обязательный аргумент). Искомое значение.</span><span class="sxs-lookup"><span data-stu-id="c8b50-113">**lookup_value** (required) The value you want to look up.</span></span>
2. <span data-ttu-id="c8b50-114">**table_array** (обязательный аргумент). Диапазон ячеек, в котором находится искомое значение.</span><span class="sxs-lookup"><span data-stu-id="c8b50-114">**table_array** (required) The range of cells where the lookup value is located.</span></span> <span data-ttu-id="c8b50-115">Чтобы функция ВПР работала правильно, искомое значение всегда должно находиться в первом столбце диапазона.</span><span class="sxs-lookup"><span data-stu-id="c8b50-115">Remember that the lookup value should always be in the first column in the range for VLOOKUP to work correctly.</span></span> <span data-ttu-id="c8b50-116">Например, если искомое значение находится в ячейке C2, диапазон должен начинаться со столбца C.</span><span class="sxs-lookup"><span data-stu-id="c8b50-116">For example, if your lookup value is in cell C2 then your range should start with C.</span></span>
3. <span data-ttu-id="c8b50-117">**col_index_num** (обязательный аргумент). Номер столбца в диапазоне, содержащем возвращаемое значение.</span><span class="sxs-lookup"><span data-stu-id="c8b50-117">The column number in the range that contains the return value.</span></span> <span data-ttu-id="c8b50-118">Например, если вы укажете в качестве диапазона B2:D11, B будет первым столбцом, C — вторым и т. д.
</span><span class="sxs-lookup"><span data-stu-id="c8b50-118">For example, if you specify B2: D11 as the range, you should count B as the first column, C as the second, and so on.</span></span>
4. <span data-ttu-id="c8b50-119">**range_lookup** (необязательный аргумент). Логическое значение, указывающее режим работы функции **ВПР**: поиск приблизительного или точного совпадения.</span><span class="sxs-lookup"><span data-stu-id="c8b50-119">**range_lookup** (optional) The logical value that specifies whether you want **VLOOKUP** to find an approximate or an exact match.</span></span> <span data-ttu-id="c8b50-120">Если необходимо, чтобы функция работала в режиме поиска приблизительного совпадения, укажите значение **TRUE**. Если необходимо, чтобы функция возвращала точные совладения, укажите значение **FALSE**.</span><span class="sxs-lookup"><span data-stu-id="c8b50-120">Optionally, you can specify TRUE if you want an approximate match or FALSE if you want an exact match of the return value.</span></span> <span data-ttu-id="c8b50-121">Если вы не укажете значение, по умолчанию будет использовано значение TRUE, и функция будет возвращать приблизительные совпадения.</span><span class="sxs-lookup"><span data-stu-id="c8b50-121">If you don't specify anything, the default value will always be TRUE or approximate match.</span></span>

<span data-ttu-id="c8b50-122">В ячейке функция `vlookup` выглядит так:</span><span class="sxs-lookup"><span data-stu-id="c8b50-122">Inside a cell, the `vlookup` function looks like this:</span></span>

<span data-ttu-id="c8b50-123">=ВПР(искомое значение, диапазон с искомым значением, номер столбца в диапазоне с возвращаемым значением, необязательное значение TRUE для указания приблизительного значения или FALSE для указания точного совпадения)</span><span class="sxs-lookup"><span data-stu-id="c8b50-123">=VLOOKUP(lookup value, range containing the lookup value, the column number in the range containing the return value, optionally specify TRUE for approximate match or FALSE for an exact match)</span></span>

<span data-ttu-id="c8b50-124">(См. документацию по функции [ВПР в Excel](https://support.office.com/ru-RU/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span><span class="sxs-lookup"><span data-stu-id="c8b50-124">(See the documentation for the [VLOOKUP Excel function](https://support.office.com/ru-RU/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span></span>


##### <a name="request"></a><span data-ttu-id="c8b50-125">Запрос:</span><span class="sxs-lookup"><span data-stu-id="c8b50-125">Request:</span></span>
<span data-ttu-id="c8b50-126">В примере ниже показано, как вызвать функцию `vlookup` и передать в нее эти параметры с помощью REST API для Excel.</span><span class="sxs-lookup"><span data-stu-id="c8b50-126">The example below shows how to call the `vlookup` function and pass these parameters with the Excel REST API.</span></span>

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

##### <a name="response"></a><span data-ttu-id="c8b50-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8b50-127">Response</span></span>

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

<span data-ttu-id="c8b50-128">Пример: `median`</span><span class="sxs-lookup"><span data-stu-id="c8b50-128">Example: `median`</span></span>

<span data-ttu-id="c8b50-129">В электронной таблице Excel функция `median` принимает массив одного или нескольких диапазонов входных значений.</span><span class="sxs-lookup"><span data-stu-id="c8b50-129">In an Excel spreadsheet, the `median` function takes an array of one or more input ranges.</span></span>

<span data-ttu-id="c8b50-130">В ячейке функция `median` выглядит так, как показано в этом примере:</span><span class="sxs-lookup"><span data-stu-id="c8b50-130">Inside a cell, the `median` function looks like this example:</span></span>

<span data-ttu-id="c8b50-131">=МЕДИАНА(A2:A6)</span><span class="sxs-lookup"><span data-stu-id="c8b50-131">=MEDIAN(A2:A6)</span></span>

<span data-ttu-id="c8b50-132">(См. документацию по [функции МЕДИАНА в Excel](https://support.office.com/ru-RU/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span><span class="sxs-lookup"><span data-stu-id="c8b50-132">(See the documentation for the [MEDIAN Excel function](https://support.office.com/ru-RU/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span></span>

##### <a name="request"></a><span data-ttu-id="c8b50-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8b50-133">Request</span></span>
<span data-ttu-id="c8b50-134">В примере ниже показано, как вызывать функцию `median` и один или несколько диапазонов входных значений с помощью REST API для Excel.</span><span class="sxs-lookup"><span data-stu-id="c8b50-134">The example below shows how to call the `median` function and one or more input ranges with the Excel REST API.</span></span>

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

##### <a name="response"></a><span data-ttu-id="c8b50-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8b50-135">Response</span></span>

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

## <a name="see-also"></a><span data-ttu-id="c8b50-136">См. также</span><span class="sxs-lookup"><span data-stu-id="c8b50-136">See also</span></span>
* [<span data-ttu-id="c8b50-137">Управление сеансами в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c8b50-137">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="c8b50-138">Запись в книгу Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c8b50-138">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="c8b50-139">Обновление формата диапазона в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c8b50-139">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="c8b50-140">Показ изображения диаграммы в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c8b50-140">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="c8b50-141">Использование REST API для Excel</span><span class="sxs-lookup"><span data-stu-id="c8b50-141">Use the Excel REST API</span></span>](../api-reference/v1.0/resources/excel.md)
