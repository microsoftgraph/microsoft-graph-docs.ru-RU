---
title: тип ресурса assignedLabel
description: Представляет метку конфиденциальности, назначенную группе Microsoft 365.
localization_priority: Normal
author: jpettere
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 9602e10dda5d558110c55f1fb4ee166e53187989
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720895"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="7b973-103">тип ресурса assignedLabel</span><span class="sxs-lookup"><span data-stu-id="7b973-103">assignedLabel resource type</span></span>

<span data-ttu-id="7b973-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b973-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7b973-105">Представляет метку конфиденциальности, назначенную группе Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7b973-105">Represents a sensitivity label assigned to an Microsoft 365 group.</span></span> <span data-ttu-id="7b973-106">Метки конфиденциальности позволяют администраторам применять определенные групповые параметры в группе, назначая классификацию группе (например, конфиденциальность, высокая конфиденциальность или общие).</span><span class="sxs-lookup"><span data-stu-id="7b973-106">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="7b973-107">Метки конфиденциальности публикуются администраторами в Центре безопасности Microsoft 365 & соответствия требованиям в рамках возможностей Microsoft Information Protection.</span><span class="sxs-lookup"><span data-stu-id="7b973-107">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="7b973-108">Дополнительные сведения о метки конфиденциальности см. в обзоре [меток sensitivity.](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="7b973-108">For more information about sensitivity labels, see [Sensitivity labels overview](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide).</span></span>

## <a name="properties"></a><span data-ttu-id="7b973-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b973-109">Properties</span></span>
| <span data-ttu-id="7b973-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b973-110">Property</span></span>     | <span data-ttu-id="7b973-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7b973-111">Type</span></span>   |<span data-ttu-id="7b973-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7b973-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b973-113">labelId</span><span class="sxs-lookup"><span data-stu-id="7b973-113">labelId</span></span>|<span data-ttu-id="7b973-114">String</span><span class="sxs-lookup"><span data-stu-id="7b973-114">String</span></span>|<span data-ttu-id="7b973-115">Уникальный идентификатор метки.</span><span class="sxs-lookup"><span data-stu-id="7b973-115">The unique identifier of the label.</span></span>|
|<span data-ttu-id="7b973-116">displayName</span><span class="sxs-lookup"><span data-stu-id="7b973-116">displayName</span></span>|<span data-ttu-id="7b973-117">String</span><span class="sxs-lookup"><span data-stu-id="7b973-117">String</span></span>|<span data-ttu-id="7b973-118">Имя отображения метки.</span><span class="sxs-lookup"><span data-stu-id="7b973-118">The display name of the label.</span></span> <span data-ttu-id="7b973-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7b973-119">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b973-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7b973-120">JSON representation</span></span>

<span data-ttu-id="7b973-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b973-121">Here is a JSON representation of the resource.</span></span>

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