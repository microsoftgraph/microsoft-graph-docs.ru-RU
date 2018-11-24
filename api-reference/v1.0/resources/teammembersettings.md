# <a name="teammembersettings-resource-type"></a>Тип ресурса teamMemberSettings



Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, в [группы](team.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|Логический|Если параметр имеет значение true, участники могли добавлять и обновлять каналов.|
|allowDeleteChannels|Логический|Если параметр имеет значение true, участники могут удалять каналы.|
|allowAddRemoveApps|Логический|Если параметр имеет значение true, участники могут добавлять и удалять приложения.|
|allowCreateUpdateRemoveTabs|Логический|Если параметр имеет значение true, участники могут добавлять, обновлять и удалять вкладки. |
|allowCreateUpdateRemoveConnectors|Логический|Если параметр имеет значение true, участники могут добавлять, обновлять и удалять соединители.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
