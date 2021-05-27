---
title: тип ресурса assignedLabel
description: Представляет метку конфиденциальности, назначенную Microsoft 365 группе. Метки конфиденциальности позволяют администраторам применять определенные групповые параметры в группе, назначая классификацию группе (например, конфиденциальность, высокая конфиденциальность или общие).
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: b54236376979d064a86eb1e4852919e2b5ff9e49
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680460"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="1fd4b-104">тип ресурса assignedLabel</span><span class="sxs-lookup"><span data-stu-id="1fd4b-104">assignedLabel resource type</span></span>

<span data-ttu-id="1fd4b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fd4b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fd4b-106">Представляет метку конфиденциальности, назначенную Microsoft 365 группе.</span><span class="sxs-lookup"><span data-stu-id="1fd4b-106">Represents a sensitivity label assigned to a Microsoft 365 group.</span></span> <span data-ttu-id="1fd4b-107">Метки конфиденциальности позволяют администраторам применять определенные групповые параметры в группе, назначая классификацию группе (например, конфиденциальность, высокая конфиденциальность или общие).</span><span class="sxs-lookup"><span data-stu-id="1fd4b-107">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="1fd4b-108">Метки конфиденциальности публикуются администраторами в центре Microsoft 365 безопасности & в рамках возможностей Microsoft Information Protection.</span><span class="sxs-lookup"><span data-stu-id="1fd4b-108">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="1fd4b-109">Дополнительные сведения о метки конфиденциальности см. в обзоре [меток sensitivity.](/Office365/SecurityCompliance/sensitivity-labels)</span><span class="sxs-lookup"><span data-stu-id="1fd4b-109">For more information about sensitivity labels, see [Sensitivity labels overview](/Office365/SecurityCompliance/sensitivity-labels).</span></span>

## <a name="properties"></a><span data-ttu-id="1fd4b-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="1fd4b-110">Properties</span></span>
| <span data-ttu-id="1fd4b-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="1fd4b-111">Property</span></span>     | <span data-ttu-id="1fd4b-112">Тип</span><span class="sxs-lookup"><span data-stu-id="1fd4b-112">Type</span></span>   |<span data-ttu-id="1fd4b-113">Описание</span><span class="sxs-lookup"><span data-stu-id="1fd4b-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1fd4b-114">labelId</span><span class="sxs-lookup"><span data-stu-id="1fd4b-114">labelId</span></span>|<span data-ttu-id="1fd4b-115">String</span><span class="sxs-lookup"><span data-stu-id="1fd4b-115">String</span></span>|<span data-ttu-id="1fd4b-116">Уникальный идентификатор метки.</span><span class="sxs-lookup"><span data-stu-id="1fd4b-116">The unique identifier of the label.</span></span>|
|<span data-ttu-id="1fd4b-117">displayName</span><span class="sxs-lookup"><span data-stu-id="1fd4b-117">displayName</span></span>|<span data-ttu-id="1fd4b-118">String</span><span class="sxs-lookup"><span data-stu-id="1fd4b-118">String</span></span>|<span data-ttu-id="1fd4b-119">Имя отображения метки.</span><span class="sxs-lookup"><span data-stu-id="1fd4b-119">The display name of the label.</span></span> <span data-ttu-id="1fd4b-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1fd4b-120">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1fd4b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1fd4b-121">JSON representation</span></span>

<span data-ttu-id="1fd4b-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1fd4b-122">Here is a JSON representation of the resource.</span></span>

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


