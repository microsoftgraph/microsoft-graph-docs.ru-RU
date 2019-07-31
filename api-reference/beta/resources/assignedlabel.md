---
title: Тип ресурса Ассигнедлабел
description: Представляет метку конфиденциальности, назначенную группе Office 365. Метки конфиденциальности позволяют администраторам применять определенные параметры группы к группе, назначая классификацию группе (например, конфиденциальную, строго конфиденциальную или общую).
localization_priority: Normal
author: krbain
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 118a8a85a8abb68f59438db9024952d16f7a279c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013292"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="6a834-104">Тип ресурса Ассигнедлабел</span><span class="sxs-lookup"><span data-stu-id="6a834-104">assignedLabel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a834-105">Представляет метку конфиденциальности, назначенную группе Office 365.</span><span class="sxs-lookup"><span data-stu-id="6a834-105">Represents a sensitivity label assigned to an Office 365 group.</span></span> <span data-ttu-id="6a834-106">Метки конфиденциальности позволяют администраторам применять определенные параметры группы к группе, назначая классификацию группе (например, конфиденциальную, строго конфиденциальную или общую).</span><span class="sxs-lookup"><span data-stu-id="6a834-106">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="6a834-107">Метки конфиденциальности публикуются администраторами в центре безопасности Microsoft 365 & соответствия требованиям в рамках возможностей защиты информации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="6a834-107">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="6a834-108">Дополнительные сведения о метках конфиденциальности приведены в разделе [Обзор меток конфиденциальности](https://docs.microsoft.com/en-us/Office365/SecurityCompliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="6a834-108">For more information about sensitivity labels, see [Sensitivity labels overview](https://docs.microsoft.com/en-us/Office365/SecurityCompliance/sensitivity-labels).</span></span>

## <a name="properties"></a><span data-ttu-id="6a834-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a834-109">Properties</span></span>
| <span data-ttu-id="6a834-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a834-110">Property</span></span>     | <span data-ttu-id="6a834-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6a834-111">Type</span></span>   |<span data-ttu-id="6a834-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6a834-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a834-113">Лабелид</span><span class="sxs-lookup"><span data-stu-id="6a834-113">labelId</span></span>|<span data-ttu-id="6a834-114">String</span><span class="sxs-lookup"><span data-stu-id="6a834-114">String</span></span>|<span data-ttu-id="6a834-115">Уникальный идентификатор метки.</span><span class="sxs-lookup"><span data-stu-id="6a834-115">The unique identifier of the label.</span></span>|
|<span data-ttu-id="6a834-116">displayName</span><span class="sxs-lookup"><span data-stu-id="6a834-116">displayName</span></span>|<span data-ttu-id="6a834-117">String</span><span class="sxs-lookup"><span data-stu-id="6a834-117">String</span></span>|<span data-ttu-id="6a834-118">Отображаемое имя метки.</span><span class="sxs-lookup"><span data-stu-id="6a834-118">The display name of the label.</span></span> <span data-ttu-id="6a834-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6a834-119">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6a834-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a834-120">JSON representation</span></span>

<span data-ttu-id="6a834-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a834-121">Here is a JSON representation of the resource.</span></span>

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
