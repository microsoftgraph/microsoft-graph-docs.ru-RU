---
title: тип ресурса assignedLabel
description: Представляет метку конфиденциальности, назначенную Microsoft 365 группе.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: ea71e19388e8d9aa1bdf7f85c85ba6a85249233a
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680467"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="28cb4-103">тип ресурса assignedLabel</span><span class="sxs-lookup"><span data-stu-id="28cb4-103">assignedLabel resource type</span></span>

<span data-ttu-id="28cb4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28cb4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="28cb4-105">Представляет метку конфиденциальности, назначенную Microsoft 365 группе.</span><span class="sxs-lookup"><span data-stu-id="28cb4-105">Represents a sensitivity label assigned to an Microsoft 365 group.</span></span> <span data-ttu-id="28cb4-106">Метки конфиденциальности позволяют администраторам применять определенные групповые параметры в группе, назначая классификацию группе (например, конфиденциальность, высокая конфиденциальность или общие).</span><span class="sxs-lookup"><span data-stu-id="28cb4-106">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="28cb4-107">Метки конфиденциальности публикуются администраторами в центре Microsoft 365 безопасности & в рамках возможностей Microsoft Information Protection.</span><span class="sxs-lookup"><span data-stu-id="28cb4-107">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="28cb4-108">Дополнительные сведения о метки конфиденциальности см. в обзоре [меток sensitivity.](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="28cb4-108">For more information about sensitivity labels, see [Sensitivity labels overview](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide).</span></span>

## <a name="properties"></a><span data-ttu-id="28cb4-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="28cb4-109">Properties</span></span>
| <span data-ttu-id="28cb4-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="28cb4-110">Property</span></span>     | <span data-ttu-id="28cb4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="28cb4-111">Type</span></span>   |<span data-ttu-id="28cb4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="28cb4-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28cb4-113">labelId</span><span class="sxs-lookup"><span data-stu-id="28cb4-113">labelId</span></span>|<span data-ttu-id="28cb4-114">String</span><span class="sxs-lookup"><span data-stu-id="28cb4-114">String</span></span>|<span data-ttu-id="28cb4-115">Уникальный идентификатор метки.</span><span class="sxs-lookup"><span data-stu-id="28cb4-115">The unique identifier of the label.</span></span>|
|<span data-ttu-id="28cb4-116">displayName</span><span class="sxs-lookup"><span data-stu-id="28cb4-116">displayName</span></span>|<span data-ttu-id="28cb4-117">String</span><span class="sxs-lookup"><span data-stu-id="28cb4-117">String</span></span>|<span data-ttu-id="28cb4-118">Имя отображения метки.</span><span class="sxs-lookup"><span data-stu-id="28cb4-118">The display name of the label.</span></span> <span data-ttu-id="28cb4-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="28cb4-119">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="28cb4-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28cb4-120">JSON representation</span></span>

<span data-ttu-id="28cb4-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28cb4-121">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.assignedLabel"
}-->

```json
{
  "labelId": "String",
  "displayName": "String"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->