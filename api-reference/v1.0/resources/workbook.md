---
title: Тип ресурса workbook
description: Объект верхнего уровня, содержащий связанные объекты книг, такие как листы, таблицы и диапазоны.
ms.localizationpriority: high
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ded7bceefb0cebdfaf45b16a88de3f4f0a9d5244
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134208"
---
# <a name="workbook-resource-type"></a>Тип ресурса workbook

Пространство имен: microsoft.graph

Объект верхнего уровня, содержащий связанные объекты книг, такие как листы, таблицы и диапазоны.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Create session](../api/workbook-createsession.md) | [workbookSessionInfo](workbooksessioninfo.md) |Создание сеанса книги для запуска сохраняемого или несохраняемого сеанса.|
|[Close session](../api/workbook-closesession.md) | Нет |Закрытие существующего сеанса.|
|[Refresh session](../api/workbook-refreshsession.md) | Нет |Обновление существующего сеанса.|

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|names|Коллекция [workbookNamedItem](nameditem.md)|Представляет коллекцию именованных элементов в книгах (именованные диапазоны и константы). Только для чтения.|
|tables|Коллекция [workbookTable](table.md)|Представляет коллекцию таблиц, сопоставленных с книгой. Только для чтения.|
|worksheets|Коллекция [workbookWorksheet](worksheet.md)|Представляет коллекцию листов, сопоставленных с книгой. Только для чтения.|
|operations|Коллекция [workbookOperation](workbookoperation.md)|Состояние операций в книге. Получить коллекцию операций нельзя, но можно получить состояние длительной операции, если в ответе возвращается заголовок `Location`. Только для чтения.|

## <a name="functions"></a>Функции

[Функции Excel](#functions): вызов функции книги с использованием синтаксиса `POST /me/drive/root/workbook/functions/{function-name}` и предоставление аргументов функции в основном тексте с помощью объекта JSON. Результирующее `value` функции и любые строки `error` возвращаются в объекте результата функции. Если значение `error` равно `null`, это свидетельствует об успешном выполнении функции. 

Полный список поддерживаемых функций см. [здесь](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Имена определенных параметров и типы данных см. в сигнатуре функции.

_Важные примечания._ 
* Входной параметр range предоставляется с использованием объекта range вместо строки адреса range.  
* Параметр index индексируется с 1, а не с 0, как в большинстве API. 

Пример: **vlookup**.

В электронной таблице Excel функция `vlookup` принимает следующие аргументы:

1. Значение, которое вы хотите найти. Его также называют искомым значением.
2. Диапазон, в котором находится искомое значение. Помните, что искомое значение должно находиться всегда в первом столбце в диапазоне ВПР. В ином случае его обработка не будет выполняться правильно. Например, если искомое значение находится в ячейке C2, диапазон должен начинаться с C.
3. Номер столбца в диапазоне, содержащий возвращаемое значение. Например, если в качестве диапазона вы указываете B2:D11, следует считать B первым столбцом, C — вторым и т. д.
4. При желании вы можете указать TRUE, если нужно приблизительное совпадение, и FALSE, если нужно точное совпадение возвращаемого значения. Если вы ничего не укажете, значением по умолчанию будет TRUE (приблизительное совпадение).

В ячейке функция `vlookup` выглядит так: 

=ВПР(искомое значение, диапазон с искомым значением, номер столбца в диапазоне с возвращаемым значением, необязательное значение TRUE для указания приблизительного значения или FALSE для указания точного совпадения)

(См. документацию по [функции ВПР в Excel](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)

В приведенном ниже примере показано, как вызывать функцию `vlookup` и передавать эти параметры с помощью REST API для Excel.

Запрос: 

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

Отклик:

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

Пример: `median`.

В электронной таблице Excel функция `median` принимает массив одного или нескольких диапазонов входных значений.

В ячейке функция `median` выглядит так, как показано в этом примере:

=МЕДИАНА(A2:A6)

(См. документацию по [функции МЕДИАНА в Excel](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)

В приведенном ниже примере показано, как вызывать функцию `median` и один или несколько диапазонов входных значений с помощью REST API для Excel. 

Запрос: 

```http 
POST https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/median
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
   "values":[
      {
         "address":"Sheet2!A1:A5"
      },
      {
         "address":"Sheet2!B1:B5"
      }
   ]
}
```

Отклик:

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
## <a name="json-representation"></a>Представление JSON

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

