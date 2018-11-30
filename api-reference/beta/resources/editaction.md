---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: EditAction
ms.openlocfilehash: 5ff2580f21f09a88b4747114e6070a5c7b523728
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081828"
---
# <a name="editaction-resource-type"></a><span data-ttu-id="d435e-102">Тип ресурса EditAction</span><span class="sxs-lookup"><span data-stu-id="d435e-102">EditAction resource type</span></span>

> <span data-ttu-id="d435e-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d435e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d435e-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d435e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d435e-105">Наличие ресурса **EditAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был изменен.</span><span class="sxs-lookup"><span data-stu-id="d435e-105">The presence of the **EditAction** resource on an [**itemActivity**][activity] indicates that the activity edited an item.</span></span>

<span data-ttu-id="d435e-106">**Примечание.** На данный момент этот ресурс пуст, но в будущих редакциях API в него могут быть добавлены дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="d435e-106">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="d435e-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d435e-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.editAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="d435e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d435e-108">Properties</span></span>

<span data-ttu-id="d435e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d435e-109">None.</span></span> <span data-ttu-id="d435e-110">Этот аспект принимает нулевое или ненулевое значение и не содержит свойств.</span><span class="sxs-lookup"><span data-stu-id="d435e-110">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="d435e-111">Замечания</span><span class="sxs-lookup"><span data-stu-id="d435e-111">Remarks</span></span>

<span data-ttu-id="d435e-112">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="d435e-112">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The EditAction object provides information about an activity that edited an item.",
  "keywords": "activities,activity,action,edit,modify",
  "section": "documentation",
  "tocPath": "Resources/EditAction"
} -->
