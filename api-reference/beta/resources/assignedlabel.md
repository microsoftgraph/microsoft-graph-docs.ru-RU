---
title: Тип ресурса Ассигнедлабел
description: Представляет метку конфиденциальности, назначенную группе Office 365. Метки конфиденциальности позволяют администраторам применять определенные параметры группы к группе, назначая классификацию группе (например, конфиденциальную, строго конфиденциальную или общую).
localization_priority: Normal
author: krbain
ms.prod: groups
ms.openlocfilehash: 430387f228bf632a7f9f9b4a046537bbe5ff4953
ms.sourcegitcommit: b18ccb24fc79f3abb470cd759e25cdd266fc77c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/17/2019
ms.locfileid: "34117690"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="2d8de-104">Тип ресурса Ассигнедлабел</span><span class="sxs-lookup"><span data-stu-id="2d8de-104">assignedLabel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d8de-105">Представляет метку конфиденциальности, назначенную группе Office 365.</span><span class="sxs-lookup"><span data-stu-id="2d8de-105">Represents a sensitivity label assigned to an Office 365 group.</span></span> <span data-ttu-id="2d8de-106">Метки конфиденциальности позволяют администраторам применять определенные параметры группы к группе, назначая классификацию группе (например, конфиденциальную, строго конфиденциальную или общую).</span><span class="sxs-lookup"><span data-stu-id="2d8de-106">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="2d8de-107">Метки конфиденциальности публикуются администраторами в центре безопасности Microsoft 365 Security _Амп_ в рамках возможностей защиты информации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="2d8de-107">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="2d8de-108">Дополнительные сведения о метках конфиденциальности приведены в разделе [Обзор меток конфиденциальности](https://docs.microsoft.com/en-us/Office365/SecurityCompliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="2d8de-108">For more information about sensitivity labels, see [Sensitivity labels overview](https://docs.microsoft.com/en-us/Office365/SecurityCompliance/sensitivity-labels).</span></span>

## <a name="properties"></a><span data-ttu-id="2d8de-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d8de-109">Properties</span></span>
| <span data-ttu-id="2d8de-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d8de-110">Property</span></span>     | <span data-ttu-id="2d8de-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2d8de-111">Type</span></span>   |<span data-ttu-id="2d8de-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2d8de-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d8de-113">Лабелид</span><span class="sxs-lookup"><span data-stu-id="2d8de-113">labelId</span></span>|<span data-ttu-id="2d8de-114">String</span><span class="sxs-lookup"><span data-stu-id="2d8de-114">String</span></span>|<span data-ttu-id="2d8de-115">Уникальный идентификатор метки.</span><span class="sxs-lookup"><span data-stu-id="2d8de-115">The unique identifier of the label.</span></span>|
|<span data-ttu-id="2d8de-116">displayName</span><span class="sxs-lookup"><span data-stu-id="2d8de-116">displayName</span></span>|<span data-ttu-id="2d8de-117">String</span><span class="sxs-lookup"><span data-stu-id="2d8de-117">String</span></span>|<span data-ttu-id="2d8de-118">Отображаемое имя метки.</span><span class="sxs-lookup"><span data-stu-id="2d8de-118">The display name of the label.</span></span> <span data-ttu-id="2d8de-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2d8de-119">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d8de-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d8de-120">JSON representation</span></span>

<span data-ttu-id="2d8de-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d8de-121">Here is a JSON representation of the resource.</span></span>

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
