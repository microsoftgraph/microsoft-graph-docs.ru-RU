---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: contentTypeOrder
localization_priority: Normal
description: Ресурс contentTypeOrder указывает, в каком порядке тип контента будет отображаться в пользовательском интерфейсе выбора.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2015b0def71ece538fddafde407e8bf044375b4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056942"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="09e13-103">Тип ресурса contentTypeOrder</span><span class="sxs-lookup"><span data-stu-id="09e13-103">ContentTypeOrder resource type</span></span>

<span data-ttu-id="09e13-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09e13-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="09e13-105">Ресурс **contentTypeOrder** указывает, в каком порядке тип контента будет отображаться в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="09e13-105">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="09e13-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="09e13-106">JSON representation</span></span>

<span data-ttu-id="09e13-107">Ниже показано представление ресурса **contentTypeOrder** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09e13-107">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="09e13-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="09e13-108">Properties</span></span>

| <span data-ttu-id="09e13-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="09e13-109">Property name</span></span> | <span data-ttu-id="09e13-110">Тип</span><span class="sxs-lookup"><span data-stu-id="09e13-110">Type</span></span>    | <span data-ttu-id="09e13-111">Описание</span><span class="sxs-lookup"><span data-stu-id="09e13-111">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="09e13-112">**default**</span><span class="sxs-lookup"><span data-stu-id="09e13-112">**default**</span></span>   | <span data-ttu-id="09e13-113">boolean</span><span class="sxs-lookup"><span data-stu-id="09e13-113">boolean</span></span> | <span data-ttu-id="09e13-114">Указывает, используется ли этот тип контента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="09e13-114">Whether this is the default Content Type</span></span>
| <span data-ttu-id="09e13-115">**position**</span><span class="sxs-lookup"><span data-stu-id="09e13-115">**position**</span></span>  | <span data-ttu-id="09e13-116">Int32</span><span class="sxs-lookup"><span data-stu-id="09e13-116">Int32</span></span>   | <span data-ttu-id="09e13-117">Указывает позицию, в которой тип контента отображается в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="09e13-117">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->

