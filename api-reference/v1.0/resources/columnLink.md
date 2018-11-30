---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: columnLink
ms.openlocfilehash: a3eae28dcd9fef3ddfba9b39103bec31ff71c9da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024464"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="47ade-102">Тип ресурса ColumnLink</span><span class="sxs-lookup"><span data-stu-id="47ade-102">ColumnLink resource type</span></span>

<span data-ttu-id="47ade-103">Ресурс **columnLink** для объекта [contentType][] связывает ресурс **columnDefinition** сайта с соответствующим типом контента.</span><span class="sxs-lookup"><span data-stu-id="47ade-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="47ade-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="47ade-105">JSON representation</span></span>

<span data-ttu-id="47ade-106">Ниже показано представление ресурса **columnLink** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47ade-106">Here is a JSON representation of a **columnLink** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="47ade-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="47ade-107">Properties</span></span>

| <span data-ttu-id="47ade-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="47ade-108">Property name</span></span> | <span data-ttu-id="47ade-109">Тип</span><span class="sxs-lookup"><span data-stu-id="47ade-109">Type</span></span>   | <span data-ttu-id="47ade-110">Описание</span><span class="sxs-lookup"><span data-stu-id="47ade-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="47ade-111">**id**</span><span class="sxs-lookup"><span data-stu-id="47ade-111">**id**</span></span>        | <span data-ttu-id="47ade-112">string</span><span class="sxs-lookup"><span data-stu-id="47ade-112">string</span></span> | <span data-ttu-id="47ade-113">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="47ade-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="47ade-114">**name**</span><span class="sxs-lookup"><span data-stu-id="47ade-114">**name**</span></span>      | <span data-ttu-id="47ade-115">string</span><span class="sxs-lookup"><span data-stu-id="47ade-115">string</span></span> | <span data-ttu-id="47ade-116">Имя столбца в этом типе контента.</span><span class="sxs-lookup"><span data-stu-id="47ade-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
