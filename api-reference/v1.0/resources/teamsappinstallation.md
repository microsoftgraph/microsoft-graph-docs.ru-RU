# <a name="teamsappinstallation-resource-type"></a>Тип ресурса teamsAppInstallation



[TeamsApp](teamsapp.md) установлен в [группы](team.md). Любой программы-роботы, являющихся частью приложения становится частью любой группы добавляется приложение.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список приложений](../api/teamsappinstallation_list.md) | [teamsAppInstallation](teamsapp.md) | Список приложений, установленные в группе.|
|[Добавить приложение](../api/teamsappinstallation_add.md) | [teamsAppInstallation](teamsapp.md) | Добавляет (установить) приложения в группу.|
|[Удаление приложения](../api/teamsappinstallation_delete.md) | Отсутствует | Удаляет (удаление) приложения из группы.|
|[Обновление приложения](../api/teamsappinstallation_delete.md) | Отсутствует | Обновление до последней версии приложения.|

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | строка   | Уникальный идентификатор (не appid команды). |

## <a name="relationships"></a>Связи

| Связь   | Тип    | Описание |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| Приложения, которая устанавливается. |
|teamsAppDefinition|[teamsAppDefinition](teamsapp.md)| Подробные сведения о данной версии приложения. |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
}
```

# <a name="see-also"></a>См. также

- [teamsApp](teamsapp.md)
- [teamsAppDefinition](teamsappdefinition.md)
- [teamsTab](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

