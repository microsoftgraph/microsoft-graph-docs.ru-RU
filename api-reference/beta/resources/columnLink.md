---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: columnLink
localization_priority: Normal
ms.openlocfilehash: d5b1d068202057bc6a07982d04ff77b6bf07f028
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543471"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="a00ac-102">Тип ресурса ColumnLink</span><span class="sxs-lookup"><span data-stu-id="a00ac-102">ColumnLink resource type</span></span>

<span data-ttu-id="a00ac-103">Ресурс **columnLink** для объекта [contentType][] связывает ресурс **columnDefinition** сайта с соответствующим типом контента.</span><span class="sxs-lookup"><span data-stu-id="a00ac-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="a00ac-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a00ac-105">JSON representation</span></span>

<span data-ttu-id="a00ac-106">Ниже показано представление ресурса **columnLink** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a00ac-106">Here is a JSON representation of a **columnLink** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="a00ac-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a00ac-107">Properties</span></span>

| <span data-ttu-id="a00ac-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="a00ac-108">Property name</span></span> | <span data-ttu-id="a00ac-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a00ac-109">Type</span></span>   | <span data-ttu-id="a00ac-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a00ac-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="a00ac-111">**id**</span><span class="sxs-lookup"><span data-stu-id="a00ac-111">**id**</span></span>        | <span data-ttu-id="a00ac-112">string</span><span class="sxs-lookup"><span data-stu-id="a00ac-112">string</span></span> | <span data-ttu-id="a00ac-113">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="a00ac-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="a00ac-114">**name**</span><span class="sxs-lookup"><span data-stu-id="a00ac-114">**name**</span></span>      | <span data-ttu-id="a00ac-115">string</span><span class="sxs-lookup"><span data-stu-id="a00ac-115">string</span></span> | <span data-ttu-id="a00ac-116">Имя столбца в этом типе контента.</span><span class="sxs-lookup"><span data-stu-id="a00ac-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
