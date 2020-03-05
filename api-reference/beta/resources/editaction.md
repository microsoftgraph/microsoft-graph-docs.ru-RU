---
author: daspek
description: Наличие ресурса EditAction в ресурсе itemActivity указывает, что в результате выполнения действия элемент был изменен.
ms.date: 09/14/2017
title: EditAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 1b7ab5e77b62d3f02ee04a5927cb2294f5c3b5a5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502853"
---
# <a name="editaction-resource-type"></a><span data-ttu-id="36e2e-103">Тип ресурса EditAction</span><span class="sxs-lookup"><span data-stu-id="36e2e-103">EditAction resource type</span></span>

<span data-ttu-id="36e2e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="36e2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36e2e-105">Наличие ресурса **EditAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был изменен.</span><span class="sxs-lookup"><span data-stu-id="36e2e-105">The presence of the **EditAction** resource on an [**itemActivity**][activity] indicates that the activity edited an item.</span></span>

<span data-ttu-id="36e2e-106">**Примечание.** На данный момент этот ресурс пуст, но в будущих редакциях API в него могут быть добавлены дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="36e2e-106">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="36e2e-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="36e2e-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.editAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="36e2e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="36e2e-108">Properties</span></span>

<span data-ttu-id="36e2e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="36e2e-109">None.</span></span> <span data-ttu-id="36e2e-110">Этот аспект принимает нулевое или ненулевое значение и не содержит свойств.</span><span class="sxs-lookup"><span data-stu-id="36e2e-110">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="36e2e-111">Замечания</span><span class="sxs-lookup"><span data-stu-id="36e2e-111">Remarks</span></span>

<span data-ttu-id="36e2e-112">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="36e2e-112">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The EditAction object provides information about an activity that edited an item.",
  "keywords": "activities,activity,action,edit,modify",
  "section": "documentation",
  "tocPath": "Resources/EditAction",
  "suppressions": []
}
-->
