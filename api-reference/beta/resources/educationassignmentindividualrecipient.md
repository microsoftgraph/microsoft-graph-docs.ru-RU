---
title: Тип ресурса ЕдукатионассигнментиндивидуалреЦипиент
description: 'Используется внутри свойства назначение. Ассигнто. Если задан отдельный список получателей, выбранные студенты в классе будут '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 695145ae8819efc66df29d752e7a95101c9fef9e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013723"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a><span data-ttu-id="c3e21-104">Тип ресурса ЕдукатионассигнментиндивидуалреЦипиент</span><span class="sxs-lookup"><span data-stu-id="c3e21-104">educationAssignmentIndividualRecipient resource type</span></span>

<span data-ttu-id="c3e21-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3e21-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3e21-106">Используется внутри свойства [назначение. ассигнто](educationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c3e21-106">Used inside the [assignment.assignTo](educationassignment.md) property.</span></span> <span data-ttu-id="c3e21-107">Если задан отдельный список получателей, выбранные студенты в классе получат объект отправки при публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="c3e21-107">When set to individual recipient list, selected students in the class will receive a submission object when the assignment is published.</span></span>

<span data-ttu-id="c3e21-108">Этот ресурс является подклассом [едукатионассигнментреЦипиент](educationassignmentrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="c3e21-108">This resource is a subclass of [educationAssignmentRecipient](educationassignmentrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c3e21-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3e21-109">Properties</span></span>
| <span data-ttu-id="c3e21-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3e21-110">Property</span></span>     | <span data-ttu-id="c3e21-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c3e21-111">Type</span></span>   |<span data-ttu-id="c3e21-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c3e21-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3e21-113">recipients</span><span class="sxs-lookup"><span data-stu-id="c3e21-113">recipients</span></span>|<span data-ttu-id="c3e21-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c3e21-114">String collection</span></span>|<span data-ttu-id="c3e21-115">Коллекция идентификаторов получателей.</span><span class="sxs-lookup"><span data-stu-id="c3e21-115">A collection of ids of the recipients.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3e21-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3e21-116">JSON representation</span></span>

<span data-ttu-id="c3e21-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3e21-117">The following is a JSON representation of the resource.</span></span>

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


