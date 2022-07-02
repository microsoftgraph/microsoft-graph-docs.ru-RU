---
title: Тип ресурса teamwork
description: Контейнер для функций Microsoft Teams, доступных организации.
author: akjo
doc_type: resourcePageType
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 8a6a07a23d71c79703643dc5280bd531eb5a5843
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577875"
---
# <a name="teamwork-resource-type"></a>Тип ресурса teamwork

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для набора функциональных возможностей Microsoft Teams, доступных для организации.

## <a name="methods"></a>Методы

| Метод                                                  | Возвращаемый тип                                         |Описание                                                                               |
|:--------------------------------------------------------|:----------------------------------------------------|:-----------------------------------------------------------------------------------------|
|[Список deletedTeams](../api/teamwork-list-deletedteams.md)|Коллекция [deletedTeam](../resources/deletedteam.md)|Получение списка объектов [deletedTeam](../resources/deletedteam.md) и их свойств.|

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|id|string| Уникальный идентификатор. |

## <a name="relationships"></a>Связи

| Связь | Тип | Описание |
|:---------------|:--------|:----------|
|deletedTeams|Коллекция [deletedTeam](../resources/deletedteam.md)| Коллекция удаленных команд.|
|devices|коллекция [teamworkDevice](../resources/teamworkdevice.md)|Устройства Teams, подготовленные для клиента.|
|workforceIntegrations|коллекция [workforceIntegration](../resources/workforceintegration.md)| Интеграция рабочих ресурсов со сменами.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamwork",
  "baseType": "microsoft.graph.entity"
}-->

``` json
{
    "@odata.type": "#microsoft.graph.teamwork",
    "id": "String (identifier)"
}
```

## <a name="see-also"></a>См. также

- [Ресурс userTeamwork](userteamwork.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamwork resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
