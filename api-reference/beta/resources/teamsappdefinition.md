---
title: тип ресурса teamsAppDefinition
description: Сведения об одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 205c656e81ed9dfc75e97cbe0734eeb36c5c0127
ms.sourcegitcommit: aa18eb8a9965f99cc97680808abba8df46f31ba5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2021
ms.locfileid: "51638909"
---
# <a name="teamsappdefinition-resource-type"></a>тип ресурса teamsAppDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сведения о версии [teamsApp](teamsapp.md).

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | string   | Уникальный id (а не командный appid). |
| teamsAppId          | Строка   | Id из манифеста Teams App. |
| publishingState| Строка|Опубликованный статус определенной версии приложения Teams. Возможные значения:</br>`submitted` — конкретная версия приложения Teams была представлена и находится на рассмотрении. </br>`published`  — Запрос на публикацию конкретной версии приложения Teams был утвержден администратором и приложение опубликовано. </br> `rejected` — Запрос на публикацию конкретной версии приложения Teams был отклонен администратором. |
| azureADAppId        | Строка   | В WebApplicationInfo.id из манифеста Teams App. |
| displayName         | string   | Имя приложения, предоставленного разработчиком приложения. |
| version             | Строка   | Номер версии приложения. |
| allowedInstallationScopes | teamsAppInstallationScope collection | Коллекция областей, в которых можно установить приложение Teams. Возможные значения:</br>`team` — указывает, что приложение Teams может быть установлено в команде и уполномочено получать доступ к данным этой группы. </br>`groupChat`  — указывает, что приложение Teams может быть установлено в групповом чате и уполномочено получать доступ к данным группового чата. </br> `personal` — указывает, что приложение Teams может быть установлено в личном поле пользователя и уполномочено получать доступ к данным этого пользователя. | 

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


