---
author: daspek
ms.author: dspektor
title: Тип ресурса renameAction
description: Объект renameAction предоставляет сведения о действии, которое переименовало элемент.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 2949a3875d657dba3c64b6753855476c1d66bfb3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034722"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="24610-103">Тип ресурса renameAction</span><span class="sxs-lookup"><span data-stu-id="24610-103">renameAction resource type</span></span>

<span data-ttu-id="24610-104">Присутствие ресурса **renameAction** в [**itemActivity**][activity] указывает, что действие переименовало элемент.</span><span class="sxs-lookup"><span data-stu-id="24610-104">The presence of the **renameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

><span data-ttu-id="24610-105">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="24610-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="24610-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="24610-106">Properties</span></span>

| <span data-ttu-id="24610-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="24610-107">Property name</span></span> | <span data-ttu-id="24610-108">Тип</span><span class="sxs-lookup"><span data-stu-id="24610-108">Type</span></span>   | <span data-ttu-id="24610-109">Описание</span><span class="sxs-lookup"><span data-stu-id="24610-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="24610-110">oldName</span><span class="sxs-lookup"><span data-stu-id="24610-110">oldName</span></span>       | <span data-ttu-id="24610-111">string</span><span class="sxs-lookup"><span data-stu-id="24610-111">string</span></span> | <span data-ttu-id="24610-112">Предыдущее имя элемента.</span><span class="sxs-lookup"><span data-stu-id="24610-112">The previous name of the item.</span></span>
| <span data-ttu-id="24610-113">Новое</span><span class="sxs-lookup"><span data-stu-id="24610-113">newName</span></span>       | <span data-ttu-id="24610-114">string</span><span class="sxs-lookup"><span data-stu-id="24610-114">string</span></span> | <span data-ttu-id="24610-115">Новое имя элемента.</span><span class="sxs-lookup"><span data-stu-id="24610-115">The new name of the item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="24610-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24610-116">JSON representation</span></span>

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
