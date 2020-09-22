---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: columnLink
localization_priority: Normal
description: Ресурс columnLink для объекта contentType связывает ресурс columnDefinition сайта с соответствующим типом контента.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4178184b1b9f2fb474783a3d017321c090c5410f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086790"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="1e0f8-103">Тип ресурса ColumnLink</span><span class="sxs-lookup"><span data-stu-id="1e0f8-103">ColumnLink resource type</span></span>

<span data-ttu-id="1e0f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e0f8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1e0f8-105">Ресурс **columnLink** для объекта [contentType][] связывает ресурс **columnDefinition** сайта с соответствующим типом контента.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-105">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="1e0f8-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1e0f8-107">JSON representation</span></span>

<span data-ttu-id="1e0f8-108">Ниже показано представление ресурса **columnLink** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-108">Here is a JSON representation of a **columnLink** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="1e0f8-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e0f8-109">Properties</span></span>

| <span data-ttu-id="1e0f8-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="1e0f8-110">Property name</span></span> | <span data-ttu-id="1e0f8-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1e0f8-111">Type</span></span>   | <span data-ttu-id="1e0f8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1e0f8-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="1e0f8-113">**id**</span><span class="sxs-lookup"><span data-stu-id="1e0f8-113">**id**</span></span>        | <span data-ttu-id="1e0f8-114">string</span><span class="sxs-lookup"><span data-stu-id="1e0f8-114">string</span></span> | <span data-ttu-id="1e0f8-115">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-115">The unique identifier for the column.</span></span>
| <span data-ttu-id="1e0f8-116">**name**</span><span class="sxs-lookup"><span data-stu-id="1e0f8-116">**name**</span></span>      | <span data-ttu-id="1e0f8-117">string</span><span class="sxs-lookup"><span data-stu-id="1e0f8-117">string</span></span> | <span data-ttu-id="1e0f8-118">Имя столбца в этом типе контента.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-118">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->

