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
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="4b550-103">Тип ресурса Едукатионксвдатапровидер</span><span class="sxs-lookup"><span data-stu-id="4b550-103">educationCsvDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b550-104">Используется для настройки профиля синхронизации данных School, когда CSV-файлы являются источником входных данных.</span><span class="sxs-lookup"><span data-stu-id="4b550-104">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="4b550-105">Производный от [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="4b550-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4b550-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b550-106">Properties</span></span>

| <span data-ttu-id="4b550-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b550-107">Property</span></span> | <span data-ttu-id="4b550-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4b550-108">Type</span></span> | <span data-ttu-id="4b550-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4b550-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="4b550-110">**настроек**</span><span class="sxs-lookup"><span data-stu-id="4b550-110">**customizations**</span></span> | [<span data-ttu-id="4b550-111">Едукатионсинчронизатионкустомизатионс</span><span class="sxs-lookup"><span data-stu-id="4b550-111">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="4b550-112">НеОбязательные настройки, которые необходимо применить к профилю синхронизации.</span><span class="sxs-lookup"><span data-stu-id="4b550-112">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b550-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b550-113">JSON representation</span></span>

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
