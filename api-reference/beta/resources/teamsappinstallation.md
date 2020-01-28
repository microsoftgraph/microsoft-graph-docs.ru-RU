---
title: Тип ресурса Теамсаппинсталлатион
description: 'TeamsApp, установленный в команде, в чате или в личной области пользователя. '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9aa86509fdbcdaa49d07987eacbfe763b848408a
ms.sourcegitcommit: 0f39f39a1c0300ef013ebd12e4df2b5ba4dabbf8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2020
ms.locfileid: "41559049"
---
# <a name="teamsappinstallation-resource-type"></a>Тип ресурса Теамсаппинсталлатион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[TeamsApp](teamsapp.md) , установленный в [команде](team.md), в [чате](chat.md)или в личной области [пользователя](user.md). Все боты, которые входят в состав приложения, станут частью любой группы, чата или пользователя, к которому добавляется приложение.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список приложений, установленных в Team](../api/teamsappinstallation-list.md) | [teamsAppInstallation](teamsappinstallation.md) collection | Список приложений, установленных в команде.|
|[Добавление приложения в команду](../api/teamsappinstallation-add.md) |Нет | Добавляет (устанавливает) приложение в команду.|
|[Удаление приложения из группы](../api/teamsappinstallation-delete.md) | Нет | Удаляет приложение из команды.|
|[Обновление приложения, установленного в команде](../api/teamsappinstallation-upgrade.md) | Нет | Обновление до последней версии приложения, установленного в команде.|
|[Перечисление приложений, установленных для пользователя](../api/user-list-teamsappinstallation.md) | [teamsAppInstallation](teamsappinstallation.md) collection | Список приложений, установленных в личной области пользователя.|
|[Добавление приложения для пользователя](../api/user-add-teamsappinstallation.md) | | Добавляет (устанавливает) приложение в личную область пользователя.|
|[Удаление приложения для пользователя](../api/user-delete-teamsappinstallation.md) | Нет | Удаляет приложение из персональной области пользователя.|
|[Обновление приложения, установленного для пользователя](../api/user-upgrade-teamsappinstallation.md) | Нет | Обновление до последней версии приложения, установленного в личной области пользователя.|

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | string   | Уникальный идентификатор (не идентификатор AP группы). |

## <a name="relationships"></a>Связи

| Связь   | Тип    | Описание |
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

## <a name="see-also"></a>См. также

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
  "suppressions": []
}
-->
