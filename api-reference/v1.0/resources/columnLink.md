---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: columnLink
ms.openlocfilehash: ef7fef6fb6ca35f1117433b452de0841691282a0
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="4f51f-102">Тип ресурса columnLink</span><span class="sxs-lookup"><span data-stu-id="4f51f-102">ColumnLink resource type</span></span>

<span data-ttu-id="4f51f-103">Ресурс **columnLink** для объекта [contentType][] связывает ресурс **columnDefinition** сайта с соответствующим типом контента.</span><span class="sxs-lookup"><span data-stu-id="4f51f-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contentType.md

## <a name="json-representation"></a><span data-ttu-id="4f51f-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4f51f-105">JSON representation</span></span>

<span data-ttu-id="4f51f-106">Ниже показано представление ресурса **columnLink** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f51f-106">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="4f51f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f51f-107">Properties</span></span>

| <span data-ttu-id="4f51f-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="4f51f-108">Property name</span></span> | <span data-ttu-id="4f51f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4f51f-109">Type</span></span>   | <span data-ttu-id="4f51f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4f51f-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="4f51f-111">**id**</span><span class="sxs-lookup"><span data-stu-id="4f51f-111">**id**</span></span>        | <span data-ttu-id="4f51f-112">строка</span><span class="sxs-lookup"><span data-stu-id="4f51f-112">string</span></span> | <span data-ttu-id="4f51f-113">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="4f51f-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="4f51f-114">**name**</span><span class="sxs-lookup"><span data-stu-id="4f51f-114">**name**</span></span>      | <span data-ttu-id="4f51f-115">строка</span><span class="sxs-lookup"><span data-stu-id="4f51f-115">string</span></span> | <span data-ttu-id="4f51f-116">Имя столбца в этом типе контента.</span><span class="sxs-lookup"><span data-stu-id="4f51f-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
