---
title: тип ресурса teamsAppDefinition
description: Сведения об одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4e8bfd4b7248d37ce8ec4d85e01a498a88fed1c3
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882322"
---
# <a name="teamsappdefinition-resource-type"></a>тип ресурса teamsAppDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сведения о версии [teamsApp](teamsapp.md).

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание                                            |
|:------------------- |:-------- |:------------------------------------------------------ |
| id                  | string   | Уникальный ID (а не ID приложения Teams).                     |
| teamsAppId          | Строка   | ID из манифеста приложения Teams.                    |
| publishingState     | Строка   | Опубликованный статус определенной версии приложения Teams. Возможные значения:</br>`submitted` — конкретная версия приложения Teams была представлена и находится на рассмотрении. </br>`published`  — Запрос на публикацию конкретной версии приложения Teams был утвержден администратором и приложение опубликовано. </br> `rejected` — Запрос на публикацию конкретной версии приложения Teams был отклонен администратором. |
| azureADAppId        | Строка   | В WebApplicationInfo.Id из манифеста приложения Teams. |
| displayName         | string   | Имя приложения, предоставленного разработчиком приложения.     |
| version             | Строка   | Номер версии приложения.                 |
| allowedInstallationScopes | teamsAppInstallationScope collection | Коллекция областей, в которых можно установить приложение Teams. Возможные значения:</br>`team` — указывает, что приложение Teams может быть установлено в команде и уполномочено получать доступ к данным этой группы. </br>`groupChat`  — указывает, что приложение Teams может быть установлено в групповом чате и уполномочено получать доступ к данным группового чата. </br> `personal` — указывает, что приложение Teams может быть установлено в личном поле пользователя и уполномочено получать доступ к данным этого пользователя. | 

## <a name="relationships"></a>Связи

| Связь   | Тип                           | Описание                                                 |
|:-------------- |:------------------------------ |:----------------------------------------------------------- |
| бот            |[teamworkBot](teamworkbot.md)   | Сведения о боте, указанном в манифесте приложения Teams. |
| colorIcon      |[teamsAppIcon](teamsappicon.md) | Цветная версия значка приложения Teams.                   |
| outlineIcon    |[teamsAppIcon](teamsappicon.md) | Очертания версии значка приложения Teams.                 |

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
  "publishingState": "#microsoft.graph.teamsAppPublishingState",
  "azureADAppId": "string",
  "displayName": "string",
  "version": "string"
}
```

## <a name="see-also"></a>См. также

- [teamsApp](teamsapp.md)
- [teamsAppIcon](teamsappicon.md)
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


