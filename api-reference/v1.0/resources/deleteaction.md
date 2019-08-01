---
author: daspek
ms.author: dspektor
title: Тип ресурса deleteAction
description: Объект deleteAction предоставляет сведения об удалении элемента.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 93f605e74a0a483a94593a9aaa40d6fd30efe914
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032734"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="e9fee-103">Тип ресурса deleteAction</span><span class="sxs-lookup"><span data-stu-id="e9fee-103">deleteAction resource type</span></span>

<span data-ttu-id="e9fee-104">Присутствие ресурса **deleteAction** в [**itemActivity**][activity] указывает на то, что действие удалило элемент.</span><span class="sxs-lookup"><span data-stu-id="e9fee-104">The presence of the **deleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

><span data-ttu-id="e9fee-105">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e9fee-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="e9fee-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9fee-106">Properties</span></span>

| <span data-ttu-id="e9fee-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e9fee-107">Property name</span></span> | <span data-ttu-id="e9fee-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e9fee-108">Type</span></span>   | <span data-ttu-id="e9fee-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e9fee-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="e9fee-110">name</span><span class="sxs-lookup"><span data-stu-id="e9fee-110">name</span></span>          | <span data-ttu-id="e9fee-111">string</span><span class="sxs-lookup"><span data-stu-id="e9fee-111">string</span></span> | <span data-ttu-id="e9fee-112">Имя элемента, который был удален.</span><span class="sxs-lookup"><span data-stu-id="e9fee-112">The name of the item that was deleted.</span></span>
| <span data-ttu-id="e9fee-113">objectType</span><span class="sxs-lookup"><span data-stu-id="e9fee-113">objectType</span></span>    | <span data-ttu-id="e9fee-114">string</span><span class="sxs-lookup"><span data-stu-id="e9fee-114">string</span></span> | <span data-ttu-id="e9fee-115">`File`или `Folder`, в зависимости от типа удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="e9fee-115">`File` or `Folder`, depending on the type of the deleted item.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e9fee-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9fee-116">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType": "File | Folder"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The deleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": []
}
-->
