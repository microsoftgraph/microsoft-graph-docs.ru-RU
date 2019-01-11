---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CreateAction
localization_priority: Normal
ms.openlocfilehash: ebdcabf51017bb407090d9ab4690b9e693a12953
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866061"
---
# <a name="createaction-resource-type"></a><span data-ttu-id="bc0b6-102">Тип ресурса CreateAction</span><span class="sxs-lookup"><span data-stu-id="bc0b6-102">CreateAction resource type</span></span>

> <span data-ttu-id="bc0b6-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bc0b6-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc0b6-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc0b6-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc0b6-105">Наличие ресурса **CreateAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия был создан элемент.</span><span class="sxs-lookup"><span data-stu-id="bc0b6-105">The presence of the **CreateAction** resource on an [**itemActivity**][activity] indicates that the activity created an item.</span></span>

<span data-ttu-id="bc0b6-106">**Примечание.** На данный момент этот ресурс пуст, но в будущих редакциях API в него могут быть добавлены дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="bc0b6-106">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="bc0b6-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bc0b6-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.createAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="bc0b6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc0b6-108">Properties</span></span>

<span data-ttu-id="bc0b6-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bc0b6-109">None.</span></span> <span data-ttu-id="bc0b6-110">Этот аспект принимает нулевое или ненулевое значение и не содержит свойств.</span><span class="sxs-lookup"><span data-stu-id="bc0b6-110">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="bc0b6-111">Замечания</span><span class="sxs-lookup"><span data-stu-id="bc0b6-111">Remarks</span></span>

<span data-ttu-id="bc0b6-112">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="bc0b6-112">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The CreateAction object provides information about the creation of an item.",
  "keywords": "activities,activity,action,create,creation",
  "section": "documentation",
  "tocPath": "Resources/CreateAction"
} -->
