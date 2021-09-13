---
title: тип ресурса teamsAppDefinition
description: Представляет сведения об одной версии teamsApp.
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 923cba82d9def93b619545cf4184180ef220f247
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021430"
---
# <a name="teamsappdefinition-resource-type"></a>тип ресурса teamsAppDefinition

Пространство имен: microsoft.graph

Представляет сведения о версии [teamsApp.](teamsapp.md)

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | string   | Уникальный ID (не Teams ID приложения). |
| teamsAppId          | string   | ID из манифеста Teams приложения. |
| publishingState| string|Опубликованный статус определенной версии приложения Teams. Возможные значения:</br>`submitted`— конкретная версия Teams была представлена и находится на рассмотрении. </br>`published`— Запрос на публикацию конкретной версии приложения Teams утвержден администратором и приложение опубликовано. </br> `rejected`— Запрос на публикацию конкретной версии приложения Teams был отклонен администратором. |
| displayName         | string   | Имя приложения, предоставленного разработчиком приложения. |
| version             | string   | Номер версии приложения. |
| shortDescription    | string   | Краткое описание приложения. |
| description         | string   | Подробное описание приложения. |

## <a name="relationships"></a>Связи

| Связь | Тип   | Описание |
|:---------------|:--------|:----------|
|бот|[teamworkBot](teamworkbot.md) | Сведения о боте, указанном в манифесте Teams приложения. |

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

