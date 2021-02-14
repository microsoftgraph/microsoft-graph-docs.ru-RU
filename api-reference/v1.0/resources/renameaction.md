---
author: daspek
title: Тип ресурса renameAction
description: Объект renameAction предоставляет сведения о действии, которое переименовывает элемент.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 35e0aa9929b8e152265a5540625f5981a587edb7
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238654"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="1f21c-103">Тип ресурса renameAction</span><span class="sxs-lookup"><span data-stu-id="1f21c-103">renameAction resource type</span></span>

<span data-ttu-id="1f21c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f21c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1f21c-105">Наличие ресурса **renameAction** в [**itemActivity**][activity] означает, что действие переименовывает элемент.</span><span class="sxs-lookup"><span data-stu-id="1f21c-105">The presence of the **renameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

><span data-ttu-id="1f21c-106">**Примечание.** Записи о действиях с элементами в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1f21c-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="1f21c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f21c-107">Properties</span></span>

| <span data-ttu-id="1f21c-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="1f21c-108">Property name</span></span> | <span data-ttu-id="1f21c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1f21c-109">Type</span></span>   | <span data-ttu-id="1f21c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1f21c-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="1f21c-111">oldName</span><span class="sxs-lookup"><span data-stu-id="1f21c-111">oldName</span></span>       | <span data-ttu-id="1f21c-112">string</span><span class="sxs-lookup"><span data-stu-id="1f21c-112">string</span></span> | <span data-ttu-id="1f21c-113">Предыдущее имя элемента.</span><span class="sxs-lookup"><span data-stu-id="1f21c-113">The previous name of the item.</span></span>
| <span data-ttu-id="1f21c-114">newName</span><span class="sxs-lookup"><span data-stu-id="1f21c-114">newName</span></span>       | <span data-ttu-id="1f21c-115">string</span><span class="sxs-lookup"><span data-stu-id="1f21c-115">string</span></span> | <span data-ttu-id="1f21c-116">Новое имя элемента.</span><span class="sxs-lookup"><span data-stu-id="1f21c-116">The new name of the item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f21c-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f21c-117">JSON representation</span></span>

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

