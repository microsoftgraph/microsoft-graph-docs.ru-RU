---
author: daspek
description: <decription>
ms.date: 09/14/2017
title: RestoreAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ec2456105c7ae1844f97e80601fe2df3bf38d028
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521091"
---
# <a name="restoreaction-resource-type"></a><span data-ttu-id="8902e-102">Тип ресурса RestoreAction</span><span class="sxs-lookup"><span data-stu-id="8902e-102">RestoreAction resource type</span></span>

<span data-ttu-id="8902e-103">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8902e-103">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8902e-104">Наличие ресурса **RestoreAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был восстановлен.</span><span class="sxs-lookup"><span data-stu-id="8902e-104">The presence of the **RestoreAction** resource on an [**itemActivity**][activity] indicates that the activity restored an item.</span></span>

<span data-ttu-id="8902e-105">**Примечание.** На данный момент этот ресурс пуст, но в будущих редакциях API в него могут быть добавлены дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="8902e-105">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="8902e-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8902e-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.restoreAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="8902e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8902e-107">Properties</span></span>

<span data-ttu-id="8902e-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="8902e-108">None.</span></span> <span data-ttu-id="8902e-109">Этот аспект принимает нулевое или ненулевое значение и не содержит свойств.</span><span class="sxs-lookup"><span data-stu-id="8902e-109">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="8902e-110">Замечания</span><span class="sxs-lookup"><span data-stu-id="8902e-110">Remarks</span></span>

<span data-ttu-id="8902e-111">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="8902e-111">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
