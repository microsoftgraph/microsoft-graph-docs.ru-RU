---
author: daspek
description: Наличие ресурса CreateAction в ресурсе itemActivity указывает, что в результате выполнения действия был создан элемент.
ms.date: 09/14/2017
title: CreateAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 349a46b4fc4b13fd597f120fdc4ca4d6641e932e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507368"
---
# <a name="createaction-resource-type"></a><span data-ttu-id="0f1f8-103">Тип ресурса CreateAction</span><span class="sxs-lookup"><span data-stu-id="0f1f8-103">CreateAction resource type</span></span>

<span data-ttu-id="0f1f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f1f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f1f8-105">Наличие ресурса **CreateAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия был создан элемент.</span><span class="sxs-lookup"><span data-stu-id="0f1f8-105">The presence of the **CreateAction** resource on an [**itemActivity**][activity] indicates that the activity created an item.</span></span>

<span data-ttu-id="0f1f8-106">**Примечание.** На данный момент этот ресурс пуст, но в будущих редакциях API в него могут быть добавлены дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="0f1f8-106">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="0f1f8-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0f1f8-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.createAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="0f1f8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f1f8-108">Properties</span></span>

<span data-ttu-id="0f1f8-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0f1f8-109">None.</span></span> <span data-ttu-id="0f1f8-110">Этот аспект принимает нулевое или ненулевое значение и не содержит свойств.</span><span class="sxs-lookup"><span data-stu-id="0f1f8-110">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="0f1f8-111">Замечания</span><span class="sxs-lookup"><span data-stu-id="0f1f8-111">Remarks</span></span>

<span data-ttu-id="0f1f8-112">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="0f1f8-112">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The CreateAction object provides information about the creation of an item.",
  "keywords": "activities,activity,action,create,creation",
  "section": "documentation",
  "tocPath": "Resources/CreateAction",
  "suppressions": []
}
-->
