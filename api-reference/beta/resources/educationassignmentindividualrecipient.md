---
title: Тип ресурса ЕдукатионассигнментиндивидуалреЦипиент
description: 'Используется внутри свойства назначение. Ассигнто. Если задан отдельный список получателей, выбранные студенты в классе будут '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7408382cadcb53d857bb36b06702f7857d64a8f4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006453"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a><span data-ttu-id="2aef2-104">Тип ресурса ЕдукатионассигнментиндивидуалреЦипиент</span><span class="sxs-lookup"><span data-stu-id="2aef2-104">educationAssignmentIndividualRecipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2aef2-105">Используется внутри свойства [назначение. ассигнто](educationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="2aef2-105">Used inside the [assignment.assignTo](educationassignment.md) property.</span></span> <span data-ttu-id="2aef2-106">Если задан отдельный список получателей, выбранные студенты в классе получат объект отправки при публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="2aef2-106">When set to individual recipient list, selected students in the class will receive a submission object when the assignment is published.</span></span>

<span data-ttu-id="2aef2-107">Этот ресурс является подклассом [едукатионассигнментреЦипиент](educationassignmentrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="2aef2-107">This resource is a subclass of [educationAssignmentRecipient](educationassignmentrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2aef2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2aef2-108">Properties</span></span>
| <span data-ttu-id="2aef2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2aef2-109">Property</span></span>     | <span data-ttu-id="2aef2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2aef2-110">Type</span></span>   |<span data-ttu-id="2aef2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2aef2-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2aef2-112">recipients</span><span class="sxs-lookup"><span data-stu-id="2aef2-112">recipients</span></span>|<span data-ttu-id="2aef2-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2aef2-113">String collection</span></span>|<span data-ttu-id="2aef2-114">Коллекция идентификаторов получателей.</span><span class="sxs-lookup"><span data-stu-id="2aef2-114">A collection of ids of the recipients.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2aef2-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2aef2-115">JSON representation</span></span>

<span data-ttu-id="2aef2-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2aef2-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
