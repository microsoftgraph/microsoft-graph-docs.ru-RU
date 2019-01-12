---
title: Тип ресурса teamsApp
description: Приложение в каталоге приложений группами Майкрософт.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2f1b45f60e9586d148a08310e9d19b1a3e6c52e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912059"
---
# <a name="teamsapp-resource-type"></a>Тип ресурса teamsApp

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Приложение в каталоге приложений [Группами Майкрософт](teams-api-overview.md) .

Пользователи могут видеть эти приложения в магазине группами Майкрософт, и эти приложения может быть установлена с [группами](team.md) с помощью метода [Add приложения в группу](../api/teamsappinstallation-add.md) .

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список опубликованных приложений](../api/teamsapp-list.md) | [teamsApp](teamsapp.md) коллекции | Список опубликованных приложений из каталога приложений группами Майкрософт.|
|[Публикация приложения](../api/teamsapp-publish.md) | [teamsApp](teamsapp.md) | Публикация приложения в каталоге приложений организации.|
|[Обновление опубликованного приложения](../api/teamsapp-update.md) | [teamsApp](teamsapp.md) | Обновление опубликованного приложения в каталоге приложений организации.|
|[Удаление опубликованного приложения](../api/teamsapp-delete.md) | Нет | Удаление опубликованного приложения из каталога приложений вашей организации.|

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | строка   | Приложения каталога созданный код приложения (отличный от предоставленного для разработчиков ID в [пакет приложения zip группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). |
| externalId          | string   | Идентификатор каталога, предоставляемый разработчиком приложения в [пакет приложения ZIP-группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). |
| displayName                | строка   | Имя каталога приложения, предоставляемый разработчиком приложения в [пакет приложения ZIP-группами Майкрософт](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). |
| distributionMethod  | teamsAppDistributionMethod     | Метод распространения для приложения. |

### <a name="teamsappdistributionmethod-values"></a>teamsAppDistributionMethod значения

|Член|Значение|Описание|
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

