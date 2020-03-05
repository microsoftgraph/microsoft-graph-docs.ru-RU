---
title: Тип ресурса Ассигнедлабел
description: Представляет метку конфиденциальности, назначенную группе Office 365. Метки конфиденциальности позволяют администраторам применять определенные параметры группы к группе, назначая классификацию группе (например, конфиденциальную, строго конфиденциальную или общую).
localization_priority: Normal
author: krbain
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 4f4f1fd854885668160b46f2b1ee9396dcf954fe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508221"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="77c6a-104">Тип ресурса Ассигнедлабел</span><span class="sxs-lookup"><span data-stu-id="77c6a-104">assignedLabel resource type</span></span>

<span data-ttu-id="77c6a-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="77c6a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77c6a-106">Представляет метку конфиденциальности, назначенную группе Office 365.</span><span class="sxs-lookup"><span data-stu-id="77c6a-106">Represents a sensitivity label assigned to an Office 365 group.</span></span> <span data-ttu-id="77c6a-107">Метки конфиденциальности позволяют администраторам применять определенные параметры группы к группе, назначая классификацию группе (например, конфиденциальную, строго конфиденциальную или общую).</span><span class="sxs-lookup"><span data-stu-id="77c6a-107">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="77c6a-108">Метки конфиденциальности публикуются администраторами в центре безопасности Microsoft 365 & соответствия требованиям в рамках возможностей защиты информации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="77c6a-108">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="77c6a-109">Дополнительные сведения о метках конфиденциальности приведены в разделе [Обзор меток конфиденциальности](/Office365/SecurityCompliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="77c6a-109">For more information about sensitivity labels, see [Sensitivity labels overview](/Office365/SecurityCompliance/sensitivity-labels).</span></span>

## <a name="properties"></a><span data-ttu-id="77c6a-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="77c6a-110">Properties</span></span>
| <span data-ttu-id="77c6a-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="77c6a-111">Property</span></span>     | <span data-ttu-id="77c6a-112">Тип</span><span class="sxs-lookup"><span data-stu-id="77c6a-112">Type</span></span>   |<span data-ttu-id="77c6a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="77c6a-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77c6a-114">лабелид</span><span class="sxs-lookup"><span data-stu-id="77c6a-114">labelId</span></span>|<span data-ttu-id="77c6a-115">String</span><span class="sxs-lookup"><span data-stu-id="77c6a-115">String</span></span>|<span data-ttu-id="77c6a-116">Уникальный идентификатор метки.</span><span class="sxs-lookup"><span data-stu-id="77c6a-116">The unique identifier of the label.</span></span>|
|<span data-ttu-id="77c6a-117">displayName</span><span class="sxs-lookup"><span data-stu-id="77c6a-117">displayName</span></span>|<span data-ttu-id="77c6a-118">String</span><span class="sxs-lookup"><span data-stu-id="77c6a-118">String</span></span>|<span data-ttu-id="77c6a-119">Отображаемое имя метки.</span><span class="sxs-lookup"><span data-stu-id="77c6a-119">The display name of the label.</span></span> <span data-ttu-id="77c6a-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77c6a-120">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77c6a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77c6a-121">JSON representation</span></span>

<span data-ttu-id="77c6a-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77c6a-122">Here is a JSON representation of the resource.</span></span>

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
