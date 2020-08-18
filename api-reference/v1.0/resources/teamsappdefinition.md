---
title: Тип ресурса Теамсаппдефинитион
description: Представляет сведения о одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 322b7f50ccb51702ae05ca55f8e73396321a0283
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791682"
---
# <a name="teamsappdefinition-resource-type"></a>Тип ресурса Теамсаппдефинитион

Пространство имен: microsoft.graph

Представляет сведения о одной версии [teamsApp](teamsapp.md).

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | string   | Уникальный идентификатор (не идентификатор приложения Teams). |
| teamsAppId          | string   | ИДЕНТИФИКАТОР из манифеста приложения Teams. |
| publishingState| string|Опубликованное состояние определенной версии приложения Teams. Возможные значения:</br>`submitted` — Определенная версия приложения Teams была отправлена и находится в процессе рецензирования. </br>`published`  — Запрос на публикацию определенной версии приложения Teams утвержден администратором, и приложение публикуется. </br> `rejected` — Запрос на публикацию определенной версии приложения Teams был отклонен администратором. |
| displayName         | string   | Имя приложения, предоставленное разработчиком приложения. |
| version             | string   | Номер версии приложения. |

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
  "version": "string",
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
