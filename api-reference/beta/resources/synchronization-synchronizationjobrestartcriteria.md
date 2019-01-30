---
title: Тип ресурса synchronizationJobRestartCriteria
description: 'Определяет область [synchronizationJob: перезапустите](../api/synchronization_synchronizationjob_restart.md) действие.'
localization_priority: Normal
ms.openlocfilehash: 1e6ac952808f80d191fc93e9a804411ec4459d4c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642522"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="80f9a-103">Тип ресурса synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="80f9a-103">synchronizationJobRestartCriteria resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80f9a-104">Определяет область [synchronizationJob: перезапустите](../api/synchronization_synchronizationjob_restart.md) действие.</span><span class="sxs-lookup"><span data-stu-id="80f9a-104">Defines the scope of the [synchronizationJob: restart](../api/synchronization_synchronizationjob_restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="80f9a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="80f9a-105">Properties</span></span>
| <span data-ttu-id="80f9a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="80f9a-106">Property</span></span>     | <span data-ttu-id="80f9a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="80f9a-107">Type</span></span>   |<span data-ttu-id="80f9a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="80f9a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80f9a-109">resetScope</span><span class="sxs-lookup"><span data-stu-id="80f9a-109">resetScope</span></span>|<span data-ttu-id="80f9a-110">String</span><span class="sxs-lookup"><span data-stu-id="80f9a-110">String</span></span>| <span data-ttu-id="80f9a-111">Разделенный запятыми сочетание следующих значений: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span><span class="sxs-lookup"><span data-stu-id="80f9a-111">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="80f9a-112">Использование `Full` Если вы хотите, чтобы все параметры.</span><span class="sxs-lookup"><span data-stu-id="80f9a-112">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="80f9a-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="80f9a-113">JSON representation</span></span>

<span data-ttu-id="80f9a-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80f9a-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
  "resetScope": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationjobrestartcriteria.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
