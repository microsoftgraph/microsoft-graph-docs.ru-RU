---
author: daspek
ms.author: dspektor
title: Тип ресурса versionAction
description: Объект VersionAction предоставляет сведения о действии, которое привело к созданию новой версии элемента.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 22f06691824d2ffa5b773a796b4c456cb2fcaecc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033448"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="25b5b-103">Тип ресурса versionAction</span><span class="sxs-lookup"><span data-stu-id="25b5b-103">versionAction resource type</span></span>

<span data-ttu-id="25b5b-104">Присутствие ресурса **versionAction** в [**itemActivity**][activity] указывает на то, что действие привело к созданию новой версии.</span><span class="sxs-lookup"><span data-stu-id="25b5b-104">The presence of the **versionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

><span data-ttu-id="25b5b-105">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="25b5b-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="25b5b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="25b5b-106">Properties</span></span>

| <span data-ttu-id="25b5b-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="25b5b-107">Property name</span></span> | <span data-ttu-id="25b5b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="25b5b-108">Type</span></span>   | <span data-ttu-id="25b5b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="25b5b-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="25b5b-110">newVersion</span><span class="sxs-lookup"><span data-stu-id="25b5b-110">newVersion</span></span>    | <span data-ttu-id="25b5b-111">string</span><span class="sxs-lookup"><span data-stu-id="25b5b-111">string</span></span> | <span data-ttu-id="25b5b-112">Имя новой версии, созданной при выполнении этого действия.</span><span class="sxs-lookup"><span data-stu-id="25b5b-112">The name of the new version that was created by this action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="25b5b-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="25b5b-113">JSON representation</span></span>

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
