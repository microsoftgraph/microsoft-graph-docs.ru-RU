# <a name="historyitem-resource-type"></a>Тип ресурса historyItem

Представляет элемент журнала для [действия](projectrome_activity.md) в приложении. Действия пользователя представляют собой отдельный пункт назначения в вашем приложении - например, телешоу, документ или текущую кампанию в видеоигре. Когда пользователь подключает это действие, это задействование регистрируется как элемент журнала, указывающий время начала и окончания для этого действия. По мере того как пользователь повторно подключает это действие с течением времени, в журнал записывается несколько элементов для одного действия пользователя.

Когда приложение создает сеанс, объект **historyItem** следует добавить к объекту **activity**, чтобы отразить период задействования пользователя. При каждом следующем взаимодействии пользователя с действием, к действию добавляется новый элемент **historyItem** для контроля задействования пользователя.

## <a name="methods"></a>Методы

|Метод | Возвращаемый тип | Описание|
|:------|:------------|:-----------|
|[Создать или заменить historyItem](../api/projectrome_put_historyitem.md) | [historyItem](projectrome_historyitem.md) | Создает или заменяет существующий **historyItem** для этого действия (обновление или вставка).  ID должен быть идентификатором GUID.|
|[Удалить historyItem](../api/projectrome_delete_historyitem.md) | Нет содержимого | Удаляет указанный **historyItem** для этого действия.|

## <a name="properties"></a>Свойства

|Имя | Тип | Описание|
|:----|:-----|:-----------|
|status | status | Устанавливается сервером. Код состояния, используемый для идентификации допустимых объектов. Значения: активный, обновлён, удалён, игнорируется.|
|userTimezone | String | Необязательный параметр. Часовой пояс, в котором устройство пользователя, используемое для создания действия, находилось во время создания действия. Значения, представленные как Олсон-идентификаторы для поддержки кросс-платформенного представления.|
|createdDateTime | DateTimeOffset | Устанавливается сервером. Дата и время создания объекта на сервере в формате UTC.|
|lastModifiedDateTime | DateTimeOffset | Устанавливается сервером. Дата и время изменения объекта на сервере в формате UTC.|
|id | Строка | Обязательно. Идентификатор GUID набора клиента для объекта **historyItem**.|
|startedDateTime | DateTimeOffset | Обязательный. Дата и время в формате UTC запуска **historyItem** (сеанса действия). Требуется для журнала временной шкалы.|
|lastActiveDateTime | DateTimeOffset | Необязательный параметр. Дата и время в формате UTC, когда **historyItem** (сеанс действия) в последний раз считался активным или законченным. Если значение null, статус **historyItem** должен быть Ongoing.|
|expirationDateTime | DateTimeOffset | Необязательный параметр. Дата и время в формате UTC, когда **historyItem** будет окончательно удален. Может быть задано клиентом.|
|activeDurationSeconds | int | Необязательный параметр. Длительность задействования активного пользователя. Если не указано, вычисляется по **startedDateTime** и **lastActiveDateTime**.|

## <a name="relationships"></a>Связи

|Связь | Тип | Описание|
|:------------|:-----|:-----------|
|activity| [userActivity](../resources/projectrome_activity.md) | Необязательный параметр. NavigationProperty/Containment; свойство навигации для связанного действия.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.activityHistoryItem",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
    "status": "active | updated | deleted | ignored",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "id": "String",
    "expirationDateTime": "DateTimeOffset",
    "startedDateTime": "DateTimeOffset",
    "userTimezone": "String",
    "lastActiveDateTime": "DateTimeOffset",
    "activeDurationSeconds":"int"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
