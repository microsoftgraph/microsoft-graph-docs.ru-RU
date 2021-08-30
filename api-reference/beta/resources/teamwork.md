---
title: Тип ресурса teamwork
description: Контейнер для функций Microsoft Teams, доступных организации.
author: akjo
doc_type: resourcePageType
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 012286f43a6ab31f29062317077042ce43b587e9
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695905"
---
# <a name="teamwork-resource-type"></a>Тип ресурса teamwork

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для набора функциональных возможностей Microsoft Teams, доступных для организации.

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
  "@odata.type": "microsoft.graph.teamwork",
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
  "description": "teamwork resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a>См. также

- [Ресурс userTeamwork](userteamwork.md)


