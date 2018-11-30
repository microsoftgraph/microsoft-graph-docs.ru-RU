---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: columnLink
ms.openlocfilehash: edb8d97094b4d26dbbcc008664bf5dfee3a4ddf9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076143"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="dbbc7-102">Тип ресурса ColumnLink</span><span class="sxs-lookup"><span data-stu-id="dbbc7-102">ColumnLink resource type</span></span>

> <span data-ttu-id="dbbc7-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dbbc7-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbbc7-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbbc7-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dbbc7-105">Ресурс **columnLink** для объекта [contentType][] связывает ресурс **columnDefinition** сайта с соответствующим типом контента.</span><span class="sxs-lookup"><span data-stu-id="dbbc7-105">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="dbbc7-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="dbbc7-107">JSON representation</span></span>

<span data-ttu-id="dbbc7-108">Ниже показано представление ресурса **columnLink** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dbbc7-108">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="dbbc7-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="dbbc7-109">Properties</span></span>

| <span data-ttu-id="dbbc7-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="dbbc7-110">Property name</span></span> | <span data-ttu-id="dbbc7-111">Тип</span><span class="sxs-lookup"><span data-stu-id="dbbc7-111">Type</span></span>   | <span data-ttu-id="dbbc7-112">Описание</span><span class="sxs-lookup"><span data-stu-id="dbbc7-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="dbbc7-113">**id**</span><span class="sxs-lookup"><span data-stu-id="dbbc7-113">**id**</span></span>        | <span data-ttu-id="dbbc7-114">строка</span><span class="sxs-lookup"><span data-stu-id="dbbc7-114">string</span></span> | <span data-ttu-id="dbbc7-115">Уникальный идентификатор столбца.</span><span class="sxs-lookup"><span data-stu-id="dbbc7-115">The unique identifier for the column.</span></span>
| <span data-ttu-id="dbbc7-116">**name**</span><span class="sxs-lookup"><span data-stu-id="dbbc7-116">**name**</span></span>      | <span data-ttu-id="dbbc7-117">строка</span><span class="sxs-lookup"><span data-stu-id="dbbc7-117">string</span></span> | <span data-ttu-id="dbbc7-118">Имя столбца в этом типе контента.</span><span class="sxs-lookup"><span data-stu-id="dbbc7-118">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
