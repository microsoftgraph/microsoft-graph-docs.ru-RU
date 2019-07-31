---
author: daspek
description: Наличие ресурса VersionAction в ресурсе itemActivity указывает, что в результате выполнения действия была создана другая версия.
ms.date: 09/14/2017
title: VersionAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8eeec313ac4ed901d7552e2ad65d02edcaa821cd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007398"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="9130c-103">Тип ресурса VersionAction</span><span class="sxs-lookup"><span data-stu-id="9130c-103">VersionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9130c-104">Наличие ресурса **VersionAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия была создана другая версия.</span><span class="sxs-lookup"><span data-stu-id="9130c-104">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="9130c-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9130c-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="9130c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9130c-106">Properties</span></span>

| <span data-ttu-id="9130c-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="9130c-107">Property name</span></span> | <span data-ttu-id="9130c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9130c-108">Type</span></span>   | <span data-ttu-id="9130c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9130c-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="9130c-110">newVersion</span><span class="sxs-lookup"><span data-stu-id="9130c-110">newVersion</span></span>    | <span data-ttu-id="9130c-111">string</span><span class="sxs-lookup"><span data-stu-id="9130c-111">string</span></span> | <span data-ttu-id="9130c-112">Имя новой версии, созданной при выполнении этого действия.</span><span class="sxs-lookup"><span data-stu-id="9130c-112">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="9130c-113">Замечания</span><span class="sxs-lookup"><span data-stu-id="9130c-113">Remarks</span></span>

<span data-ttu-id="9130c-114">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="9130c-114">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
