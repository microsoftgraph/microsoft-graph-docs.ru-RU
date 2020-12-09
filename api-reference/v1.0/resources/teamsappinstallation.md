---
title: Тип ресурса Теамсаппинсталлатион
description: Представляет teamsApp, установленный в команде или персональную область пользователя.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1c872d41ebc09978d9dc54ac01d82cb33258541d
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607037"
---
# <a name="teamsappinstallation-resource-type"></a>Тип ресурса Теамсаппинсталлатион

Пространство имен: microsoft.graph

Представляет [teamsApp](teamsapp.md) , установленный в [команде](team.md) или персональную область [пользователя](user.md). Все боты, которые входят в состав приложения, станут частью любой рабочей группы или пользователя, к которому добавляется приложение.

> [!NOTE]
> `id`Ресурс **теамсаппинсталлатион** имеет не то же значение, что и `id` связанный ресурс **teamsApp** .

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список приложений, установленных в Team](../api/team-list-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) collection | Список приложений, установленных в команде.|
|[Получение приложения, установленного в команде](../api/team-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | Получение указанного приложения, установленного в команде.|
|[Добавление приложения в команду](../api/team-post-installedapps.md) |Нет | Добавление приложения в группу (установка).|
|[Удаление приложения из группы](../api/team-delete-installedapps.md) | Нет | Удаление приложения из команды (удаление).|
|[Обновление приложения, установленного в команде](../api/team-teamsappinstallation-upgrade.md) | Нет | Обновите приложение, установленное в команде, до последней версии.|
|[Перечисление приложений, установленных для пользователя](../api/userteamwork-list-installedapps.md) | Коллекция [усерскопетеамсаппинсталлатион](userscopeteamsappinstallation.md) | Список приложений, установленных в личной области пользователя.|
|[Получение приложения, установленного для пользователя](../api/userteamwork-get-installedapps.md)| [усерскопетеамсаппинсталлатион](userscopeteamsappinstallation.md) | Получение указанного приложения, установленного в личной области пользователя. |
|[Добавление приложения для пользователя](../api/userteamwork-post-installedapps.md) | | Добавление (установка) приложения в личной области пользователя.|
|[Удаление приложения для пользователя](../api/userteamwork-delete-installedapps.md) | Нет | Удалить (удалить) приложение в личной области пользователя.|
|[Обновление приложения, установленного для пользователя](../api/userteamwork-teamsappinstallation-upgrade.md) | Нет | Обновление приложения, установленного в личной области пользователя, до последней версии.|


## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | string   | Уникальный идентификатор (не идентификатор приложения Teams). |

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
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
  "suppressions": []
}-->

