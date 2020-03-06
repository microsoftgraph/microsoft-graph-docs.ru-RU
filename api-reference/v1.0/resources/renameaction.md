---
author: daspek
ms.author: dspektor
title: Тип ресурса renameAction
description: Объект renameAction предоставляет сведения о действии, которое переименовало элемент.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b21d4630ca29aff9322d5114a5048b42f19fa4a0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533850"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="bad0e-103">Тип ресурса renameAction</span><span class="sxs-lookup"><span data-stu-id="bad0e-103">renameAction resource type</span></span>

<span data-ttu-id="bad0e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bad0e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bad0e-105">Присутствие ресурса **renameAction** в [**itemActivity**][activity] указывает, что действие переименовало элемент.</span><span class="sxs-lookup"><span data-stu-id="bad0e-105">The presence of the **renameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

><span data-ttu-id="bad0e-106">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="bad0e-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="bad0e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bad0e-107">Properties</span></span>

| <span data-ttu-id="bad0e-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="bad0e-108">Property name</span></span> | <span data-ttu-id="bad0e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bad0e-109">Type</span></span>   | <span data-ttu-id="bad0e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bad0e-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="bad0e-111">oldName</span><span class="sxs-lookup"><span data-stu-id="bad0e-111">oldName</span></span>       | <span data-ttu-id="bad0e-112">string</span><span class="sxs-lookup"><span data-stu-id="bad0e-112">string</span></span> | <span data-ttu-id="bad0e-113">Предыдущее имя элемента.</span><span class="sxs-lookup"><span data-stu-id="bad0e-113">The previous name of the item.</span></span>
| <span data-ttu-id="bad0e-114">Новое</span><span class="sxs-lookup"><span data-stu-id="bad0e-114">newName</span></span>       | <span data-ttu-id="bad0e-115">string</span><span class="sxs-lookup"><span data-stu-id="bad0e-115">string</span></span> | <span data-ttu-id="bad0e-116">Новое имя элемента.</span><span class="sxs-lookup"><span data-stu-id="bad0e-116">The new name of the item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bad0e-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bad0e-117">JSON representation</span></span>

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
