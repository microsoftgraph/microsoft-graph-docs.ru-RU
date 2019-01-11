---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RestoreAction
localization_priority: Normal
ms.openlocfilehash: 25cfe884d74b54e1cc7881415009e2df0daafa11
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831677"
---
# <a name="restoreaction-resource-type"></a><span data-ttu-id="9ac92-102">Тип ресурса RestoreAction</span><span class="sxs-lookup"><span data-stu-id="9ac92-102">RestoreAction resource type</span></span>

> <span data-ttu-id="9ac92-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9ac92-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ac92-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ac92-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9ac92-105">Наличие ресурса **RestoreAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был восстановлен.</span><span class="sxs-lookup"><span data-stu-id="9ac92-105">The presence of the **RestoreAction** resource on an [**itemActivity**][activity] indicates that the activity restored an item.</span></span>

<span data-ttu-id="9ac92-106">**Примечание.** На данный момент этот ресурс пуст, но в будущих редакциях API в него могут быть добавлены дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="9ac92-106">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="9ac92-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9ac92-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.restoreAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="9ac92-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ac92-108">Properties</span></span>

<span data-ttu-id="9ac92-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="9ac92-109">None.</span></span> <span data-ttu-id="9ac92-110">Этот аспект принимает нулевое или ненулевое значение и не содержит свойств.</span><span class="sxs-lookup"><span data-stu-id="9ac92-110">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="9ac92-111">Замечания</span><span class="sxs-lookup"><span data-stu-id="9ac92-111">Remarks</span></span>

<span data-ttu-id="9ac92-112">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="9ac92-112">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The RestoreAction object provides information about an activity that restored an item.",
  "keywords": "activities,activity,action,restore,undelete",
  "section": "documentation",
  "tocPath": "Resources/RestoreAction"
} -->
