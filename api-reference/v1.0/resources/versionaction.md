---
author: daspek
ms.author: dspektor
title: Тип ресурса versionAction
description: Объект VersionAction предоставляет сведения о действии, которое привело к созданию новой версии элемента.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 94efbb554420030eb33a814de72d5d79ab065738
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015283"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="9f418-103">Тип ресурса versionAction</span><span class="sxs-lookup"><span data-stu-id="9f418-103">versionAction resource type</span></span>

<span data-ttu-id="9f418-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f418-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9f418-105">Присутствие ресурса **versionAction** в [**itemActivity**][activity] указывает на то, что действие привело к созданию новой версии.</span><span class="sxs-lookup"><span data-stu-id="9f418-105">The presence of the **versionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

><span data-ttu-id="9f418-106">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="9f418-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="9f418-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f418-107">Properties</span></span>

| <span data-ttu-id="9f418-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="9f418-108">Property name</span></span> | <span data-ttu-id="9f418-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9f418-109">Type</span></span>   | <span data-ttu-id="9f418-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9f418-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="9f418-111">newVersion</span><span class="sxs-lookup"><span data-stu-id="9f418-111">newVersion</span></span>    | <span data-ttu-id="9f418-112">string</span><span class="sxs-lookup"><span data-stu-id="9f418-112">string</span></span> | <span data-ttu-id="9f418-113">Имя новой версии, созданной при выполнении этого действия.</span><span class="sxs-lookup"><span data-stu-id="9f418-113">The name of the new version that was created by this action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f418-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9f418-114">JSON representation</span></span>

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

