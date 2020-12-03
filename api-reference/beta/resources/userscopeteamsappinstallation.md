---
title: Тип ресурса Усерскопетеамсаппинсталлатион
description: Представляет teamsApp, установленный в личной области пользователя.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 19ca16e4d6a3171cc622440ee79dce3d93e8dd84
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564240"
---
# <a name="userscopeteamsappinstallation-resource-type"></a>Тип ресурса Усерскопетеамсаппинсталлатион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет [teamsApp](teamsapp.md) , установленный в личной области [пользователя](user.md). Все боты, которые входят в состав приложения, станут частью личной области пользователя, в которую добавляется приложение.
Этот тип наследуется от [теамсаппинсталлатион](teamsappinstallation.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление приложений, установленных для пользователя](../api/userteamwork-list-installedapps.md)| Коллекция [усерскопетеамсаппинсталлатион](userscopeteamsappinstallation.md) | Список приложений, установленных в личной области пользователя. |
|[Получение приложения, установленного для пользователя](../api/userteamwork-get-installedapps.md)| [усерскопетеамсаппинсталлатион](userscopeteamsappinstallation.md) | Список указанного приложения, установленного в личной области пользователя. |
|[Добавление приложения для пользователя](../api/userteamwork-add-installedapps.md) | Нет | Добавляет (устанавливает) приложение в личную область пользователя. |
|[Удаление приложения для пользователя](../api/userteamwork-delete-installedapps.md) | Нет | Удаляет приложение из персональной области пользователя. |
|[Обновление приложения, установленного для пользователя](../api/userteamwork-upgrade-installedapps.md) | Нет | Обновление до последней версии приложения, установленного в личной области пользователя.|
|[Получение разговора между пользователем и приложением](../api/userscopeteamsappinstallation-get-chat.md) | [chat](chat.md) | Перечисление одного сеанса разговора между пользователем и приложением. |

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | string   | Уникальный идентификатор (не идентификатор приложения Teams). |

## <a name="relationships"></a>Связи

| Связь   | Тип    | Описание |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| Установленное приложение. |
|teamsAppDefinition|[teamsAppDefinition](teamsappdefinition.md)| Сведения о данной версии приложения. |
|чат |[chat](chat.md) | Чат между пользователем и приложением Teams. | 

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userScopeTeamsAppInstallation",
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
<!-- {
  "type": "#page.annotation",
  "description": "userScopeTeamsAppInstallation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
  "suppressions": []
}-->

