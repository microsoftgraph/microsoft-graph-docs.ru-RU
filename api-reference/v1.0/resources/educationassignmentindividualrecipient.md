---
title: тип ресурса educationAssignmentIndividualRecipient
description: Используется внутри свойства assignment.assignTo.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 147697685f58723d940102333abd9ffc378bee28
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912817"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a><span data-ttu-id="8dfbd-103">тип ресурса educationAssignmentIndividualRecipient</span><span class="sxs-lookup"><span data-stu-id="8dfbd-103">educationAssignmentIndividualRecipient resource type</span></span>

<span data-ttu-id="8dfbd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dfbd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8dfbd-105">Используется внутри [свойства assignment.assignTo.](educationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8dfbd-105">Used inside the [assignment.assignTo](educationassignment.md) property.</span></span> <span data-ttu-id="8dfbd-106">Если задан отдельный список получателей, выбранные учащиеся в классе получат объект отправки при публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="8dfbd-106">When set to individual recipient list, selected students in the class will receive a submission object when the assignment is published.</span></span>

<span data-ttu-id="8dfbd-107">Этот ресурс является подклассом [educationAssignmentRecipient](educationassignmentrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="8dfbd-107">This resource is a subclass of [educationAssignmentRecipient](educationassignmentrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8dfbd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8dfbd-108">Properties</span></span>
| <span data-ttu-id="8dfbd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8dfbd-109">Property</span></span>     | <span data-ttu-id="8dfbd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8dfbd-110">Type</span></span>   |<span data-ttu-id="8dfbd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8dfbd-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8dfbd-112">recipients</span><span class="sxs-lookup"><span data-stu-id="8dfbd-112">recipients</span></span>|<span data-ttu-id="8dfbd-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8dfbd-113">String collection</span></span>|<span data-ttu-id="8dfbd-114">Коллекция ID-адресов получателей.</span><span class="sxs-lookup"><span data-stu-id="8dfbd-114">A collection of IDs of the recipients.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8dfbd-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8dfbd-115">JSON representation</span></span>

<span data-ttu-id="8dfbd-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8dfbd-116">The following is a JSON representation of the resource.</span></span>

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


