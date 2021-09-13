---
title: тип ресурса userScopeTeamsAppInstallation
description: Представляет teamsApp, установленный в личной области пользователя.
author: AkJo
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e0ebe4544d419c7cdf4ea72c79b2e76fc231d004
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136259"
---
# <a name="userscopeteamsappinstallation-resource-type"></a>тип ресурса userScopeTeamsAppInstallation

Пространство имен: microsoft.graph

Представляет [teamsApp,](teamsapp.md) установленную в личной области [пользователя.](user.md) Все боты, которые являются частью приложения, станут частью личной области пользователя, в которую добавляется приложение.
Этот тип наследуется [от teamsAppInstallation.](teamsappinstallation.md)

> [!NOTE]
> `id`Ресурс **teamsAppInstallation** имеет не то же значение, что и `id` связанный ресурс **teamsApp**.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление приложений, установленных для пользователя](../api/userteamwork-list-installedapps.md)| Коллекция [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Список приложений, установленных в личной области пользователя. |
|[Получает установленное приложение для пользователя](../api/userteamwork-get-installedapps.md)| [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Список указанного приложения, установленного в личном поле пользователя. |
|[Добавление приложения для пользователя](../api/userteamwork-post-installedapps.md) | Нет | Добавьте (установите) приложение в личный круг пользователя. |
|[Удаление приложения для пользователя](../api/userteamwork-delete-installedapps.md) | Нет | Удалите (удалите) приложение в личной области пользователя. |
|[Обновление приложения, установленного для пользователя](../api/userteamwork-teamsappinstallation-upgrade.md) | Нет | Обновление до последней версии приложения, установленного в личном поле пользователя.|
|[Общение в чате между пользователем и приложением](../api/userscopeteamsappinstallation-get-chat.md) | [chat](chat.md) | Список чаты один на один между пользователем и приложением. |

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | string   | Уникальный ID (не Teams ID приложения). |

## <a name="relationships"></a>Отношения

| Связь   | Тип    | Описание |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| Установленное приложение. |
|teamsAppDefinition|[teamsAppDefinition](teamsappdefinition.md)| Сведения об этой версии приложения. |
|чат |[chat](chat.md) | Чат между пользователем и Teams приложением. | 

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

