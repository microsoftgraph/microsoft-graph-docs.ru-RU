---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: columnLink
localization_priority: Normal
ms.openlocfilehash: 435696cc596f73830104ea8ec0619bf40a462d62
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834533"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="142fc-102">Тип ресурса ColumnLink</span><span class="sxs-lookup"><span data-stu-id="142fc-102">ColumnLink resource type</span></span>

<span data-ttu-id="142fc-103">Ресурс **columnLink** для объекта [contentType][] связывает ресурс **columnDefinition** сайта с соответствующим типом контента.</span><span class="sxs-lookup"><span data-stu-id="142fc-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="142fc-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="142fc-105">JSON representation</span></span>

<span data-ttu-id="142fc-106">Ниже показано представление ресурса **columnLink** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="142fc-106">Here is a JSON representation of a **columnLink** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="142fc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="142fc-107">Properties</span></span>

| <span data-ttu-id="142fc-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="142fc-108">Property name</span></span> | <span data-ttu-id="142fc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="142fc-109">Type</span></span>   | <span data-ttu-id="142fc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="142fc-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="142fc-111">**id**</span><span class="sxs-lookup"><span data-stu-id="142fc-111">**id**</span></span>        | <span data-ttu-id="142fc-112">string</span><span class="sxs-lookup"><span data-stu-id="142fc-112">string</span></span> | <span data-ttu-id="142fc-113">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="142fc-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="142fc-114">**name**</span><span class="sxs-lookup"><span data-stu-id="142fc-114">**name**</span></span>      | <span data-ttu-id="142fc-115">string</span><span class="sxs-lookup"><span data-stu-id="142fc-115">string</span></span> | <span data-ttu-id="142fc-116">Имя столбца в этом типе контента.</span><span class="sxs-lookup"><span data-stu-id="142fc-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
