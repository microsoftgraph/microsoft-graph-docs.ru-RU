---
title: Тип ресурса Теамсаппинсталлатион
description: 'TeamsApp, установленный в команде, в чате или в личной области пользователя. '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f5775514eb242f540bc6740d8e21620448f2d280
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563641"
---
# <a name="teamsappinstallation-resource-type"></a>Тип ресурса Теамсаппинсталлатион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[TeamsApp](teamsapp.md) , установленный в [команде](team.md), в [чате](chat.md)или в личной области [пользователя](user.md). Все боты, которые входят в состав приложения, станут частью любой группы, чата или пользователя, к которому добавляется приложение.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список приложений, установленных в Team](../api/teamsappinstallation-list.md) | [teamsAppInstallation](teamsappinstallation.md) collection | Список приложений, установленных в команде.|
|[Получение приложения, установленного в команде](../api/team-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | Список приложений, установленных в команде.|
|[Добавление приложения в команду](../api/teamsappinstallation-add.md) |Нет | Добавляет (устанавливает) приложение в команду.|
|[Удаление приложения из группы](../api/teamsappinstallation-delete.md) | Нет | Удаляет приложение из команды.|
|[Обновление приложения, установленного в команде](../api/teamsappinstallation-upgrade.md) | Нет | Обновление до последней версии приложения, установленного в команде.|
|[Перечисление приложений, установленных для пользователя](../api/userteamwork-list-installedapps.md) | Коллекция [усерскопетеамсаппинсталлатион](userscopeteamsappinstallation.md) | Список приложений, установленных в личной области пользователя.|
|[Получает установленное приложение для пользователя](../api/userteamwork-get-installedapps.md)| [усерскопетеамсаппинсталлатион](userscopeteamsappinstallation.md) | Перечисление указанного приложения, установленного в личной области пользователя. |
|[Добавление приложения для пользователя](../api/userteamwork-add-installedapps.md) | | Добавляет (устанавливает) приложение в личную область пользователя.|
|[Удаление приложения для пользователя](../api/userteamwork-delete-installedapps.md) | Нет | Удаляет приложение из персональной области пользователя.|
|[Обновление приложения, установленного для пользователя](../api/userteamwork-upgrade-installedapps.md) | Нет | Обновление до последней версии приложения, установленного в личной области пользователя.|

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
- [усерскопетеамсаппинсталлатион](../resources/userscopeteamsappinstallation.md)

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


