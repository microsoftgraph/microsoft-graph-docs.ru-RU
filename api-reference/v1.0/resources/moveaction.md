---
author: daspek
ms.author: dspektor
title: Тип ресурса moveAction
description: Объект MoveAction предоставляет сведения о действии, которое переместит элемент.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 04c9ddad00b5705d84af6e72ac194a0d32fd015c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447383"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="c1c74-103">Тип ресурса moveAction</span><span class="sxs-lookup"><span data-stu-id="c1c74-103">moveAction resource type</span></span>

<span data-ttu-id="c1c74-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c1c74-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c1c74-105">Присутствие ресурса **moveAction** в [**itemActivity**][activity] указывает на то, что действие переместило элемент.</span><span class="sxs-lookup"><span data-stu-id="c1c74-105">The presence of the **moveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

><span data-ttu-id="c1c74-106">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c1c74-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="c1c74-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1c74-107">Properties</span></span>

| <span data-ttu-id="c1c74-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c1c74-108">Property name</span></span> | <span data-ttu-id="c1c74-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c1c74-109">Type</span></span>   | <span data-ttu-id="c1c74-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c1c74-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="c1c74-111">from</span><span class="sxs-lookup"><span data-stu-id="c1c74-111">from</span></span>          | <span data-ttu-id="c1c74-112">строка</span><span class="sxs-lookup"><span data-stu-id="c1c74-112">string</span></span> | <span data-ttu-id="c1c74-113">Имя расположения, из которого был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="c1c74-113">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="c1c74-114">to</span><span class="sxs-lookup"><span data-stu-id="c1c74-114">to</span></span>            | <span data-ttu-id="c1c74-115">string</span><span class="sxs-lookup"><span data-stu-id="c1c74-115">string</span></span> | <span data-ttu-id="c1c74-116">Имя расположения, в которое был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="c1c74-116">The name of the location the item was moved to.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1c74-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1c74-117">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.moveAction"
}-->

```json
{
  "from": "string",
  "to": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction",
  "suppressions": []
}
-->
