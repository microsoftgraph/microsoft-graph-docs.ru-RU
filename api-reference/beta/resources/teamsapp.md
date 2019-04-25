---
title: Тип ресурса teamsApp
description: Приложение в каталоге приложений Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fe60222ae6c5d8475722e18e69555df2d3892759
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553955"
---
# <a name="teamsapp-resource-type"></a>Тип ресурса teamsApp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Приложение в каталоге приложений [Microsoft Teams](teams-api-overview.md) .

Пользователи могут просматривать эти приложения в магазине Microsoft Teams, и эти приложения можно установить в Teams с помощью метода [Add App to Team](../api/teamsappinstallation-add.md) . [](team.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список опубликованных приложений](../api/teamsapp-list.md) | Коллекция [teamsApp](teamsapp.md) | Список опубликованных приложений из каталога приложений Microsoft Teams.|
|[Публикация приложения](../api/teamsapp-publish.md) | [teamsApp](teamsapp.md) | Опубликуйте приложение в каталоге приложений организации.|
|[Обновление опубликованного приложения](../api/teamsapp-update.md) | [teamsApp](teamsapp.md) | Обновление опубликованного приложения в каталоге приложений организации.|
|[Удаление опубликованного приложения](../api/teamsapp-delete.md) | Нет | Удаление опубликованного приложения из каталога приложений организации.|

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | строка   | Идентификатор приложения, созданного приложением каталога (отличается от идентификатора, предоставленного разработчиком, в [пакете приложения Microsoft Teams ZIP](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). |
| externalId          | string   | Идентификатор каталога, предоставленный разработчиком приложения в [пакете ZIP приложения Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). |
| displayName                | string   | Имя приложения каталога, предоставленное разработчиком приложения в [пакете ZIP приложения Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). |
| distributionMethod  | teamsAppDistributionMethod     | Способ распространения для приложения. |

### <a name="teamsappdistributionmethod-values"></a>значения teamsAppDistributionMethod

|Member|Значение|Описание|
|:---|:---|:---|
|восстановлен|нуль| Приложение доступно всем клиентам через магазин приложений Microsoft Teams.|
|organization;|1 |Приложение доступно только в этом клиенте.|
|неопубликованные|2 |Приложение доступно только для пользователя или группы, на которую он установлен.|

## <a name="relationships"></a>Связи

| Отношение | Тип   | Описание |
|:---------------|:--------|:----------|
|Аппдефинитионс|Коллекция [теамсаппдефинитион](teamsappdefinition.md)| Сведения о каждой версии приложения. |

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsApp",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "externalId": "string",
  "displayName": "Test App",
  "distributionMethod": "Organization"
}
```

# <a name="see-also"></a>См. также

- [teamsAppInstallation](teamsappinstallation.md)
- [Теамсаппдефинитион](teamsappdefinition.md)
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
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsapp.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

