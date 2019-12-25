---
title: Тип ресурса Ассигнедлабел
description: Представляет метку конфиденциальности, назначенную группе Office 365. Метки конфиденциальности позволяют администраторам применять определенные параметры группы к группе, назначая классификацию группе (например, конфиденциальную, строго конфиденциальную или общую).
localization_priority: Normal
author: krbain
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 7e8390ec1773061d447e7526f55e67b87e51531b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870941"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="8594b-104">Тип ресурса Ассигнедлабел</span><span class="sxs-lookup"><span data-stu-id="8594b-104">assignedLabel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8594b-105">Представляет метку конфиденциальности, назначенную группе Office 365.</span><span class="sxs-lookup"><span data-stu-id="8594b-105">Represents a sensitivity label assigned to an Office 365 group.</span></span> <span data-ttu-id="8594b-106">Метки конфиденциальности позволяют администраторам применять определенные параметры группы к группе, назначая классификацию группе (например, конфиденциальную, строго конфиденциальную или общую).</span><span class="sxs-lookup"><span data-stu-id="8594b-106">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="8594b-107">Метки конфиденциальности публикуются администраторами в центре безопасности Microsoft 365 & соответствия требованиям в рамках возможностей защиты информации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="8594b-107">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="8594b-108">Дополнительные сведения о метках конфиденциальности приведены в разделе [Обзор меток конфиденциальности](/Office365/SecurityCompliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="8594b-108">For more information about sensitivity labels, see [Sensitivity labels overview](/Office365/SecurityCompliance/sensitivity-labels).</span></span>

## <a name="properties"></a><span data-ttu-id="8594b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8594b-109">Properties</span></span>
| <span data-ttu-id="8594b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8594b-110">Property</span></span>     | <span data-ttu-id="8594b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8594b-111">Type</span></span>   |<span data-ttu-id="8594b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8594b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8594b-113">лабелид</span><span class="sxs-lookup"><span data-stu-id="8594b-113">labelId</span></span>|<span data-ttu-id="8594b-114">String</span><span class="sxs-lookup"><span data-stu-id="8594b-114">String</span></span>|<span data-ttu-id="8594b-115">Уникальный идентификатор метки.</span><span class="sxs-lookup"><span data-stu-id="8594b-115">The unique identifier of the label.</span></span>|
|<span data-ttu-id="8594b-116">displayName</span><span class="sxs-lookup"><span data-stu-id="8594b-116">displayName</span></span>|<span data-ttu-id="8594b-117">String</span><span class="sxs-lookup"><span data-stu-id="8594b-117">String</span></span>|<span data-ttu-id="8594b-118">Отображаемое имя метки.</span><span class="sxs-lookup"><span data-stu-id="8594b-118">The display name of the label.</span></span> <span data-ttu-id="8594b-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8594b-119">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8594b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8594b-120">JSON representation</span></span>

<span data-ttu-id="8594b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8594b-121">Here is a JSON representation of the resource.</span></span>

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
