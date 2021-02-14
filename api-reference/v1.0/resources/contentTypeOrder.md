---
author: daspek
ms.date: 09/13/2017
title: contentTypeOrder
localization_priority: Normal
description: Ресурс contentTypeOrder указывает, в каком порядке тип контента будет отображаться в пользовательском интерфейсе выбора.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e25025e86c03d7c94ed88a94ad390a56db4a44b0
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238507"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="c27ec-103">Тип ресурса contentTypeOrder</span><span class="sxs-lookup"><span data-stu-id="c27ec-103">ContentTypeOrder resource type</span></span>

<span data-ttu-id="c27ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c27ec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c27ec-105">Ресурс **contentTypeOrder** указывает, в каком порядке тип контента будет отображаться в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="c27ec-105">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c27ec-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c27ec-106">JSON representation</span></span>

<span data-ttu-id="c27ec-107">Ниже показано представление ресурса **contentTypeOrder** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c27ec-107">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="c27ec-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c27ec-108">Properties</span></span>

| <span data-ttu-id="c27ec-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c27ec-109">Property name</span></span> | <span data-ttu-id="c27ec-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c27ec-110">Type</span></span>    | <span data-ttu-id="c27ec-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c27ec-111">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="c27ec-112">**default**</span><span class="sxs-lookup"><span data-stu-id="c27ec-112">**default**</span></span>   | <span data-ttu-id="c27ec-113">boolean</span><span class="sxs-lookup"><span data-stu-id="c27ec-113">boolean</span></span> | <span data-ttu-id="c27ec-114">Указывает, используется ли этот тип контента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c27ec-114">Whether this is the default Content Type</span></span>
| <span data-ttu-id="c27ec-115">**position**</span><span class="sxs-lookup"><span data-stu-id="c27ec-115">**position**</span></span>  | <span data-ttu-id="c27ec-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c27ec-116">Int32</span></span>   | <span data-ttu-id="c27ec-117">Указывает позицию, в которой тип контента отображается в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="c27ec-117">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->

