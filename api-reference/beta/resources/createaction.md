---
author: daspek
description: Наличие ресурса CreateAction в ресурсе itemActivity указывает, что в результате выполнения действия был создан элемент.
ms.date: 09/14/2017
title: CreateAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e47a57e392ef629730a9de68c973d54b2ab5c2fe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973183"
---
# <a name="createaction-resource-type"></a><span data-ttu-id="d88f5-103">Тип ресурса CreateAction</span><span class="sxs-lookup"><span data-stu-id="d88f5-103">CreateAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d88f5-104">Наличие ресурса **CreateAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия был создан элемент.</span><span class="sxs-lookup"><span data-stu-id="d88f5-104">The presence of the **CreateAction** resource on an [**itemActivity**][activity] indicates that the activity created an item.</span></span>

<span data-ttu-id="d88f5-105">**Примечание.** На данный момент этот ресурс пуст, но в будущих редакциях API в него могут быть добавлены дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="d88f5-105">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="d88f5-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d88f5-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.createAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="d88f5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d88f5-107">Properties</span></span>

<span data-ttu-id="d88f5-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="d88f5-108">None.</span></span> <span data-ttu-id="d88f5-109">Этот аспект принимает нулевое или ненулевое значение и не содержит свойств.</span><span class="sxs-lookup"><span data-stu-id="d88f5-109">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="d88f5-110">Замечания</span><span class="sxs-lookup"><span data-stu-id="d88f5-110">Remarks</span></span>

<span data-ttu-id="d88f5-111">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="d88f5-111">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
