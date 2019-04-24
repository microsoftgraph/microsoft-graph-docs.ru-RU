---
title: Тип ресурса Едукатионксвдатапровидер
description: 'Используется для настройки профиля синхронизации данных School, когда CSV-файлы являются источником входных данных.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bebacbc1c618c7558d81bde2611840e8d225a8fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507182"
---
# <a name="educationcsvdataprovider-resource-type"></a>Тип ресурса Едукатионксвдатапровидер

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для настройки профиля синхронизации данных School, когда CSV-файлы являются источником входных данных.  

Производный от [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **настроек** | [Едукатионсинчронизатионкустомизатионс](educationsynchronizationcustomizations.md) | НеОбязательные настройки, которые необходимо применить к профилю синхронизации.|

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationcsvdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
