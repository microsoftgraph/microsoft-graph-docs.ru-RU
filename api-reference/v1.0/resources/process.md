# <a name="process-resource-type"></a>Тип ресурса process

Содержит информацию о состоянии процесса, связанного с оповещением.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|accountName|String|Идентификатор учетной записи пользователя (контекст учетной записи пользователя, под которой запущен процесс), например, AccountName, ИД безопасности и т. п.|
|commandLine|String|Полная командная строка вызова процесса, включающая все параметры.|
|createdDateTime|DateTimeOffset|Время запуска процесса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|fileHash|[fileHash](filehash.md)|Сложный тип, содержащий хэш-значение файла (криптографическое и чувствительное к расположению).|
|integrityLevel|processIntegrityLevel|Уровень целостности данных процесса. Возможные значения: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.|
|isElevated|Boolean|Значение true, если процесс с повышенными правами.|
|name|String|Имя файла образа процесса.|
|parentProcessCreatedDateTime|DateTimeOffset|Дата и время запуска родительского процесса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|parentProcessId|Int32|Идентификатор (PID) родительского процесса.|
|parentProcessName|String|Имя файла образа родительского процесса.|
|path|String|Полный путь, включающий имя файла.|
|processId|Int32|Идентификатор (PID) процесса.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.process"
}-->

```json
{
  "accountName": "String",
  "commandLine": "String",
  "createdDateTime": "String (timestamp)",
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
  "isElevated": true,
  "name": "String",
  "parentProcessCreatedDateTime": "String (timestamp)",
  "parentProcessId": 1024,
  "parentProcessName": "String",
  "path": "String",
  "processId": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->