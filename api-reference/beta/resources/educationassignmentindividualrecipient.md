---
title: Тип ресурса ЕдукатионассигнментиндивидуалреЦипиент
description: 'Используется внутри свойства назначение. Ассигнто. Если задан отдельный список получателей, выбранные студенты в классе будут '
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 736345901faeeb4d3fab4d417752b684f1e19307
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/26/2019
ms.locfileid: "30799993"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a><span data-ttu-id="edb5b-104">Тип ресурса ЕдукатионассигнментиндивидуалреЦипиент</span><span class="sxs-lookup"><span data-stu-id="edb5b-104">educationAssignmentIndividualRecipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edb5b-105">Используется внутри свойства [назначение. ассигнто](educationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="edb5b-105">Used inside the [assignment.assignTo](educationassignment.md) property.</span></span> <span data-ttu-id="edb5b-106">Если задан отдельный список получателей, выбранные студенты в классе получат объект отправки при публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="edb5b-106">When set to individual recipient list, selected students in the class will receive a submission object when the assignment is published.</span></span>

<span data-ttu-id="edb5b-107">Этот ресурс является подклассом [едукатионассигнментреЦипиент](educationassignmentrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="edb5b-107">This resource is a subclass of [educationAssignmentRecipient](educationassignmentrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="edb5b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="edb5b-108">Properties</span></span>
| <span data-ttu-id="edb5b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="edb5b-109">Property</span></span>     | <span data-ttu-id="edb5b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="edb5b-110">Type</span></span>   |<span data-ttu-id="edb5b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="edb5b-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edb5b-112">recipients</span><span class="sxs-lookup"><span data-stu-id="edb5b-112">recipients</span></span>|<span data-ttu-id="edb5b-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="edb5b-113">String collection</span></span>|<span data-ttu-id="edb5b-114">Коллекция идентификаторов получателей.</span><span class="sxs-lookup"><span data-stu-id="edb5b-114">A collection of ids of the recipients.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="edb5b-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="edb5b-115">JSON representation</span></span>

<span data-ttu-id="edb5b-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edb5b-116">The following is a JSON representation of the resource.</span></span>

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
