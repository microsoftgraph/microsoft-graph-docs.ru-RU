---
author: daspek
ms.author: dspektor
title: Тип ресурса versionAction
description: Объект VersionAction предоставляет сведения о действии, которое привело к созданию новой версии элемента.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 0d05ad93c59ba736dd90276fc5e3db6e05740344
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970793"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="24c49-103">Тип ресурса versionAction</span><span class="sxs-lookup"><span data-stu-id="24c49-103">versionAction resource type</span></span>

<span data-ttu-id="24c49-104">Присутствие ресурса **versionAction** в [**itemActivity**] [ activity] указывает на то, что действие привело к созданию новой версии.</span><span class="sxs-lookup"><span data-stu-id="24c49-104">The presence of the **versionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

><span data-ttu-id="24c49-105">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="24c49-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="24c49-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="24c49-106">Properties</span></span>

| <span data-ttu-id="24c49-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="24c49-107">Property name</span></span> | <span data-ttu-id="24c49-108">Тип</span><span class="sxs-lookup"><span data-stu-id="24c49-108">Type</span></span>   | <span data-ttu-id="24c49-109">Описание</span><span class="sxs-lookup"><span data-stu-id="24c49-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="24c49-110">newVersion</span><span class="sxs-lookup"><span data-stu-id="24c49-110">newVersion</span></span>    | <span data-ttu-id="24c49-111">string</span><span class="sxs-lookup"><span data-stu-id="24c49-111">string</span></span> | <span data-ttu-id="24c49-112">Имя новой версии, созданной при выполнении этого действия.</span><span class="sxs-lookup"><span data-stu-id="24c49-112">The name of the new version that was created by this action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="24c49-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24c49-113">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.versionAction"
}-->

```json
{
  "newVersion": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction",
  "suppressions": []
}
-->
