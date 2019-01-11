---
title: Тип ресурса mentionsPreview
description: Представляет сведения об объектах упоминаются в экземпляре ресурсов.
localization_priority: Normal
ms.openlocfilehash: 1534b7f0ef48a80d0faaaa09880b91cb270e8eca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826112"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="7fb24-103">Тип ресурса mentionsPreview</span><span class="sxs-lookup"><span data-stu-id="7fb24-103">mentionsPreview resource type</span></span>

> <span data-ttu-id="7fb24-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7fb24-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fb24-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fb24-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7fb24-106">Представляет сведения о [упомянуть](../resources/mention.md) объекты в экземпляре ресурсов.</span><span class="sxs-lookup"><span data-stu-id="7fb24-106">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="7fb24-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7fb24-107">Properties</span></span>
| <span data-ttu-id="7fb24-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7fb24-108">Property</span></span>     | <span data-ttu-id="7fb24-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7fb24-109">Type</span></span>   |<span data-ttu-id="7fb24-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7fb24-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7fb24-111">isMentioned</span><span class="sxs-lookup"><span data-stu-id="7fb24-111">isMentioned</span></span> | <span data-ttu-id="7fb24-112">Логический</span><span class="sxs-lookup"><span data-stu-id="7fb24-112">Boolean</span></span> | <span data-ttu-id="7fb24-113">Значение true, если пользователь выполнил вход упоминается в экземпляре ресурсов родительского.</span><span class="sxs-lookup"><span data-stu-id="7fb24-113">True if the signed-in user is mentioned in the parent resource instance.</span></span> <span data-ttu-id="7fb24-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7fb24-114">Read-only.</span></span> <span data-ttu-id="7fb24-115">Поддержка фильтра.</span><span class="sxs-lookup"><span data-stu-id="7fb24-115">Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7fb24-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7fb24-116">JSON representation</span></span>

<span data-ttu-id="7fb24-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7fb24-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mentionsPreview"
}-->

```json
{
  "isMentioned": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mentionsPreview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
