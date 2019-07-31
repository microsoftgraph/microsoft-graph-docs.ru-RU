---
author: daspek
description: Ресурс columnLink для объекта contentType связывает ресурс columnDefinition сайта с соответствующим типом контента.
ms.date: 09/12/2017
title: columnLink
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 4add6ac0edc401815d8072371ce0faca48d5852b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012949"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="08db5-103">Тип ресурса ColumnLink</span><span class="sxs-lookup"><span data-stu-id="08db5-103">ColumnLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08db5-104">Ресурс **columnLink** для объекта [contentType][] связывает ресурс **columnDefinition** сайта с соответствующим типом контента.</span><span class="sxs-lookup"><span data-stu-id="08db5-104">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="08db5-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="08db5-106">JSON representation</span></span>

<span data-ttu-id="08db5-107">Ниже показано представление ресурса **columnLink** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08db5-107">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="08db5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="08db5-108">Properties</span></span>

| <span data-ttu-id="08db5-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="08db5-109">Property name</span></span> | <span data-ttu-id="08db5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="08db5-110">Type</span></span>   | <span data-ttu-id="08db5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="08db5-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="08db5-112">**id**</span><span class="sxs-lookup"><span data-stu-id="08db5-112">**id**</span></span>        | <span data-ttu-id="08db5-113">string</span><span class="sxs-lookup"><span data-stu-id="08db5-113">string</span></span> | <span data-ttu-id="08db5-114">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="08db5-114">The unique identifier for the column.</span></span>
| <span data-ttu-id="08db5-115">**name**</span><span class="sxs-lookup"><span data-stu-id="08db5-115">**name**</span></span>      | <span data-ttu-id="08db5-116">string</span><span class="sxs-lookup"><span data-stu-id="08db5-116">string</span></span> | <span data-ttu-id="08db5-117">Имя столбца в этом типе контента.</span><span class="sxs-lookup"><span data-stu-id="08db5-117">The name of the column  in this content type.</span></span>

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
