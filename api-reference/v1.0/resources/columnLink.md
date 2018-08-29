---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: columnLink
ms.openlocfilehash: cdae360afb6e626ee481a7e98ed5f90e657203b2
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265122"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="9d36b-102">Тип ресурса columnLink</span><span class="sxs-lookup"><span data-stu-id="9d36b-102">ColumnLink resource type</span></span>

<span data-ttu-id="9d36b-103">Ресурс **columnLink** для объекта [contentType][] связывает ресурс **columnDefinition** сайта с соответствующим типом контента.</span><span class="sxs-lookup"><span data-stu-id="9d36b-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contentType.md

## <a name="json-representation"></a><span data-ttu-id="9d36b-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9d36b-105">JSON representation</span></span>

<span data-ttu-id="9d36b-106">Ниже показано представление ресурса **columnLink** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d36b-106">Here is a JSON representation of a **columnLink** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="9d36b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d36b-107">Properties</span></span>

| <span data-ttu-id="9d36b-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="9d36b-108">Property name</span></span> | <span data-ttu-id="9d36b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9d36b-109">Type</span></span>   | <span data-ttu-id="9d36b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9d36b-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="9d36b-111">**id**</span><span class="sxs-lookup"><span data-stu-id="9d36b-111">**id**</span></span>        | <span data-ttu-id="9d36b-112">строка</span><span class="sxs-lookup"><span data-stu-id="9d36b-112">string</span></span> | <span data-ttu-id="9d36b-113">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="9d36b-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="9d36b-114">**name**</span><span class="sxs-lookup"><span data-stu-id="9d36b-114">**name**</span></span>      | <span data-ttu-id="9d36b-115">строка</span><span class="sxs-lookup"><span data-stu-id="9d36b-115">string</span></span> | <span data-ttu-id="9d36b-116">Имя столбца в этом типе контента.</span><span class="sxs-lookup"><span data-stu-id="9d36b-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
