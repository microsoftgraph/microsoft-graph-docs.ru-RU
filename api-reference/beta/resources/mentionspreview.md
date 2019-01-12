---
title: Тип ресурса mentionsPreview
description: Представляет сведения об объектах упоминаются в экземпляре ресурсов.
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 3bb087f6eb1d3c49b85213acf60393346a42b7cf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949292"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="19e94-103">Тип ресурса mentionsPreview</span><span class="sxs-lookup"><span data-stu-id="19e94-103">mentionsPreview resource type</span></span>

> <span data-ttu-id="19e94-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="19e94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19e94-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19e94-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19e94-106">Представляет сведения о [упомянуть](../resources/mention.md) объекты в экземпляре ресурсов.</span><span class="sxs-lookup"><span data-stu-id="19e94-106">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="19e94-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="19e94-107">Properties</span></span>
| <span data-ttu-id="19e94-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="19e94-108">Property</span></span>     | <span data-ttu-id="19e94-109">Тип</span><span class="sxs-lookup"><span data-stu-id="19e94-109">Type</span></span>   |<span data-ttu-id="19e94-110">Описание</span><span class="sxs-lookup"><span data-stu-id="19e94-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="19e94-111">isMentioned</span><span class="sxs-lookup"><span data-stu-id="19e94-111">isMentioned</span></span> | <span data-ttu-id="19e94-112">Логический</span><span class="sxs-lookup"><span data-stu-id="19e94-112">Boolean</span></span> | <span data-ttu-id="19e94-113">Значение true, если пользователь выполнил вход упоминается в экземпляре ресурсов родительского.</span><span class="sxs-lookup"><span data-stu-id="19e94-113">True if the signed-in user is mentioned in the parent resource instance.</span></span> <span data-ttu-id="19e94-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19e94-114">Read-only.</span></span> <span data-ttu-id="19e94-115">Поддержка фильтра.</span><span class="sxs-lookup"><span data-stu-id="19e94-115">Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="19e94-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19e94-116">JSON representation</span></span>

<span data-ttu-id="19e94-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19e94-117">Here is a JSON representation of the resource.</span></span>

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
