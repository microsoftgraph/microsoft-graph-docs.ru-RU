# <a name="workbook-resource-type"></a>Тип ресурса workbook

Workbook — это объект верхнего уровня, содержащий связанные объекты книг, например листы, таблицы, диапазоны и т. д.

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
| Связь | Тип    |Описание|
|:---------------|:--------|:----------|
|names|Коллекция объектов [NamedItem](nameditem.md)|Представляет коллекцию именованных элементов в книге (именованные диапазоны и константы). Только для чтения.|
|tables|Коллекция объектов [Table](table.md)|Представляет коллекцию таблиц, сопоставленных с книгой. Только для чтения.|
|worksheets|Коллекция объектов [Worksheet](worksheet.md)|Представляет коллекцию листов, сопоставленных с книгой. Только для чтения.|

## <a name="functions"></a>Функции

[Функции Excel](#functions): вызов функции книги с использованием синтаксиса `POST /workbook/functions/{function-name}` и предоставление аргументов функции в основном тексте с помощью объекта JSON. Результирующее `value` функции и любые строки `error` возвращаются в объекте результата функции. Если значение `error` равно `null`, это свидетельствует об успешном выполнении функции. 

Полный список поддерживаемых функций см. [здесь](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Имена определенных параметров и типы данных см. в сигнатуре функции.

_Важные примечания._ 
* Входной параметр range предоставляется с использованием объекта range вместо строки адреса range.  
* Параметр index индексируется с 1, а не с 0, как в большинстве API. 

Пример. 

В примере ниже при вызове функции `vlookup` в нее передаются значение подстановки, входной диапазон и значение, которое необходимо возвратить. 

Запрос: 

```http 
POST https://graph.microsoft.com/v1.0/me/drive/root:/book1.xlsx:/workbook/functions/vlookup
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
HTTP code: 200, OK
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/vlookup()",
    "error": null,
    "value": "28.3"
}
```

Пример. 

В примере ниже при вызове функции `median` в нее передается массив входных диапазонов. 

Запрос: 

```http 
POST https://graph.microsoft.com/v1.0/me/drive/root:/book1.xlsx:/workbook/functions/median
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
HTTP code: 200, OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookFunctionResult",
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
