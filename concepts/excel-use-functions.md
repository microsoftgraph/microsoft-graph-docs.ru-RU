---
title: Использование функций книг в Excel с помощью Microsoft Graph
description: 'Вы можете вызвать любую функцию книги, используя следующий синтаксис: `POST /me/drive/root/workbook/functions/{function-name}`. Укажите аргументы функции в теле запроса с помощью объекта JSON. Система возвращает `value`, полученное в результате выполнения функции, и все строки `error` в объекте результата выполнения функции. Если значение `error` равно `null`, это свидетельствует об успешном выполнении функции.'
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 39b93c633951ffe8997a66132a830673459776963d5d537c61aa67fb29a41fe0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205165"
---
# <a name="use-workbook-functions-in-excel-with-microsoft-graph"></a>Использование функций книг в Excel с помощью Microsoft Graph

Вы можете вызвать любую функцию книги, используя следующий синтаксис: `POST /me/drive/root/workbook/functions/{function-name}`. Укажите аргументы функции в теле запроса с помощью объекта JSON. Система возвращает `value`, полученное в результате выполнения функции, и все строки `error` в объекте результата выполнения функции. Если значение `error` равно `null`, это свидетельствует об успешном выполнении функции.

Полный список поддерживаемых функций см. в [Excel. Класс "Функции".](/javascript/api/excel/excel.functions?view=excel-js-preview) Имена определенных параметров и типы данных см. в сигнатуре функции.

_Важные примечания._
* Входной параметр range предоставляется с использованием объекта range вместо строки адреса range.  
* Параметр index индексируется с 1, а не с 0, как в большинстве API.

Пример: **vlookup**.

В электронной таблице Excel функция `vlookup` принимает следующие аргументы:

1. **lookup_value** (обязательный аргумент). Искомое значение.
2. **table_array** (обязательный аргумент). Диапазон ячеек, в котором находится искомое значение. Помните, что искомое значение должно находиться всегда в первом столбце в диапазоне ВПР. В ином случае его обработка не будет выполняться правильно. Например, если искомое значение находится в ячейке C2, диапазон должен начинаться с C.
3. **col_index_num** (обязательный аргумент). Номер столбца в диапазоне, содержащем возвращаемое значение. Например, если вы укажете в качестве диапазона B2:D11, B будет первым столбцом, C — вторым и т. д.

4. **range_lookup** (необязательный аргумент). Логическое значение, указывающее режим работы функции **ВПР**: поиск приблизительного или точного совпадения. Если необходимо, чтобы функция работала в режиме поиска приблизительного совпадения, укажите значение **TRUE**. Если необходимо, чтобы функция возвращала точные совладения, укажите значение **FALSE**. Если вы ничего не укажете, значением по умолчанию будет TRUE (приблизительное совпадение).

В ячейке функция `vlookup` выглядит так:

=ВПР(искомое значение, диапазон с искомым значением, номер столбца в диапазоне с возвращаемым значением, необязательное значение TRUE для указания приблизительного значения или FALSE для указания точного совпадения)

(См. документацию по [функции ВПР в Excel](https://support.office.com/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)


##### <a name="request"></a>Запрос:
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

##### <a name="response"></a>Ответ

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

(См. документацию по [функции МЕДИАНА в Excel](https://support.office.com/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)

##### <a name="request"></a>Запрос
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

##### <a name="response"></a>Отклик

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
* [Использование REST API для Excel](/graph/api/resources/excel?view=graph-rest-1.0)
