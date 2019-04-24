---
title: Тип ресурса Синчронизатионжобрестарткритериа
description: 'Определяет область действия [синчронизатионжоб: Restart](../api/synchronization_synchronizationjob_restart.md) .'
localization_priority: Normal
ms.openlocfilehash: 1e6ac952808f80d191fc93e9a804411ec4459d4c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453618"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="d4f21-103">Тип ресурса Синчронизатионжобрестарткритериа</span><span class="sxs-lookup"><span data-stu-id="d4f21-103">synchronizationJobRestartCriteria resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4f21-104">Определяет область действия [синчронизатионжоб: Restart](../api/synchronization_synchronizationjob_restart.md) .</span><span class="sxs-lookup"><span data-stu-id="d4f21-104">Defines the scope of the [synchronizationJob: restart](../api/synchronization_synchronizationjob_restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="d4f21-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4f21-105">Properties</span></span>
| <span data-ttu-id="d4f21-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4f21-106">Property</span></span>     | <span data-ttu-id="d4f21-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d4f21-107">Type</span></span>   |<span data-ttu-id="d4f21-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d4f21-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4f21-109">Ресетскопе</span><span class="sxs-lookup"><span data-stu-id="d4f21-109">resetScope</span></span>|<span data-ttu-id="d4f21-110">Строка</span><span class="sxs-lookup"><span data-stu-id="d4f21-110">String</span></span>| <span data-ttu-id="d4f21-111">Разделенная заПятыми комбинация следующих значений: `Full`, `QuarantineState` `Watermark`,, `Escrows`, `ConnectorDataStore`.</span><span class="sxs-lookup"><span data-stu-id="d4f21-111">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="d4f21-112">Используйте `Full` , если вы хотите использовать все параметры.</span><span class="sxs-lookup"><span data-stu-id="d4f21-112">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4f21-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4f21-113">JSON representation</span></span>

<span data-ttu-id="d4f21-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4f21-114">The following is a JSON representation of the resource.</span></span>

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
