---
title: Использование функций книги в Excel
description: Функции книги в Excel с Microsoft Graph можно использовать для вызова любой функции книги. Содержит примеры для функций випрука и медиана.
ms.localizationpriority: medium
author: lumine2008
ms.prod: excel
ms.openlocfilehash: eec1834a63ab87304b33eea1f75629fe12e56aec
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443370"
---
# <a name="use-workbook-functions-in-excel"></a>Использование функций книги в Excel

Функции книги в Excel с Microsoft Graph можно использовать для вызова любой функции книги с помощью следующего синтаксиса: `POST /me/drive/root/workbook/functions/{function-name}` Аргументы функции в теле можно указать с помощью объекта JSON. Результирующее `value` функции и любые строки `error` возвращаются в объекте результата функции. Если значение `error` равно `null`, это свидетельствует об успешном выполнении функции.

Полный список поддерживаемых функций см. в [описании класса Excel.Functions](/javascript/api/excel/excel.functions?view=excel-js-preview&preserve-view=true). Имена определенных параметров и типы данных см. в сигнатуре функции.

> [!IMPORTANT]
> - Входной параметр range предоставляется с использованием объекта range вместо строки адреса range.  
> - Параметр index индексируется с 1, а не с 0, как в большинстве API.

## <a name="example-vlookup"></a>Пример: `vlookup`

В электронной таблице Excel функция `vlookup` принимает следующие аргументы:

- **lookup_value** (обязательно): значение, которое требуется найти.

- **table_array** (обязательно): диапазон ячеек, в которых находится значение подстановки. Помните, что значение подстановки всегда должно находиться в первом столбце диапазона, чтобы функция **ВПР** правильно работает. Например, если значение подстановки находится в ячейке C2, диапазон должен начинаться с C.

- **col_index_num** (обязательно): номер столбца в диапазоне, содержащего возвращаемое значение. Например, если вы укажете в качестве диапазона B2:D11, B будет первым столбцом, C — вторым и т. д.


- **range_lookup** (необязательно): логическое значение, указывающее, требуется ли ВПР  найти приблизительное или точное совпадение. Если необходимо, чтобы функция работала в режиме поиска приблизительного совпадения, укажите значение **TRUE**. Если необходимо, чтобы функция возвращала точные совладения, укажите значение **FALSE**. Если ничего не указать, значение по умолчанию всегда будет равно TRUE или приблизительному совпадению.

В ячейке функция `vlookup` выглядит так:

`=VLOOKUP`(значение подстановки, диапазон, содержащий значение подстановки, номер столбца в диапазоне, содержащего возвращаемое значение, при необходимости укажите TRUE для приблизительного совпадения или FALSE для точного совпадения)

Дополнительные сведения см. в документации по функции [Excel ВПР](https://support.office.com/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).

### <a name="request"></a>Запрос

В примере ниже показано, как вызвать функцию `vlookup` и передать в нее эти параметры с помощью REST API для Excel.

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

### <a name="response"></a>Ответ

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

## <a name="example-median"></a>Пример: `median`.

В электронной таблице Excel функция `median` принимает массив одного или нескольких диапазонов входных значений.

В ячейке функция `median` выглядит так, как показано в этом примере:

`=MEDIAN(A2:A6)`

Дополнительные сведения см. в документации по функции [MediaN Excel](https://support.office.com/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).

### <a name="request"></a>Запрос

В примере ниже показано, как вызывать функцию `median` и один или несколько диапазонов входных значений с помощью REST API для Excel.

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

### <a name="response"></a>Отклик

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

## <a name="see-also"></a>См. также

* [Управление сеансами в Excel с помощью Microsoft Graph](excel-manage-sessions.md)
* [Запись в книгу Excel с помощью Microsoft Graph](excel-write-to-workbook.md)
* [Обновление формата диапазона в Excel с помощью Microsoft Graph](excel-update-range-format.md)
* [Показ изображения диаграммы в Excel с помощью Microsoft Graph](excel-display-chart-image.md)
* [Использование REST API для Excel](/graph/api/resources/excel)
