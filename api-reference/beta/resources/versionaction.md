---
author: daspek
description: Наличие ресурса VersionAction в ресурсе itemActivity указывает, что в результате выполнения действия была создана другая версия.
ms.date: 09/14/2017
title: VersionAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 0f16858c8b62f327019d2523488827fa6b20dced
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057747"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="2a3d9-103">Тип ресурса VersionAction</span><span class="sxs-lookup"><span data-stu-id="2a3d9-103">VersionAction resource type</span></span>

<span data-ttu-id="2a3d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a3d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a3d9-105">Наличие ресурса **VersionAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия была создана другая версия.</span><span class="sxs-lookup"><span data-stu-id="2a3d9-105">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="2a3d9-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a3d9-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2a3d9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a3d9-107">Properties</span></span>

| <span data-ttu-id="2a3d9-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2a3d9-108">Property name</span></span> | <span data-ttu-id="2a3d9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2a3d9-109">Type</span></span>   | <span data-ttu-id="2a3d9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2a3d9-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="2a3d9-111">newVersion</span><span class="sxs-lookup"><span data-stu-id="2a3d9-111">newVersion</span></span>    | <span data-ttu-id="2a3d9-112">string</span><span class="sxs-lookup"><span data-stu-id="2a3d9-112">string</span></span> | <span data-ttu-id="2a3d9-113">Имя новой версии, созданной при выполнении этого действия.</span><span class="sxs-lookup"><span data-stu-id="2a3d9-113">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="2a3d9-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="2a3d9-114">Remarks</span></span>

<span data-ttu-id="2a3d9-115">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="2a3d9-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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


