---
title: Тип ресурса workbook
description: Объект верхнего уровня, содержащий связанные объекты книг, такие как листы, таблицы и диапазоны.
localization_priority: Priority
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ec413303365d97a2683997939e20820ed9205f84
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577830"
---
# <a name="workbook-resource-type"></a><span data-ttu-id="4ffc8-103">Тип ресурса workbook</span><span class="sxs-lookup"><span data-stu-id="4ffc8-103">workbook resource type</span></span>

<span data-ttu-id="4ffc8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ffc8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4ffc8-105">Объект верхнего уровня, содержащий связанные объекты книг, такие как листы, таблицы и диапазоны.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-105">The top-level object that contains related workbook objects such as worksheets, tables, and ranges.</span></span>

## <a name="methods"></a><span data-ttu-id="4ffc8-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4ffc8-106">Methods</span></span>

| <span data-ttu-id="4ffc8-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4ffc8-107">Method</span></span>       | <span data-ttu-id="4ffc8-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4ffc8-108">Return Type</span></span>  |<span data-ttu-id="4ffc8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4ffc8-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4ffc8-110">Create session</span><span class="sxs-lookup"><span data-stu-id="4ffc8-110">Create session</span></span>](../api/workbook-createsession.md) | [<span data-ttu-id="4ffc8-111">workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="4ffc8-111">workbookSessionInfo</span></span>](workbooksessioninfo.md) |<span data-ttu-id="4ffc8-112">Создание сеанса книги для запуска сохраняемого или несохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-112">Create a workbook session to start a persistent or non-persistent session.</span></span>|
|[<span data-ttu-id="4ffc8-113">Close session</span><span class="sxs-lookup"><span data-stu-id="4ffc8-113">Close session</span></span>](../api/workbook-closesession.md) | <span data-ttu-id="4ffc8-114">Нет</span><span class="sxs-lookup"><span data-stu-id="4ffc8-114">None</span></span> |<span data-ttu-id="4ffc8-115">Закрытие существующего сеанса.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-115">Close an existing session.</span></span>|
|[<span data-ttu-id="4ffc8-116">Refresh session</span><span class="sxs-lookup"><span data-stu-id="4ffc8-116">Refresh session</span></span>](../api/workbook-refreshsession.md) | <span data-ttu-id="4ffc8-117">Нет</span><span class="sxs-lookup"><span data-stu-id="4ffc8-117">None</span></span> |<span data-ttu-id="4ffc8-118">Обновление существующего сеанса.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-118">Refresh an existing session.</span></span>|

## <a name="properties"></a><span data-ttu-id="4ffc8-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ffc8-119">Properties</span></span>
<span data-ttu-id="4ffc8-120">Нет</span><span class="sxs-lookup"><span data-stu-id="4ffc8-120">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="4ffc8-121">Связи</span><span class="sxs-lookup"><span data-stu-id="4ffc8-121">Relationships</span></span>
| <span data-ttu-id="4ffc8-122">Связь</span><span class="sxs-lookup"><span data-stu-id="4ffc8-122">Relationship</span></span> | <span data-ttu-id="4ffc8-123">Тип</span><span class="sxs-lookup"><span data-stu-id="4ffc8-123">Type</span></span>   |<span data-ttu-id="4ffc8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4ffc8-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ffc8-125">names</span><span class="sxs-lookup"><span data-stu-id="4ffc8-125">names</span></span>|<span data-ttu-id="4ffc8-126">Коллекция [workbookNamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="4ffc8-126">[workbookNamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="4ffc8-p101">Представляет коллекцию именованных элементов в книге (именованные диапазоны и константы). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-p101">Represents a collection of workbook scoped named items (named ranges and constants). Read-only.</span></span>|
|<span data-ttu-id="4ffc8-129">tables</span><span class="sxs-lookup"><span data-stu-id="4ffc8-129">tables</span></span>|<span data-ttu-id="4ffc8-130">Коллекция [workbookTable](table.md)</span><span class="sxs-lookup"><span data-stu-id="4ffc8-130">[workbookTable](table.md) collection</span></span>|<span data-ttu-id="4ffc8-p102">Представляет коллекцию таблиц, сопоставленных с книгой. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-p102">Represents a collection of tables associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="4ffc8-133">worksheets</span><span class="sxs-lookup"><span data-stu-id="4ffc8-133">worksheets</span></span>|<span data-ttu-id="4ffc8-134">Коллекция [workbookWorksheet](worksheet.md)</span><span class="sxs-lookup"><span data-stu-id="4ffc8-134">[workbookWorksheet](worksheet.md) collection</span></span>|<span data-ttu-id="4ffc8-135">Представляет коллекцию листов, сопоставленных с книгой.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-135">Represents a collection of worksheets associated with the workbook.</span></span> <span data-ttu-id="4ffc8-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-136">Read-only.</span></span>|
|<span data-ttu-id="4ffc8-137">operations</span><span class="sxs-lookup"><span data-stu-id="4ffc8-137">operations</span></span>|<span data-ttu-id="4ffc8-138">Коллекция [workbookOperation](workbookoperation.md)</span><span class="sxs-lookup"><span data-stu-id="4ffc8-138">[workbookOperation](workbookoperation.md) collection</span></span>|<span data-ttu-id="4ffc8-139">Состояние операций в книге.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-139">The status of workbook operations.</span></span> <span data-ttu-id="4ffc8-140">Получить коллекцию операций нельзя, но можно получить состояние длительной операции, если в ответе возвращается заголовок `Location`.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-140">Getting an operation collection is not supported, but you can get the status of a long-running operation if the `Location` header is returned in the response.</span></span> <span data-ttu-id="4ffc8-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-141">Read-only.</span></span>|

## <a name="functions"></a><span data-ttu-id="4ffc8-142">Функции</span><span class="sxs-lookup"><span data-stu-id="4ffc8-142">Functions</span></span>

<span data-ttu-id="4ffc8-p105">[Функции Excel](#functions): вызов функции книги с использованием синтаксиса `POST /me/drive/root/workbook/functions/{function-name}` и предоставление аргументов функции в основном тексте с помощью объекта JSON. Результирующее `value` функции и любые строки `error` возвращаются в объекте результата функции. Если значение `error` равно `null`, это свидетельствует об успешном выполнении функции.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-p105">[Excel functions](#functions): Invoke a workbook function using the syntax `POST /me/drive/root/workbook/functions/{function-name}` and providing the function argument(s) in the body using a JSON object. The function's resulting `value` and any `error` strings are returned in the function result object. The `error` value of `null` indicates successful execution of the function.</span></span> 

<span data-ttu-id="4ffc8-p106">Полный список поддерживаемых функций см. [здесь](https://support.office.com/ru-RU/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Имена определенных параметров и типы данных см. в сигнатуре функции.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-p106">The complete list of supported functions are listed [here](https://support.office.com/ru-RU/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="4ffc8-148">_Важные примечания._</span><span class="sxs-lookup"><span data-stu-id="4ffc8-148">_Important notes:_</span></span> 
* <span data-ttu-id="4ffc8-149">Входной параметр range предоставляется с использованием объекта range вместо строки адреса range.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-149">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="4ffc8-150">Параметр index индексируется с 1, а не с 0, как в большинстве API.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-150">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span> 

<span data-ttu-id="4ffc8-151">Пример: **vlookup**.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-151">Example: **vlookup**</span></span>

<span data-ttu-id="4ffc8-152">В электронной таблице Excel функция `vlookup` принимает следующие аргументы:</span><span class="sxs-lookup"><span data-stu-id="4ffc8-152">In an Excel spreadsheet, the `vlookup` function takes the following arguments:</span></span>

1. <span data-ttu-id="4ffc8-153">Значение, которое вы хотите найти. Его также называют искомым значением.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-153">The value you want to look up, also called the lookup value.</span></span>
2. <span data-ttu-id="4ffc8-154">Диапазон, в котором находится искомое значение.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-154">The range where the lookup value is located.</span></span> <span data-ttu-id="4ffc8-155">Помните, что искомое значение должно находиться всегда в первом столбце в диапазоне ВПР. В ином случае его обработка не будет выполняться правильно.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-155">Remember that the lookup value should always be in the first column in the range for VLOOKUP to work correctly.</span></span> <span data-ttu-id="4ffc8-156">Например, если искомое значение находится в ячейке C2, диапазон должен начинаться с C.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-156">For example, if your lookup value is in cell C2 then your range should start with C.</span></span>
3. <span data-ttu-id="4ffc8-157">Номер столбца в диапазоне, который содержит возвращаемое значение.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-157">The column number in the range that contains the return value.</span></span> <span data-ttu-id="4ffc8-158">Например, если вы укажете в качестве диапазона B2:D11, B будет первым столбцом, C — вторым и т. д.
</span><span class="sxs-lookup"><span data-stu-id="4ffc8-158">For example, if you specify B2: D11 as the range, you should count B as the first column, C as the second, and so on.</span></span>
4. <span data-ttu-id="4ffc8-159">При желании вы можете указать TRUE, если нужно приблизительное совпадение, и FALSE, если нужно точное совпадение возвращаемого значения.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-159">Optionally, you can specify TRUE if you want an approximate match or FALSE if you want an exact match of the return value.</span></span> <span data-ttu-id="4ffc8-160">Если вы ничего не укажете, значением по умолчанию будет TRUE (приблизительное совпадение).</span><span class="sxs-lookup"><span data-stu-id="4ffc8-160">If you don't specify anything, the default value will always be TRUE or approximate match.</span></span>

<span data-ttu-id="4ffc8-161">В ячейке функция `vlookup` выглядит так:</span><span class="sxs-lookup"><span data-stu-id="4ffc8-161">Inside a cell, the `vlookup` function looks like this:</span></span> 

<span data-ttu-id="4ffc8-162">=ВПР(искомое значение, диапазон с искомым значением, номер столбца в диапазоне с возвращаемым значением, необязательное значение TRUE для указания приблизительного значения или FALSE для указания точного совпадения)</span><span class="sxs-lookup"><span data-stu-id="4ffc8-162">=VLOOKUP(lookup value, range containing the lookup value, the column number in the range containing the return value, optionally specify TRUE for approximate match or FALSE for an exact match)</span></span>

<span data-ttu-id="4ffc8-163">(См. документацию по [функции ВПР в Excel](https://support.office.com/ru-RU/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span><span class="sxs-lookup"><span data-stu-id="4ffc8-163">(See the documentation for the [VLOOKUP Excel function](https://support.office.com/ru-RU/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span></span>

<span data-ttu-id="4ffc8-164">В приведенном ниже примере показано, как вызывать функцию `vlookup` и передавать эти параметры с помощью REST API для Excel.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-164">The example below shows how to call the `vlookup` function and pass these parameters with the Excel REST API.</span></span>

<span data-ttu-id="4ffc8-165">Запрос:</span><span class="sxs-lookup"><span data-stu-id="4ffc8-165">Request:</span></span> 

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

<span data-ttu-id="4ffc8-166">Отклик:</span><span class="sxs-lookup"><span data-stu-id="4ffc8-166">Response:</span></span>

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

<span data-ttu-id="4ffc8-167">Пример: `median`.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-167">Example: `median`</span></span>

<span data-ttu-id="4ffc8-168">В электронной таблице Excel функция `median` принимает массив одного или нескольких диапазонов входных значений.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-168">In an Excel spreadsheet, the `median` function takes an array of one or more input ranges.</span></span>

<span data-ttu-id="4ffc8-169">В ячейке функция `median` выглядит так, как показано в этом примере:</span><span class="sxs-lookup"><span data-stu-id="4ffc8-169">Inside a cell, the `median` function looks like this example:</span></span>

<span data-ttu-id="4ffc8-170">=МЕДИАНА(A2:A6)</span><span class="sxs-lookup"><span data-stu-id="4ffc8-170">=MEDIAN(A2:A6)</span></span>

<span data-ttu-id="4ffc8-171">(См. документацию по [функции МЕДИАНА в Excel](https://support.office.com/ru-RU/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span><span class="sxs-lookup"><span data-stu-id="4ffc8-171">(See the documentation for the [MEDIAN Excel function](https://support.office.com/ru-RU/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span></span>

<span data-ttu-id="4ffc8-172">В приведенном ниже примере показано, как вызывать функцию `median` и один или несколько диапазонов входных значений с помощью REST API для Excel.</span><span class="sxs-lookup"><span data-stu-id="4ffc8-172">The example below shows how to call the `median` function and one or more input ranges with the Excel REST API.</span></span> 

<span data-ttu-id="4ffc8-173">Запрос:</span><span class="sxs-lookup"><span data-stu-id="4ffc8-173">Request:</span></span> 

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

<span data-ttu-id="4ffc8-174">Отклик:</span><span class="sxs-lookup"><span data-stu-id="4ffc8-174">Response:</span></span>

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
## <a name="json-representation"></a><span data-ttu-id="4ffc8-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ffc8-175">JSON representation</span></span>

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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Workbook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

