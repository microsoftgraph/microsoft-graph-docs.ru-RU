---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RestoreAction
localization_priority: Normal
ms.openlocfilehash: f04f9811cefba60d0b06b99605774fb8fbfa0125
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562975"
---
# <a name="restoreaction-resource-type"></a><span data-ttu-id="14949-102">Тип ресурса RestoreAction</span><span class="sxs-lookup"><span data-stu-id="14949-102">RestoreAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14949-103">Наличие ресурса **RestoreAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был восстановлен.</span><span class="sxs-lookup"><span data-stu-id="14949-103">The presence of the **RestoreAction** resource on an [**itemActivity**][activity] indicates that the activity restored an item.</span></span>

<span data-ttu-id="14949-104">**Примечание.** На данный момент этот ресурс пуст, но в будущих редакциях API в него могут быть добавлены дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="14949-104">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="14949-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="14949-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.restoreAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="14949-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="14949-106">Properties</span></span>

<span data-ttu-id="14949-107">Нет.</span><span class="sxs-lookup"><span data-stu-id="14949-107">None.</span></span> <span data-ttu-id="14949-108">Этот аспект принимает нулевое или ненулевое значение и не содержит свойств.</span><span class="sxs-lookup"><span data-stu-id="14949-108">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="14949-109">Замечания</span><span class="sxs-lookup"><span data-stu-id="14949-109">Remarks</span></span>

<span data-ttu-id="14949-110">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="14949-110">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The RestoreAction object provides information about an activity that restored an item.",
  "keywords": "activities,activity,action,restore,undelete",
  "section": "documentation",
  "tocPath": "Resources/RestoreAction",
  "suppressions": []
}
-->
