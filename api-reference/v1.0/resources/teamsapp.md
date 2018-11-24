# <a name="teamsapp-resource-type"></a>Тип ресурса teamsApp



Приложение в каталоге приложений [Группами Майкрософт](teams_api_overview.md) .

Пользователи могут видеть эти приложения в магазине группами Майкрософт, и эти приложения может быть установлена с [группами](team.md) с помощью метода [Add приложения в группу](../api/teamsappinstallation_add.md) .

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список опубликованных приложений](../api/teamsapp_list.md) | [teamsApp](teamsApp.md) коллекции | Список опубликованных приложений из каталога приложений группами Майкрософт.|
|[Публикация приложения](../api/teamsapp_publish.md) | [teamsApp](teamsApp.md) | Публикация приложения в каталоге приложений организации.|
|[Обновление опубликованного приложения](../api/teamsapp_update.md) | [teamsApp](teamsApp.md) | Обновление опубликованного приложения в каталоге приложений организации.|
|[Удаление опубликованного приложения](../api/teamsapp_delete.md) | Отсутствует | Удаление опубликованного приложения из каталога приложений вашей организации.|

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | строка   | Приложения каталога созданный код приложения (отличный от предоставленного для разработчиков ID в [пакет приложения zip группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). |
| externalId          | string   | Идентификатор каталога, предоставляемый разработчиком приложения в [пакет приложения ZIP-группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). |
| displayName                | строка   | Имя каталога приложения, предоставляемый разработчиком приложения в [пакет приложения ZIP-группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). |
| distributionMethod  | teamsAppDistributionMethod     | Метод распространения для приложения. |

### <a name="teamsappdistributionmethod-values"></a>teamsAppDistributionMethod значения

|Элемент|Значение|Описание|
|:---|:---|:---|
|хранилище|0| Приложение доступно для всех клиентов через хранилище приложений группами Майкрософт.|
|organization;|1|Приложение доступно только при этом клиента.|
|sideloaded|2|Приложение будет доступно только для пользователей/групп его установленных для.|

## <a name="relationships"></a>Связи

| Связь | Тип   | Описание |
|:---------------|:--------|:----------|
|appDefinitions|[teamsAppDefinition](teamsappdefinition.md) коллекции| Подробные сведения для каждой версии приложения. |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsApp",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "externalId": "string",
  "displayName": "Test App",
  "distributionMethod": "Organization"
}
```

# <a name="see-also"></a>См. также

- [teamsAppInstallation](teamsappinstallation.md)
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

