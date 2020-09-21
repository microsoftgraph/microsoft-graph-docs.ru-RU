---
author: daspek
ms.author: dspektor
title: Тип ресурса renameAction
description: Объект renameAction предоставляет сведения о действии, которое переименовало элемент.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 693c5d8586a7ceef2c30f1e6dae17ac47d8e2d1f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967319"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="2e8f9-103">Тип ресурса renameAction</span><span class="sxs-lookup"><span data-stu-id="2e8f9-103">renameAction resource type</span></span>

<span data-ttu-id="2e8f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e8f9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2e8f9-105">Присутствие ресурса **renameAction** в [**itemActivity**][activity] указывает, что действие переименовало элемент.</span><span class="sxs-lookup"><span data-stu-id="2e8f9-105">The presence of the **renameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

><span data-ttu-id="2e8f9-106">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="2e8f9-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="2e8f9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e8f9-107">Properties</span></span>

| <span data-ttu-id="2e8f9-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2e8f9-108">Property name</span></span> | <span data-ttu-id="2e8f9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2e8f9-109">Type</span></span>   | <span data-ttu-id="2e8f9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2e8f9-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="2e8f9-111">oldName</span><span class="sxs-lookup"><span data-stu-id="2e8f9-111">oldName</span></span>       | <span data-ttu-id="2e8f9-112">string</span><span class="sxs-lookup"><span data-stu-id="2e8f9-112">string</span></span> | <span data-ttu-id="2e8f9-113">Предыдущее имя элемента.</span><span class="sxs-lookup"><span data-stu-id="2e8f9-113">The previous name of the item.</span></span>
| <span data-ttu-id="2e8f9-114">Новое</span><span class="sxs-lookup"><span data-stu-id="2e8f9-114">newName</span></span>       | <span data-ttu-id="2e8f9-115">string</span><span class="sxs-lookup"><span data-stu-id="2e8f9-115">string</span></span> | <span data-ttu-id="2e8f9-116">Новое имя элемента.</span><span class="sxs-lookup"><span data-stu-id="2e8f9-116">The new name of the item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e8f9-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e8f9-117">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.renameAction"
}-->

```json
{
  "oldName": "string",
  "newName": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The renameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/renameAction",
  "suppressions": []
}
-->

