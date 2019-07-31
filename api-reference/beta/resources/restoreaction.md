---
author: daspek
description: <decription>
ms.date: 09/14/2017
title: RestoreAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 88adfd244e2f8460d6749333cc64a80bf4d47361
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008693"
---
# <a name="restoreaction-resource-type"></a><span data-ttu-id="4031c-102">Тип ресурса RestoreAction</span><span class="sxs-lookup"><span data-stu-id="4031c-102">RestoreAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4031c-103">Наличие ресурса **RestoreAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был восстановлен.</span><span class="sxs-lookup"><span data-stu-id="4031c-103">The presence of the **RestoreAction** resource on an [**itemActivity**][activity] indicates that the activity restored an item.</span></span>

<span data-ttu-id="4031c-104">**Примечание.** На данный момент этот ресурс пуст, но в будущих редакциях API в него могут быть добавлены дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="4031c-104">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="4031c-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4031c-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.restoreAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="4031c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4031c-106">Properties</span></span>

<span data-ttu-id="4031c-107">Нет.</span><span class="sxs-lookup"><span data-stu-id="4031c-107">None.</span></span> <span data-ttu-id="4031c-108">Этот аспект принимает нулевое или ненулевое значение и не содержит свойств.</span><span class="sxs-lookup"><span data-stu-id="4031c-108">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="4031c-109">Замечания</span><span class="sxs-lookup"><span data-stu-id="4031c-109">Remarks</span></span>

<span data-ttu-id="4031c-110">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4031c-110">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
