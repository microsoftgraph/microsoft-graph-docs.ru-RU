---
title: Тип ресурса Теамсаппинсталлатион
description: 'TeamsApp, установленный в команде. '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1a76d11472b3faef95e87ed4724f1397ebe467a6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033784"
---
# <a name="teamsappinstallation-resource-type"></a>Тип ресурса Теамсаппинсталлатион

[TeamsApp](teamsapp.md) , установленный в [команде](team.md). Все боты, которые входят в состав приложения, станут частью любой команды, в которую добавляется приложение.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список приложений](../api/teamsappinstallation-list.md) | [teamsAppInstallation](teamsappinstallation.md) | Список приложений, установленных в команде.|
|[Добавление приложения](../api/teamsappinstallation-add.md) | [teamsAppInstallation](teamsappinstallation.md) | Добавляет (устанавливает) приложение в команду.|
|[Удаление приложения](../api/teamsappinstallation-delete.md) | Нет | Удаляет приложение из команды.|
|[Обновление приложения](../api/teamsappinstallation-upgrade.md) | Нет | Обновление до последней версии приложения.|

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | string   | Уникальный идентификатор (а не идентификаторы Teams). |

## <a name="relationships"></a>Отношения

| Отношение   | Тип    | Описание |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| Установленное приложение. |
|teamsAppDefinition|[teamsAppDefinition](teamsappdefinition.md)| Сведения о данной версии приложения. |

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
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
