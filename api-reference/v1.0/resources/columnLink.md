---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: columnLink
localization_priority: Normal
description: Ресурс columnLink для объекта contentType связывает ресурс columnDefinition сайта с соответствующим типом контента.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d3914c4b3cfe18d2dead778116b86134caaf6caa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029696"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="b538a-103">Тип ресурса ColumnLink</span><span class="sxs-lookup"><span data-stu-id="b538a-103">ColumnLink resource type</span></span>

<span data-ttu-id="b538a-104">Ресурс **columnLink** для объекта [contentType][] связывает ресурс **columnDefinition** сайта с соответствующим типом контента.</span><span class="sxs-lookup"><span data-stu-id="b538a-104">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="b538a-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b538a-106">JSON representation</span></span>

<span data-ttu-id="b538a-107">Ниже показано представление ресурса **columnLink** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b538a-107">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="b538a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b538a-108">Properties</span></span>

| <span data-ttu-id="b538a-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="b538a-109">Property name</span></span> | <span data-ttu-id="b538a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b538a-110">Type</span></span>   | <span data-ttu-id="b538a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b538a-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="b538a-112">**id**</span><span class="sxs-lookup"><span data-stu-id="b538a-112">**id**</span></span>        | <span data-ttu-id="b538a-113">string</span><span class="sxs-lookup"><span data-stu-id="b538a-113">string</span></span> | <span data-ttu-id="b538a-114">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="b538a-114">The unique identifier for the column.</span></span>
| <span data-ttu-id="b538a-115">**name**</span><span class="sxs-lookup"><span data-stu-id="b538a-115">**name**</span></span>      | <span data-ttu-id="b538a-116">string</span><span class="sxs-lookup"><span data-stu-id="b538a-116">string</span></span> | <span data-ttu-id="b538a-117">Имя столбца в этом типе контента.</span><span class="sxs-lookup"><span data-stu-id="b538a-117">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
