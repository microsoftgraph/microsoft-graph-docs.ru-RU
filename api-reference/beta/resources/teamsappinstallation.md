---
title: Тип ресурса teamsAppInstallation
description: 'TeamsApp, установленные в группе. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b4cf14c36fc0ab0b33f88d4b330e76957e65164a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512838"
---
# <a name="teamsappinstallation-resource-type"></a>Тип ресурса teamsAppInstallation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[TeamsApp](teamsapp.md) установлен в [группы](team.md). Любой программы-роботы, являющихся частью приложения становится частью любой группы добавляется приложение.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список приложений](../api/teamsappinstallation-list.md) | [teamsAppInstallation](teamsapp.md) | Список приложений, установленные в группе.|
|[Добавить приложение](../api/teamsappinstallation-add.md) | [teamsAppInstallation](teamsapp.md) | Добавляет (установить) приложения в группу.|
|[Удаление приложения](../api/teamsappinstallation-delete.md) | Нет | Удаляет (удаление) приложения из группы.|
|[Обновление приложения](../api/teamsappinstallation-delete.md) | Нет | Обновление до последней версии приложения.|

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | string   | Уникальный идентификатор (не appid команды). |

## <a name="relationships"></a>Отношения

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
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstallation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

