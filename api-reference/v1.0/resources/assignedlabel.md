---
title: Тип ресурса Ассигнедлабел
description: Представляет метку конфиденциальности, назначенную группе Microsoft 365.
localization_priority: Normal
author: krbain
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: b3c226624e850d0d1a5bb2e3866246ecaee9d832
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003313"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="12288-103">Тип ресурса Ассигнедлабел</span><span class="sxs-lookup"><span data-stu-id="12288-103">assignedLabel resource type</span></span>

<span data-ttu-id="12288-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12288-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="12288-105">Представляет метку конфиденциальности, назначенную группе Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="12288-105">Represents a sensitivity label assigned to an Microsoft 365 group.</span></span> <span data-ttu-id="12288-106">Метки конфиденциальности позволяют администраторам применять определенные параметры группы к группе, назначая классификацию группе (например, конфиденциальную, строго конфиденциальную или общую).</span><span class="sxs-lookup"><span data-stu-id="12288-106">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="12288-107">Метки конфиденциальности публикуются администраторами в центре безопасности Microsoft 365 & соответствия требованиям в рамках возможностей защиты информации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="12288-107">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="12288-108">Дополнительные сведения о метках конфиденциальности приведены в разделе [Обзор меток конфиденциальности](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="12288-108">For more information about sensitivity labels, see [Sensitivity labels overview](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide).</span></span>

## <a name="properties"></a><span data-ttu-id="12288-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="12288-109">Properties</span></span>
| <span data-ttu-id="12288-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="12288-110">Property</span></span>     | <span data-ttu-id="12288-111">Тип</span><span class="sxs-lookup"><span data-stu-id="12288-111">Type</span></span>   |<span data-ttu-id="12288-112">Описание</span><span class="sxs-lookup"><span data-stu-id="12288-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12288-113">лабелид</span><span class="sxs-lookup"><span data-stu-id="12288-113">labelId</span></span>|<span data-ttu-id="12288-114">String</span><span class="sxs-lookup"><span data-stu-id="12288-114">String</span></span>|<span data-ttu-id="12288-115">Уникальный идентификатор метки.</span><span class="sxs-lookup"><span data-stu-id="12288-115">The unique identifier of the label.</span></span>|
|<span data-ttu-id="12288-116">displayName</span><span class="sxs-lookup"><span data-stu-id="12288-116">displayName</span></span>|<span data-ttu-id="12288-117">String</span><span class="sxs-lookup"><span data-stu-id="12288-117">String</span></span>|<span data-ttu-id="12288-118">Отображаемое имя метки.</span><span class="sxs-lookup"><span data-stu-id="12288-118">The display name of the label.</span></span> <span data-ttu-id="12288-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12288-119">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12288-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="12288-120">JSON representation</span></span>

<span data-ttu-id="12288-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12288-121">Here is a JSON representation of the resource.</span></span>

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
