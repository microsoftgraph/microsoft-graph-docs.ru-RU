---
title: Тип ресурса ЕдукатионассигнментиндивидуалреЦипиент
description: 'Используется внутри свойства назначение. Ассигнто. Если задан отдельный список получателей, выбранные студенты в классе будут '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b5bccdf98bbba4c0965daf5d5aba93cf1a34b758
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502559"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a><span data-ttu-id="411c2-104">Тип ресурса ЕдукатионассигнментиндивидуалреЦипиент</span><span class="sxs-lookup"><span data-stu-id="411c2-104">educationAssignmentIndividualRecipient resource type</span></span>

<span data-ttu-id="411c2-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="411c2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="411c2-106">Используется внутри свойства [назначение. ассигнто](educationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="411c2-106">Used inside the [assignment.assignTo](educationassignment.md) property.</span></span> <span data-ttu-id="411c2-107">Если задан отдельный список получателей, выбранные студенты в классе получат объект отправки при публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="411c2-107">When set to individual recipient list, selected students in the class will receive a submission object when the assignment is published.</span></span>

<span data-ttu-id="411c2-108">Этот ресурс является подклассом [едукатионассигнментреЦипиент](educationassignmentrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="411c2-108">This resource is a subclass of [educationAssignmentRecipient](educationassignmentrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="411c2-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="411c2-109">Properties</span></span>
| <span data-ttu-id="411c2-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="411c2-110">Property</span></span>     | <span data-ttu-id="411c2-111">Тип</span><span class="sxs-lookup"><span data-stu-id="411c2-111">Type</span></span>   |<span data-ttu-id="411c2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="411c2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="411c2-113">recipients</span><span class="sxs-lookup"><span data-stu-id="411c2-113">recipients</span></span>|<span data-ttu-id="411c2-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="411c2-114">String collection</span></span>|<span data-ttu-id="411c2-115">Коллекция идентификаторов получателей.</span><span class="sxs-lookup"><span data-stu-id="411c2-115">A collection of ids of the recipients.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="411c2-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="411c2-116">JSON representation</span></span>

<span data-ttu-id="411c2-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="411c2-117">The following is a JSON representation of the resource.</span></span>

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
