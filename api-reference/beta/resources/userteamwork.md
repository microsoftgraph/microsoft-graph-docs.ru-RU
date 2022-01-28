---
title: Тип ресурса userTeamwork
description: 'Контейнер для функций Microsoft Teams, доступных пользователю. '
author: akjo
doc_type: resourcePageType
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: ff6a364ed21286d2fb01791bc0ccef0997f3ab5f
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262227"
---
# <a name="userteamwork-resource-type"></a>Тип ресурса userTeamwork

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для набора функциональных возможностей Microsoft Teams, доступных для пользователя в клиенте.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление installedApps](../api/userteamwork-list-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md) collection|Получение списка приложений, установленных в личной области указанного пользователя.|

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|id|string| Уникальный идентификатор. |

## <a name="relationships"></a>Связи

| Связь | Тип | Описание |
|:---------------|:--------|:----------|
|installedApps|[teamsAppInstallation](teamsappinstallation.md) collection|Приложения, установленные в личной области пользователя.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userTeamwork",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "userteamwork resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a>См. также

- [Тип ресурса teamwork](teamwork.md)