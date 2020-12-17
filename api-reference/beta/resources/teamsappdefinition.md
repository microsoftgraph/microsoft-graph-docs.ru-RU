---
title: Тип ресурса teamsAppDefinition
description: Сведения об одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6b5fd771d1fb38de5354c74778f5eae798ccc91e
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706117"
---
# <a name="teamsappdefinition-resource-type"></a>Тип ресурса teamsAppDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сведения о версии [teamsApp.](teamsapp.md)

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | string   | Уникальный ид (не appid teams). |
| teamsAppId          | string   | ИД из манифеста приложения Teams. |
| publishingState| string|Состояние публикации определенной версии приложения Teams. Возможные значения:</br>`submitted` — конкретная версия приложения Teams была отправлена и находится на рассмотрении. </br>`published`  — запрос на публикацию определенной версии приложения Teams утвержден администратором, и приложение опубликовано. </br> `rejected` — запрос на публикацию определенной версии приложения Teams был отклонен администратором. |
| azureADAppId        | string   | WebApplicationInfo.id из манифеста приложения Teams. |
| displayName         | string   | Имя приложения, предоставленное разработчиком приложения. |
| version             | string   | Номер версии приложения. |

## <a name="relationships"></a>Связи

| Связь | Тип   | Описание |
|:---------------|:--------|:----------|
|bot|[teamworkBot](teamworkbot.md) | Сведения о боте, указанном в манифесте приложения Teams. |

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "Test App",
  "version": "1.0.0"
}
```

## <a name="see-also"></a>См. также

- [teamsApp](teamsapp.md)
- [teamsAppInstallation](teamsappinstallation.md)
- [teamsTab](../resources/teamstab.md)

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


