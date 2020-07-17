---
title: Тип ресурса "книга"
description: Содержит связанные объекты книг, такие как листы, таблицы, диапазоны и т. д.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 34523b5ff0e358344b8c3c5b695e89a9bdddd7a2
ms.sourcegitcommit: b469176f49aacbd02cd06838cc7c8d36cf5bc768
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2020
ms.locfileid: "45165109"
---
# <a name="workbook-resource-type"></a>Тип ресурса "книга"

Пространство имен: microsoft.graph

Содержит связанные объекты книг, такие как листы, таблицы, диапазоны и т. д.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание сеанса](../api/workbook-createsession.md) | [workbookSessionInfo](workbooksessioninfo.md) |Создание сеанса книги для запуска сохраняемого или несохраняемого сеанса.|
|[Закрыть сеанс](../api/workbook-closesession.md) | Нет |Закрытие существующего сеанса.|
|[Сеанс обновления](../api/workbook-refreshsession.md) | Нет |Обновление существующего сеанса.|

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|names|Коллекция [воркбукнамедитем](workbooknameditem.md) |Представляет коллекцию именованных элементов в книге (именованные диапазоны и константы). Только для чтения.|
|tables|Коллекция [воркбуктабле](workbooktable.md) |Представляет коллекцию таблиц, сопоставленных с книгой. Только для чтения.|
|worksheets|Коллекция [воркбукворкшит](workbookworksheet.md) |Представляет коллекцию листов, сопоставленных с книгой. Только для чтения.|
|воркббукаппликатион|[воркбукаппликатион](workbookapplication.md) |Представляет Воркбукаппликатион Excel, который управляет книгой.|
|operations|Коллекция [воркбукоператион](workbookoperation.md)|Состояние операций книги. Получение коллекции операций не поддерживается, но вы можете получить состояние длительной операции, если `Location` заголовок возвращается в ответе. Только для чтения. Допускается значение null.|

## <a name="functions"></a>Функции

[Функции Excel](#functions): вызов функции книги с использованием синтаксиса `POST /workbook/functions/{function-name}` и предоставление аргументов функции в основном тексте с помощью объекта JSON. Результирующее `value` функции и любые строки `error` возвращаются в объекте результата функции. Если значение `error` равно `null`, это свидетельствует об успешном выполнении функции. 

Полный список поддерживаемых функций см. [здесь](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Имена определенных параметров и типы данных см. в сигнатуре функции.

_Важные примечания._ 
* Входной параметр range предоставляется с использованием объекта range вместо строки адреса range.  
* Параметр index индексируется с 1, а не с 0, как в большинстве API. 

Пример: **vlookup**.

В электронной таблице Excel функция `vlookup` принимает следующие аргументы:

1. Значение, которое вы хотите найти. Его также называют искомым значением.
2. Диапазон, в котором находится искомое значение. Помните, что искомое значение должно находиться всегда в первом столбце в диапазоне ВПР. В ином случае его обработка не будет выполняться правильно. Например, если искомое значение находится в ячейке C2, диапазон должен начинаться с C.
3. Номер столбца в диапазоне, который содержит возвращаемое значение. Например, если вы укажете в качестве диапазона B2:D11, B будет первым столбцом, C — вторым и т. д.

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
"values" :  [
        { "address": "Sheet2!A1:A5" },
        { "address": "Sheet2!B1:B5" },
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
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.workbook"
}-->
``` json
{
    "id": "string"
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
