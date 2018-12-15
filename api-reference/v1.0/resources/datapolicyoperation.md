# <a name="datapolicyoperation-resource-type"></a>Тип ресурса dataPolicyOperation

Представляет операцию политики отправленных данных. Он содержит сведения, необходимые для отслеживания состояния операции. Например администратор компании запрос данных политики операции экспорта данных сотрудника компании и затем отслеживать этот запрос.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение dataPolicyOperation](../api/datapolicyoperation-get.md) | [dataPolicyOperation](datapolicyoperation.md) |Извлечение свойств объекта **dataPolicyOperation** .|
|[Экспорт личных данных](../api/user-exportpersonaldata.md) | Нет |Запрос данных политики операция экспортировать данные организации пользователя, можно просмотреть более поздней версии с помощью [получения dataPolicyOperation](../api/datapolicyoperation-get.md)|

## <a name="properties"></a>Свойства

> **Примечание:** Все свойства в этом ресурсов доступны только для чтения.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|completedDateTime|DateTimeOffset|Представляет, когда запрос для этой операции политики данных был выполнен, в формате UTC, в формате ISO 8601. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. NULL до завершения операции.|
|id|Строка| Уникальный ключ для этой операции. |
|status|строка| Возможные значения: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.|
|storageLocation|String.|URL-адрес расположения, в котором выполняется экспорт данных для запросы на экспорт.|
|userId|String|Идентификатор пользователя, для которого выполняется операция.|
|submittedDateTime|DateTimeOffset|Представляет, когда для этой операции с данными был отправлен запрос, в формате UTC, в формате ISO 8601. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Ход выполнения|String.|Указывает ход выполнения операции.|

## <a name="relationships"></a>Связи
Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dataPolicyOperation"
}-->

```json
{
  "completedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "status": "string",
  "storageLocation": "String",
  "userId": "String",
  "submittedDateTime": "String (timestamp)", 
  "progress": "String (double)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dataPolicyOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
