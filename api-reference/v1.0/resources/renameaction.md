---
author: daspek
ms.author: dspektor
title: Тип ресурса renameAction
description: Объект renameAction предоставляет сведения о действии, которое переименовало элемент.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bce040130d74b7977fc1f988a34edde674f9e0d4
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970803"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="71edd-103">Тип ресурса renameAction</span><span class="sxs-lookup"><span data-stu-id="71edd-103">renameAction resource type</span></span>

<span data-ttu-id="71edd-104">Присутствие ресурса **renameAction** в [**itemActivity**] [ activity] указывает, что действие переименовало элемент.</span><span class="sxs-lookup"><span data-stu-id="71edd-104">The presence of the **renameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

><span data-ttu-id="71edd-105">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="71edd-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="71edd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="71edd-106">Properties</span></span>

| <span data-ttu-id="71edd-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="71edd-107">Property name</span></span> | <span data-ttu-id="71edd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="71edd-108">Type</span></span>   | <span data-ttu-id="71edd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="71edd-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="71edd-110">oldName</span><span class="sxs-lookup"><span data-stu-id="71edd-110">oldName</span></span>       | <span data-ttu-id="71edd-111">string</span><span class="sxs-lookup"><span data-stu-id="71edd-111">string</span></span> | <span data-ttu-id="71edd-112">Предыдущее имя элемента.</span><span class="sxs-lookup"><span data-stu-id="71edd-112">The previous name of the item.</span></span>
| <span data-ttu-id="71edd-113">Новое</span><span class="sxs-lookup"><span data-stu-id="71edd-113">newName</span></span>       | <span data-ttu-id="71edd-114">string</span><span class="sxs-lookup"><span data-stu-id="71edd-114">string</span></span> | <span data-ttu-id="71edd-115">Новое имя элемента.</span><span class="sxs-lookup"><span data-stu-id="71edd-115">The new name of the item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="71edd-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71edd-116">JSON representation</span></span>

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
