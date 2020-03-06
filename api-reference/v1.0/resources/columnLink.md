---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: columnLink
localization_priority: Normal
description: Ресурс columnLink для объекта contentType связывает ресурс columnDefinition сайта с соответствующим типом контента.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fe17c5baf13e24800f28af1895561d55f3bf66cd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531809"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="6c760-103">Тип ресурса ColumnLink</span><span class="sxs-lookup"><span data-stu-id="6c760-103">ColumnLink resource type</span></span>

<span data-ttu-id="6c760-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c760-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c760-105">Ресурс **columnLink** для объекта [contentType][] связывает ресурс **columnDefinition** сайта с соответствующим типом контента.</span><span class="sxs-lookup"><span data-stu-id="6c760-105">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="6c760-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6c760-107">JSON representation</span></span>

<span data-ttu-id="6c760-108">Ниже показано представление ресурса **columnLink** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c760-108">Here is a JSON representation of a **columnLink** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="6c760-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c760-109">Properties</span></span>

| <span data-ttu-id="6c760-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="6c760-110">Property name</span></span> | <span data-ttu-id="6c760-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6c760-111">Type</span></span>   | <span data-ttu-id="6c760-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6c760-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="6c760-113">**id**</span><span class="sxs-lookup"><span data-stu-id="6c760-113">**id**</span></span>        | <span data-ttu-id="6c760-114">строка</span><span class="sxs-lookup"><span data-stu-id="6c760-114">string</span></span> | <span data-ttu-id="6c760-115">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="6c760-115">The unique identifier for the column.</span></span>
| <span data-ttu-id="6c760-116">**name**</span><span class="sxs-lookup"><span data-stu-id="6c760-116">**name**</span></span>      | <span data-ttu-id="6c760-117">string</span><span class="sxs-lookup"><span data-stu-id="6c760-117">string</span></span> | <span data-ttu-id="6c760-118">Имя столбца в этом типе контента.</span><span class="sxs-lookup"><span data-stu-id="6c760-118">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
