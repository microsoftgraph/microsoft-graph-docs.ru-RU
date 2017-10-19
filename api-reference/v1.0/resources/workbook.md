# <a name="workbook-resource-type"></a><span data-ttu-id="fc782-101">Тип ресурса workbook</span><span class="sxs-lookup"><span data-stu-id="fc782-101">Workbook resource type</span></span>

<span data-ttu-id="fc782-102">Workbook — это объект верхнего уровня, содержащий связанные объекты книг, например листы, таблицы, диапазоны и т. д.</span><span class="sxs-lookup"><span data-stu-id="fc782-102">Workbook is the top level object which contains related workbook objects such as worksheets, tables, ranges, etc.</span></span>

## <a name="properties"></a><span data-ttu-id="fc782-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc782-103">Properties</span></span>
<span data-ttu-id="fc782-104">Нет</span><span class="sxs-lookup"><span data-stu-id="fc782-104">None</span></span>

## <a name="methods"></a><span data-ttu-id="fc782-105">Методы</span><span class="sxs-lookup"><span data-stu-id="fc782-105">Methods</span></span>

| <span data-ttu-id="fc782-106">Метод</span><span class="sxs-lookup"><span data-stu-id="fc782-106">Method</span></span>       | <span data-ttu-id="fc782-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fc782-107">Return Type</span></span>  |<span data-ttu-id="fc782-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fc782-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fc782-109">Create Session</span><span class="sxs-lookup"><span data-stu-id="fc782-109">Create Upload Session</span></span>](../api/workbook_createsession.md) | [<span data-ttu-id="fc782-110">workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="fc782-110">workbookSessionInfo</span></span>](workbooksessioninfo.md) |<span data-ttu-id="fc782-111">Создание сеанса книги для запуска сохраняемого или несохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="fc782-111">Create a workbook session to start a persistent or non-persistent session.</span></span>|
|[<span data-ttu-id="fc782-112">Close Session</span><span class="sxs-lookup"><span data-stu-id="fc782-112">Close Session</span></span>](../api/workbook_closesession.md) | <span data-ttu-id="fc782-113">Нет</span><span class="sxs-lookup"><span data-stu-id="fc782-113">None</span></span> |<span data-ttu-id="fc782-114">Закрытие существующего сеанса.</span><span class="sxs-lookup"><span data-stu-id="fc782-114">Close an existing session.</span></span>|
|[<span data-ttu-id="fc782-115">Refresh Session</span><span class="sxs-lookup"><span data-stu-id="fc782-115">Refresh Session</span></span>](../api/workbook_refreshsession.md) | <span data-ttu-id="fc782-116">Нет</span><span class="sxs-lookup"><span data-stu-id="fc782-116">None</span></span> |<span data-ttu-id="fc782-117">Обновление существующего сеанса.</span><span class="sxs-lookup"><span data-stu-id="fc782-117">Refresh an existing session.</span></span>|


## <a name="relationships"></a><span data-ttu-id="fc782-118">Связи</span><span class="sxs-lookup"><span data-stu-id="fc782-118">Relationships</span></span>
| <span data-ttu-id="fc782-119">Связь</span><span class="sxs-lookup"><span data-stu-id="fc782-119">Relationship</span></span> | <span data-ttu-id="fc782-120">Тип</span><span class="sxs-lookup"><span data-stu-id="fc782-120">Type</span></span>   |<span data-ttu-id="fc782-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fc782-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc782-122">names</span><span class="sxs-lookup"><span data-stu-id="fc782-122">names</span></span>|<span data-ttu-id="fc782-123">Коллекция объектов [NamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="fc782-123">[NamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="fc782-p101">Представляет коллекцию именованных элементов в книге (именованные диапазоны и константы). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc782-p101">Represents a collection of workbook scoped named items (named ranges and constants). Read-only.</span></span>|
|<span data-ttu-id="fc782-126">tables</span><span class="sxs-lookup"><span data-stu-id="fc782-126">tables</span></span>|<span data-ttu-id="fc782-127">Коллекция объектов [Table](table.md)</span><span class="sxs-lookup"><span data-stu-id="fc782-127">[Table](table.md) collection</span></span>|<span data-ttu-id="fc782-p102">Представляет коллекцию таблиц, сопоставленных с книгой. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc782-p102">Represents a collection of tables associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="fc782-130">worksheets</span><span class="sxs-lookup"><span data-stu-id="fc782-130">worksheets</span></span>|<span data-ttu-id="fc782-131">Коллекция объектов [Worksheet](worksheet.md)</span><span class="sxs-lookup"><span data-stu-id="fc782-131">[Worksheet](worksheet.md) collection</span></span>|<span data-ttu-id="fc782-p103">Представляет коллекцию листов, сопоставленных с книгой. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc782-p103">Represents a collection of worksheets associated with the workbook. Read-only.</span></span>|

## <a name="functions"></a><span data-ttu-id="fc782-134">Функции</span><span class="sxs-lookup"><span data-stu-id="fc782-134">Functions</span></span>

<span data-ttu-id="fc782-135">[Функции Excel](#functions): Вызов функции книги с использованием синтаксиса `POST /workbook/functions/{function-name}` и предоставление аргументов функции в теле с помощью объекта JSON.</span><span class="sxs-lookup"><span data-stu-id="fc782-135">[Excel functions](#functions): Invoke a workbook function using the syntax `POST /workbook/functions/{function-name}` and providing the function argument(s) in the body using a JSON object. The function's resulting  and any  strings are returned in the function result object. The  value of  indicates successful execution of the function.</span></span> <span data-ttu-id="fc782-136">Результирующее `value` функции и все строки `error` возвращаются в объекте результата функции.</span><span class="sxs-lookup"><span data-stu-id="fc782-136">The function's resulting `value` and any `error` strings are returned in the function result object.</span></span> <span data-ttu-id="fc782-137">Если значение `error` равно `null`, это свидетельствует об успешном выполнении функции.</span><span class="sxs-lookup"><span data-stu-id="fc782-137">The `error` value of `null` indicates successful execution of the function.</span></span> 

<span data-ttu-id="fc782-138">Полный список поддерживаемых функций см. [здесь](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188).</span><span class="sxs-lookup"><span data-stu-id="fc782-138">The complete list of supported functions are listed here. Refer to the function signature for specific parameter names and data types.</span></span> <span data-ttu-id="fc782-139">Имена определенных параметров и типы данных см. в сигнатуре функции.</span><span class="sxs-lookup"><span data-stu-id="fc782-139">The complete list of supported functions are listed here. Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="fc782-140">_Важные примечания._</span><span class="sxs-lookup"><span data-stu-id="fc782-140">_Important notes:_</span></span> 
* <span data-ttu-id="fc782-141">Входной параметр range предоставляется с использованием объекта range вместо строки адреса range.</span><span class="sxs-lookup"><span data-stu-id="fc782-141">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="fc782-142">Параметр index индексируется с 1, а не с 0, как в большинстве API.</span><span class="sxs-lookup"><span data-stu-id="fc782-142">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span> 

<span data-ttu-id="fc782-143">Пример.</span><span class="sxs-lookup"><span data-stu-id="fc782-143">Example:</span></span> 

<span data-ttu-id="fc782-144">В примере ниже при вызове функции `vlookup` в нее передаются значение подстановки, входной диапазон и значение, которое необходимо возвратить.</span><span class="sxs-lookup"><span data-stu-id="fc782-144">In the below example, `vlookup` function is called by passing lookup value, input range and the value to be returned.</span></span> 

<span data-ttu-id="fc782-145">Запрос:</span><span class="sxs-lookup"><span data-stu-id="fc782-145">Request:</span></span> 

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

<span data-ttu-id="fc782-146">Отклик:</span><span class="sxs-lookup"><span data-stu-id="fc782-146">Response:</span></span>

```http
HTTP code: 200, OK
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/vlookup()",
    "error": null,
    "value": "28.3"
}
```

<span data-ttu-id="fc782-147">Пример.</span><span class="sxs-lookup"><span data-stu-id="fc782-147">Example:</span></span> 

<span data-ttu-id="fc782-148">В примере ниже при вызове функции `median` в нее передается массив входных диапазонов.</span><span class="sxs-lookup"><span data-stu-id="fc782-148">In the below example, `median` function is called by passing the input range(s) in an array.</span></span> 

<span data-ttu-id="fc782-149">Запрос:</span><span class="sxs-lookup"><span data-stu-id="fc782-149">Request:</span></span> 

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

<span data-ttu-id="fc782-150">Отклик:</span><span class="sxs-lookup"><span data-stu-id="fc782-150">Response:</span></span>

```http
HTTP code: 200, OK
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
