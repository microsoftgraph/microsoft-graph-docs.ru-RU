---
title: Тип ресурса educationCsvDataProvider
description: 'Используется для настройки синхронизации профилей данных school после ввода источника файлов CSV.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bebacbc1c618c7558d81bde2611840e8d225a8fd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529875"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="fcf18-103">Тип ресурса educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="fcf18-103">educationCsvDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcf18-104">Используется для настройки синхронизации профилей данных school после ввода источника файлов CSV.</span><span class="sxs-lookup"><span data-stu-id="fcf18-104">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="fcf18-105">На основе [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="fcf18-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fcf18-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fcf18-106">Properties</span></span>

| <span data-ttu-id="fcf18-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcf18-107">Property</span></span> | <span data-ttu-id="fcf18-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fcf18-108">Type</span></span> | <span data-ttu-id="fcf18-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fcf18-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="fcf18-110">**пользовательских настроек**</span><span class="sxs-lookup"><span data-stu-id="fcf18-110">**customizations**</span></span> | [<span data-ttu-id="fcf18-111">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="fcf18-111">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="fcf18-112">Необязательный настроек применяется для синхронизации профилей.</span><span class="sxs-lookup"><span data-stu-id="fcf18-112">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fcf18-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fcf18-113">JSON representation</span></span>

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
