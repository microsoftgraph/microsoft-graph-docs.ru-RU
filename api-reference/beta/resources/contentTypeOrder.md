---
author: daspek
description: Ресурс contentTypeOrder указывает, в каком порядке тип контента будет отображаться в пользовательском интерфейсе выбора.
ms.date: 09/13/2017
title: contentTypeOrder
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 464ac5978f505e74ca99226080c35574917fd550
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973211"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="dba94-103">Тип ресурса contentTypeOrder</span><span class="sxs-lookup"><span data-stu-id="dba94-103">ContentTypeOrder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dba94-104">Ресурс **contentTypeOrder** указывает, в каком порядке тип контента будет отображаться в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="dba94-104">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dba94-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="dba94-105">JSON representation</span></span>

<span data-ttu-id="dba94-106">Ниже показано представление ресурса **contentTypeOrder** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dba94-106">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="dba94-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dba94-107">Properties</span></span>

| <span data-ttu-id="dba94-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="dba94-108">Property name</span></span> | <span data-ttu-id="dba94-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dba94-109">Type</span></span>    | <span data-ttu-id="dba94-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dba94-110">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="dba94-111">**default**</span><span class="sxs-lookup"><span data-stu-id="dba94-111">**default**</span></span>   | <span data-ttu-id="dba94-112">boolean</span><span class="sxs-lookup"><span data-stu-id="dba94-112">boolean</span></span> | <span data-ttu-id="dba94-113">Указывает, используется ли этот тип контента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dba94-113">Whether this is the default Content Type</span></span>
| <span data-ttu-id="dba94-114">**position**</span><span class="sxs-lookup"><span data-stu-id="dba94-114">**position**</span></span>  | <span data-ttu-id="dba94-115">Int32</span><span class="sxs-lookup"><span data-stu-id="dba94-115">Int32</span></span>   | <span data-ttu-id="dba94-116">Указывает позицию, в которой тип контента отображается в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="dba94-116">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder",
  "suppressions": []
}
-->
