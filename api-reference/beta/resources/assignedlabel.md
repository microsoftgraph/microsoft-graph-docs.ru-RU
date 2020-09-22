---
title: Тип ресурса Ассигнедлабел
description: Представляет метку конфиденциальности, назначенную группе Microsoft 365. Метки конфиденциальности позволяют администраторам применять определенные параметры группы к группе, назначая классификацию группе (например, конфиденциальную, строго конфиденциальную или общую).
localization_priority: Normal
author: krbain
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 8ef079363d4951f269ea509534cecd2e6ae2a0f9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050108"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="69c20-104">Тип ресурса Ассигнедлабел</span><span class="sxs-lookup"><span data-stu-id="69c20-104">assignedLabel resource type</span></span>

<span data-ttu-id="69c20-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69c20-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69c20-106">Представляет метку конфиденциальности, назначенную группе Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="69c20-106">Represents a sensitivity label assigned to a Microsoft 365 group.</span></span> <span data-ttu-id="69c20-107">Метки конфиденциальности позволяют администраторам применять определенные параметры группы к группе, назначая классификацию группе (например, конфиденциальную, строго конфиденциальную или общую).</span><span class="sxs-lookup"><span data-stu-id="69c20-107">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="69c20-108">Метки конфиденциальности публикуются администраторами в центре безопасности Microsoft 365 & соответствия требованиям в рамках возможностей защиты информации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="69c20-108">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="69c20-109">Дополнительные сведения о метках конфиденциальности приведены в разделе [Обзор меток конфиденциальности](/Office365/SecurityCompliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="69c20-109">For more information about sensitivity labels, see [Sensitivity labels overview](/Office365/SecurityCompliance/sensitivity-labels).</span></span>

## <a name="properties"></a><span data-ttu-id="69c20-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="69c20-110">Properties</span></span>
| <span data-ttu-id="69c20-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="69c20-111">Property</span></span>     | <span data-ttu-id="69c20-112">Тип</span><span class="sxs-lookup"><span data-stu-id="69c20-112">Type</span></span>   |<span data-ttu-id="69c20-113">Описание</span><span class="sxs-lookup"><span data-stu-id="69c20-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69c20-114">лабелид</span><span class="sxs-lookup"><span data-stu-id="69c20-114">labelId</span></span>|<span data-ttu-id="69c20-115">Строка</span><span class="sxs-lookup"><span data-stu-id="69c20-115">String</span></span>|<span data-ttu-id="69c20-116">Уникальный идентификатор метки.</span><span class="sxs-lookup"><span data-stu-id="69c20-116">The unique identifier of the label.</span></span>|
|<span data-ttu-id="69c20-117">displayName</span><span class="sxs-lookup"><span data-stu-id="69c20-117">displayName</span></span>|<span data-ttu-id="69c20-118">Строка</span><span class="sxs-lookup"><span data-stu-id="69c20-118">String</span></span>|<span data-ttu-id="69c20-119">Отображаемое имя метки.</span><span class="sxs-lookup"><span data-stu-id="69c20-119">The display name of the label.</span></span> <span data-ttu-id="69c20-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69c20-120">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69c20-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69c20-121">JSON representation</span></span>

<span data-ttu-id="69c20-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69c20-122">Here is a JSON representation of the resource.</span></span>

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


