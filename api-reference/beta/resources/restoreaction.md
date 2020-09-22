---
author: daspek
description: <decription>
ms.date: 09/14/2017
title: RestoreAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: fca74c8bdfbae8c43f5dab0cafbe9cd4abadd008
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026262"
---
# <a name="restoreaction-resource-type"></a><span data-ttu-id="e5da1-102">Тип ресурса RestoreAction</span><span class="sxs-lookup"><span data-stu-id="e5da1-102">RestoreAction resource type</span></span>

<span data-ttu-id="e5da1-103">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5da1-103">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5da1-104">Наличие ресурса **RestoreAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был восстановлен.</span><span class="sxs-lookup"><span data-stu-id="e5da1-104">The presence of the **RestoreAction** resource on an [**itemActivity**][activity] indicates that the activity restored an item.</span></span>

<span data-ttu-id="e5da1-105">**Примечание.** На данный момент этот ресурс пуст, но в будущих редакциях API в него могут быть добавлены дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="e5da1-105">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="e5da1-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e5da1-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.restoreAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="e5da1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5da1-107">Properties</span></span>

<span data-ttu-id="e5da1-108">Нет</span><span class="sxs-lookup"><span data-stu-id="e5da1-108">None.</span></span> <span data-ttu-id="e5da1-109">Этот аспект принимает нулевое или ненулевое значение и не содержит свойств.</span><span class="sxs-lookup"><span data-stu-id="e5da1-109">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="e5da1-110">Замечания</span><span class="sxs-lookup"><span data-stu-id="e5da1-110">Remarks</span></span>

<span data-ttu-id="e5da1-111">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e5da1-111">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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


