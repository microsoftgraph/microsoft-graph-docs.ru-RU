---
title: Тип ресурса addIn
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 6e76b8f7981be5da9a2ac8437ff21d4a59dbbe73
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884219"
---
# <a name="addin-resource-type"></a><span data-ttu-id="03938-103">Тип ресурса addIn</span><span class="sxs-lookup"><span data-stu-id="03938-103">addIn resource type</span></span>

> <span data-ttu-id="03938-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="03938-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03938-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03938-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="03938-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03938-106">JSON representation</span></span>

<span data-ttu-id="03938-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03938-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addIn"
}-->

```json
{
  "id": "guid",
  "properties": [{"@odata.type": "microsoft.graph.keyvalue"}],
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="03938-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="03938-108">Properties</span></span>
| <span data-ttu-id="03938-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="03938-109">Property</span></span>     | <span data-ttu-id="03938-110">Тип</span><span class="sxs-lookup"><span data-stu-id="03938-110">Type</span></span>   |<span data-ttu-id="03938-111">Описание</span><span class="sxs-lookup"><span data-stu-id="03938-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03938-112">id</span><span class="sxs-lookup"><span data-stu-id="03938-112">id</span></span>|<span data-ttu-id="03938-113">Идентификатор GUID</span><span class="sxs-lookup"><span data-stu-id="03938-113">guid</span></span>||
|<span data-ttu-id="03938-114">свойства</span><span class="sxs-lookup"><span data-stu-id="03938-114">properties</span></span>|<span data-ttu-id="03938-115">Коллекция [keyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="03938-115">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="03938-116">type</span><span class="sxs-lookup"><span data-stu-id="03938-116">type</span></span>|<span data-ttu-id="03938-117">строка</span><span class="sxs-lookup"><span data-stu-id="03938-117">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
