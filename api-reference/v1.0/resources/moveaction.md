---
author: daspek
ms.author: dspektor
title: Тип ресурса moveAction
description: Объект MoveAction предоставляет сведения о действии, которое переместит элемент.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ec1ac8ccaae502f66e205571e17eb5ad3eced8e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020533"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="7b85c-103">Тип ресурса moveAction</span><span class="sxs-lookup"><span data-stu-id="7b85c-103">moveAction resource type</span></span>

<span data-ttu-id="7b85c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b85c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7b85c-105">Присутствие ресурса **moveAction** в [**itemActivity**][activity] указывает на то, что действие переместило элемент.</span><span class="sxs-lookup"><span data-stu-id="7b85c-105">The presence of the **moveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

><span data-ttu-id="7b85c-106">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="7b85c-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="7b85c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b85c-107">Properties</span></span>

| <span data-ttu-id="7b85c-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7b85c-108">Property name</span></span> | <span data-ttu-id="7b85c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7b85c-109">Type</span></span>   | <span data-ttu-id="7b85c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7b85c-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="7b85c-111">from</span><span class="sxs-lookup"><span data-stu-id="7b85c-111">from</span></span>          | <span data-ttu-id="7b85c-112">string</span><span class="sxs-lookup"><span data-stu-id="7b85c-112">string</span></span> | <span data-ttu-id="7b85c-113">Имя расположения, из которого был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="7b85c-113">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="7b85c-114">to</span><span class="sxs-lookup"><span data-stu-id="7b85c-114">to</span></span>            | <span data-ttu-id="7b85c-115">string</span><span class="sxs-lookup"><span data-stu-id="7b85c-115">string</span></span> | <span data-ttu-id="7b85c-116">Имя расположения, в которое был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="7b85c-116">The name of the location the item was moved to.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b85c-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7b85c-117">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.moveAction"
}-->

```json
{
  "from": "string",
  "to": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction",
  "suppressions": []
}
-->

