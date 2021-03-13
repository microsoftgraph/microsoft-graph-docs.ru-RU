---
title: тип ресурса assignedLabel
description: Представляет метку конфиденциальности, назначенную группе Microsoft 365. Метки конфиденциальности позволяют администраторам применять определенные групповые параметры в группе, назначая классификацию группе (например, конфиденциальность, высокая конфиденциальность или общие).
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: f22bfdd6cce307a83a90ada1da6a312994a3538e
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761249"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="57e7a-104">тип ресурса assignedLabel</span><span class="sxs-lookup"><span data-stu-id="57e7a-104">assignedLabel resource type</span></span>

<span data-ttu-id="57e7a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57e7a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57e7a-106">Представляет метку конфиденциальности, назначенную группе Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="57e7a-106">Represents a sensitivity label assigned to a Microsoft 365 group.</span></span> <span data-ttu-id="57e7a-107">Метки конфиденциальности позволяют администраторам применять определенные групповые параметры в группе, назначая классификацию группе (например, конфиденциальность, высокая конфиденциальность или общие).</span><span class="sxs-lookup"><span data-stu-id="57e7a-107">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="57e7a-108">Метки конфиденциальности публикуются администраторами в Центре безопасности Microsoft 365 & соответствия требованиям в рамках возможностей Microsoft Information Protection.</span><span class="sxs-lookup"><span data-stu-id="57e7a-108">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="57e7a-109">Дополнительные сведения о метки конфиденциальности см. в обзоре [меток sensitivity.](/Office365/SecurityCompliance/sensitivity-labels)</span><span class="sxs-lookup"><span data-stu-id="57e7a-109">For more information about sensitivity labels, see [Sensitivity labels overview](/Office365/SecurityCompliance/sensitivity-labels).</span></span>

## <a name="properties"></a><span data-ttu-id="57e7a-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="57e7a-110">Properties</span></span>
| <span data-ttu-id="57e7a-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="57e7a-111">Property</span></span>     | <span data-ttu-id="57e7a-112">Тип</span><span class="sxs-lookup"><span data-stu-id="57e7a-112">Type</span></span>   |<span data-ttu-id="57e7a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="57e7a-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57e7a-114">labelId</span><span class="sxs-lookup"><span data-stu-id="57e7a-114">labelId</span></span>|<span data-ttu-id="57e7a-115">String</span><span class="sxs-lookup"><span data-stu-id="57e7a-115">String</span></span>|<span data-ttu-id="57e7a-116">Уникальный идентификатор метки.</span><span class="sxs-lookup"><span data-stu-id="57e7a-116">The unique identifier of the label.</span></span>|
|<span data-ttu-id="57e7a-117">displayName</span><span class="sxs-lookup"><span data-stu-id="57e7a-117">displayName</span></span>|<span data-ttu-id="57e7a-118">String</span><span class="sxs-lookup"><span data-stu-id="57e7a-118">String</span></span>|<span data-ttu-id="57e7a-119">Имя отображения метки.</span><span class="sxs-lookup"><span data-stu-id="57e7a-119">The display name of the label.</span></span> <span data-ttu-id="57e7a-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57e7a-120">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57e7a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="57e7a-121">JSON representation</span></span>

<span data-ttu-id="57e7a-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57e7a-122">Here is a JSON representation of the resource.</span></span>

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


