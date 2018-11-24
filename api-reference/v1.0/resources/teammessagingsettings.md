# <a name="teammessagingsettings-resource-type"></a>Тип ресурса teamMessagingSettings



Параметры для настройки системы обмена сообщениями и упоминания в [группы](team.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowUserEditMessages|Логический|Если параметр имеет значение true, пользователи могут изменять свои сообщения;|
|allowUserDeleteMessages|Логический|Если параметр имеет значение true, пользователи могут удалять свои сообщения.|
|allowOwnerDeleteMessages|Логический|Если параметр имеет значение true, владельцы могут удалять все сообщения.|
|allowTeamMentions|Логический|Если задано значение true, допускаются упоминания @team.|
|allowChannelMentions|Логический|Если задано значение true, допускаются упоминания @channel.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}-->

```json
{
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
