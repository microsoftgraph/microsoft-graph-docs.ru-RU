---
title: тип ресурса teamsAppInstallation
description: Представляет teamsApp, установленную в команде или в личной области пользователя.
author: AkJo
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 81626d05c7cc417b083b8c08b0fab02cc0dbad08
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128187"
---
# <a name="teamsappinstallation-resource-type"></a>тип ресурса teamsAppInstallation

Пространство имен: microsoft.graph

Представляет [teamsApp,](teamsapp.md) установленную в [команде или](team.md) в личной области [пользователя.](user.md) Все боты, которые являются частью приложения, станут частью личной области любой команды или пользователя, в которую добавляется приложение.

> [!NOTE]
> `id`Ресурс **teamsAppInstallation** имеет не то же значение, что и `id` связанный ресурс **teamsApp**.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление приложений, установленных в команде](../api/team-list-installedapps.md) | Коллекция [teamsAppInstallation](teamsappinstallation.md) | Перечисление приложений, установленных в команде.|
|[Получение приложения, установленного в команде](../api/team-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | Получение указанного приложения, установленного в команде.|
|[Добавление приложения в команду](../api/team-post-installedapps.md) |Нет | Добавление (установка) приложения в команду.|
|[Обновление приложения, установленного в команде](../api/team-teamsappinstallation-upgrade.md) | Нет | Обновление приложения, установленного в команде, до последней версии.|
|[Удаление приложения из команды](../api/team-delete-installedapps.md) | Нет | Удаление приложения из команды.|
|[Перечисление приложений, установленных для пользователя](../api/userteamwork-list-installedapps.md) | Коллекция [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Список приложений, установленных в личной области пользователя.|
|[Установку приложения для пользователя](../api/userteamwork-get-installedapps.md)| [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Получите указанное приложение, установленное в личном поле пользователя. |
|[Добавление приложения для пользователя](../api/userteamwork-post-installedapps.md) | | Добавьте (установите) приложение в личный круг пользователя.|
|[Обновление приложения, установленного для пользователя](../api/userteamwork-teamsappinstallation-upgrade.md) | Нет | Обновление приложения, установленного в личном поле пользователя, до последней версии.|
|[Удаление приложения для пользователя](../api/userteamwork-delete-installedapps.md) | Нет | Удалите (удалите) приложение в личной области пользователя.|


## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | string   | Уникальный ID (не Teams ID приложения). |

## <a name="relationships"></a>Отношения

| Связь   | Тип    | Описание |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| Установленное приложение. |
|teamsAppDefinition|[teamsAppDefinition](teamsappdefinition.md)| Сведения об этой версии приложения. |


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
- [userScopeTeamsAppInstallation](../resources/userscopeteamsappinstallation.md)

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

