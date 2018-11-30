---
title: Тип ресурса teamsAppInstallation
description: 'TeamsApp, установленные в группе. '
ms.openlocfilehash: 64573e163c0ec5ce9f3282e747dffd4ccc6718de
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077813"
---
# <a name="teamsappinstallation-resource-type"></a>Тип ресурса teamsAppInstallation

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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

| Связь   | Тип    | Description |
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

