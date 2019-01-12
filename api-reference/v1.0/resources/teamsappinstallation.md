---
title: Тип ресурса teamsAppInstallation
description: 'TeamsApp, установленные в группе. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 153b131cd24709995d7215b1cf568a8565f42a80
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929482"
---
# <a name="teamsappinstallation-resource-type"></a>Тип ресурса teamsAppInstallation



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

