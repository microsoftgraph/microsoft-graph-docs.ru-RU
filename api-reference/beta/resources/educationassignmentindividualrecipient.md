---
title: Тип ресурса ЕдукатионассигнментиндивидуалреЦипиент
description: 'Используется внутри свойства назначение. Ассигнто. Если задан отдельный список получателей, выбранные студенты в классе будут '
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 736345901faeeb4d3fab4d417752b684f1e19307
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543016"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a><span data-ttu-id="7d9a3-104">Тип ресурса ЕдукатионассигнментиндивидуалреЦипиент</span><span class="sxs-lookup"><span data-stu-id="7d9a3-104">educationAssignmentIndividualRecipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d9a3-105">Используется внутри свойства [назначение. ассигнто](educationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="7d9a3-105">Used inside the [assignment.assignTo](educationassignment.md) property.</span></span> <span data-ttu-id="7d9a3-106">Если задан отдельный список получателей, выбранные студенты в классе получат объект отправки при публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="7d9a3-106">When set to individual recipient list, selected students in the class will receive a submission object when the assignment is published.</span></span>

<span data-ttu-id="7d9a3-107">Этот ресурс является подклассом [едукатионассигнментреЦипиент](educationassignmentrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="7d9a3-107">This resource is a subclass of [educationAssignmentRecipient](educationassignmentrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7d9a3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d9a3-108">Properties</span></span>
| <span data-ttu-id="7d9a3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d9a3-109">Property</span></span>     | <span data-ttu-id="7d9a3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7d9a3-110">Type</span></span>   |<span data-ttu-id="7d9a3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7d9a3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d9a3-112">recipients</span><span class="sxs-lookup"><span data-stu-id="7d9a3-112">recipients</span></span>|<span data-ttu-id="7d9a3-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7d9a3-113">String collection</span></span>|<span data-ttu-id="7d9a3-114">Коллекция идентификаторов получателей.</span><span class="sxs-lookup"><span data-stu-id="7d9a3-114">A collection of ids of the recipients.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d9a3-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7d9a3-115">JSON representation</span></span>

<span data-ttu-id="7d9a3-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d9a3-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentIndividualRecipient"
}-->

```json
{
  "recipients": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentindividualrecipient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
