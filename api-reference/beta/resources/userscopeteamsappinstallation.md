---
title: Тип ресурса Усерскопетеамсаппинсталлатион
description: Представляет teamsApp, установленный в личной области пользователя.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 70ebdcb30c67d59e3a12c4a0514314015e163c17
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607023"
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
|[Добавление приложения для пользователя](../api/userteamwork-post-installedapps.md) | Нет | Добавляет (устанавливает) приложение в личную область пользователя. |
|[Удаление приложения для пользователя](../api/userteamwork-delete-installedapps.md) | Нет | Удаляет приложение из персональной области пользователя. |
|[Обновление приложения, установленного для пользователя](../api/userteamwork-teamsappinstallation-upgrade.md) | Нет | Обновление до последней версии приложения, установленного в личной области пользователя.|
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

