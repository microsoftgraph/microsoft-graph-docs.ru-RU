---
author: daspek
description: Наличие ресурса EditAction в ресурсе itemActivity указывает, что в результате выполнения действия элемент был изменен.
ms.date: 09/14/2017
title: EditAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 374b4f7374ba91360bdaa97e5bc36fb0f5aabbae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006509"
---
# <a name="editaction-resource-type"></a><span data-ttu-id="cdd71-103">Тип ресурса EditAction</span><span class="sxs-lookup"><span data-stu-id="cdd71-103">EditAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdd71-104">Наличие ресурса **EditAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был изменен.</span><span class="sxs-lookup"><span data-stu-id="cdd71-104">The presence of the **EditAction** resource on an [**itemActivity**][activity] indicates that the activity edited an item.</span></span>

<span data-ttu-id="cdd71-105">**Примечание.** На данный момент этот ресурс пуст, но в будущих редакциях API в него могут быть добавлены дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="cdd71-105">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="cdd71-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cdd71-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.editAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="cdd71-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cdd71-107">Properties</span></span>

<span data-ttu-id="cdd71-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="cdd71-108">None.</span></span> <span data-ttu-id="cdd71-109">Этот аспект принимает нулевое или ненулевое значение и не содержит свойств.</span><span class="sxs-lookup"><span data-stu-id="cdd71-109">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="cdd71-110">Замечания</span><span class="sxs-lookup"><span data-stu-id="cdd71-110">Remarks</span></span>

<span data-ttu-id="cdd71-111">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="cdd71-111">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
