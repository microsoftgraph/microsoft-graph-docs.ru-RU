---
title: Тип ресурса userTeamwork
description: 'Контейнер для функций Microsoft Teams, доступных пользователю. '
author: akjo
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 6ef5bb1ddf0944e7d61ab5321ae50e766713326c
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060439"
---
# <a name="userteamwork-resource-type"></a>Тип ресурса userTeamwork

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для набора функциональных возможностей Microsoft Teams, доступных для пользователя в клиенте.

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


