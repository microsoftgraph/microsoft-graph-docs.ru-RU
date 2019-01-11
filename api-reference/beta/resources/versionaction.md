---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: VersionAction
localization_priority: Normal
ms.openlocfilehash: 1f315b26c45e337986784200fb6ec2c78612344b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866712"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="8eddb-102">Тип ресурса VersionAction</span><span class="sxs-lookup"><span data-stu-id="8eddb-102">VersionAction resource type</span></span>

> <span data-ttu-id="8eddb-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8eddb-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8eddb-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8eddb-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8eddb-105">Наличие ресурса **VersionAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия была создана другая версия.</span><span class="sxs-lookup"><span data-stu-id="8eddb-105">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="8eddb-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8eddb-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8eddb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8eddb-107">Properties</span></span>

| <span data-ttu-id="8eddb-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="8eddb-108">Property name</span></span> | <span data-ttu-id="8eddb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8eddb-109">Type</span></span>   | <span data-ttu-id="8eddb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8eddb-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="8eddb-111">newVersion</span><span class="sxs-lookup"><span data-stu-id="8eddb-111">newVersion</span></span>    | <span data-ttu-id="8eddb-112">string</span><span class="sxs-lookup"><span data-stu-id="8eddb-112">string</span></span> | <span data-ttu-id="8eddb-113">Имя новой версии, созданной при выполнении этого действия.</span><span class="sxs-lookup"><span data-stu-id="8eddb-113">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="8eddb-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="8eddb-114">Remarks</span></span>

<span data-ttu-id="8eddb-115">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="8eddb-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction"
} -->
