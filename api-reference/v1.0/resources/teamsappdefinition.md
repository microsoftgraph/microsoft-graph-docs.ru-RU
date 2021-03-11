---
title: тип ресурса teamsAppDefinition
description: Представляет сведения об одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8a43083e1f7fb717e2d54caef4017aeae97d9392
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625935"
---
# <a name="teamsappdefinition-resource-type"></a>тип ресурса teamsAppDefinition

Пространство имен: microsoft.graph

Представляет сведения о версии [teamsApp.](teamsapp.md)

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | string   | Уникальный ID (а не ID приложения Teams). |
| teamsAppId          | Строка   | ID из манифеста приложения Teams. |
| publishingState| Строка|Опубликованный статус определенной версии приложения Teams. Возможные значения:</br>`submitted` — конкретная версия приложения Teams была представлена и находится на рассмотрении. </br>`published`  — Запрос на публикацию конкретной версии приложения Teams был утвержден администратором и приложение опубликовано. </br> `rejected` — Запрос на публикацию конкретной версии приложения Teams был отклонен администратором. |
| displayName         | string   | Имя приложения, предоставленного разработчиком приложения. |
| version             | Строка   | Номер версии приложения. |
| shortDescription    | Строка   | Краткое описание приложения. |
| description         | string   | Подробное описание приложения. |

## <a name="relationships"></a>Связи

| Связь | Тип   | Описание |
|:---------------|:--------|:----------|
|бот|[teamworkBot](teamworkbot.md) | Сведения о боте, указанном в манифесте приложения Teams. |

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
  "displayName": "string",
  "version": "string"
}
```

## <a name="see-also"></a>См. также

- [teamsApp](teamsapp.md)
- [teamsAppInstallation](teamsappinstallation.md)
- [teamsTab](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

