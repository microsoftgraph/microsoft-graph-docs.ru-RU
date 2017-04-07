# <a name="uploadsession-resource-type"></a>Тип ресурса UploadSession

Ресурс **UploadSession** предоставляет сведения о том, как отправлять большие файлы в библиотеки документов OneDrive, OneDrive для бизнеса или SharePoint.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "uploadUrl", "nextExpectedRanges" ],
  "@odata.type": "microsoft.graph.uploadSession"
}-->

```json
{
  "expirationDateTime": "timestamp",
  "nextExpectedRanges": ["string"],
  "uploadUrl": "url"
}

```
## <a name="properties"></a>Свойства


| Свойство             | Тип              |Описание|
|:-------------------|:------------------|:----------|
| expirationDateTime | DateTimeOffset    | Дата и время (в формате UTC) истечения срока действия сеанса. Полный файл необходимо отправить до наступления этого момента. |
| nextExpectedRanges | Коллекция строк | Коллекция диапазонов байтов файла, отсутствующих на сервере. Эти диапазоны имеют нулевую индексацию и формат "начало-конец" (например, "0–26" для указания первых 27 байтов файла). |
| uploadUrl          | Строка            | URL-адрес конечной точки, принимающей запросы PUT для диапазонов байтов файла. |

## <a name="additional-resources"></a>Дополнительные ресурсы

Сведения о том, как отправлять файлы с помощью сеанса отправки, см. в статье [Отправка больших файлов с помощью сеанса отправки](../api/item_createUploadSession.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "uploadSession resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->