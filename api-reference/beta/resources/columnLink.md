---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: columnLink
localization_priority: Normal
ms.openlocfilehash: c6fc12dcfaeffcb3cd4fb08a6863611ae33541d5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341441"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="f067c-102">Тип ресурса ColumnLink</span><span class="sxs-lookup"><span data-stu-id="f067c-102">ColumnLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f067c-103">Ресурс **columnLink** для объекта [contentType][] связывает ресурс **columnDefinition** сайта с соответствующим типом контента.</span><span class="sxs-lookup"><span data-stu-id="f067c-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="f067c-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f067c-105">JSON representation</span></span>

<span data-ttu-id="f067c-106">Ниже показано представление ресурса **columnLink** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f067c-106">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="f067c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f067c-107">Properties</span></span>

| <span data-ttu-id="f067c-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="f067c-108">Property name</span></span> | <span data-ttu-id="f067c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f067c-109">Type</span></span>   | <span data-ttu-id="f067c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f067c-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="f067c-111">**id**</span><span class="sxs-lookup"><span data-stu-id="f067c-111">**id**</span></span>        | <span data-ttu-id="f067c-112">string</span><span class="sxs-lookup"><span data-stu-id="f067c-112">string</span></span> | <span data-ttu-id="f067c-113">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="f067c-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="f067c-114">**name**</span><span class="sxs-lookup"><span data-stu-id="f067c-114">**name**</span></span>      | <span data-ttu-id="f067c-115">string</span><span class="sxs-lookup"><span data-stu-id="f067c-115">string</span></span> | <span data-ttu-id="f067c-116">Имя столбца в этом типе контента.</span><span class="sxs-lookup"><span data-stu-id="f067c-116">The name of the column  in this content type.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink",
  "suppressions": []
}
-->
