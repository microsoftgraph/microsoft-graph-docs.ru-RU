---
title: Тип ресурса synchronizationError
description: Представляет ошибки, возникшей во время синхронизации.
ms.openlocfilehash: a1e3725151a4e36772cd3b6079f787370f4c85dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075585"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="fb914-103">Тип ресурса synchronizationError</span><span class="sxs-lookup"><span data-stu-id="fb914-103">synchronizationError resource type</span></span>

> <span data-ttu-id="fb914-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fb914-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb914-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb914-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fb914-106">Представляет ошибки, возникшей во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="fb914-106">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="fb914-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb914-107">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="fb914-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb914-108">Property</span></span>     | <span data-ttu-id="fb914-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fb914-109">Type</span></span>   |<span data-ttu-id="fb914-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fb914-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb914-111">code</span><span class="sxs-lookup"><span data-stu-id="fb914-111">code</span></span>|<span data-ttu-id="fb914-112">String</span><span class="sxs-lookup"><span data-stu-id="fb914-112">String</span></span>||
|<span data-ttu-id="fb914-113">message</span><span class="sxs-lookup"><span data-stu-id="fb914-113">message</span></span>|<span data-ttu-id="fb914-114">String</span><span class="sxs-lookup"><span data-stu-id="fb914-114">String</span></span>||
|<span data-ttu-id="fb914-115">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="fb914-115">tenantActionable</span></span>|<span data-ttu-id="fb914-116">Логический</span><span class="sxs-lookup"><span data-stu-id="fb914-116">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="fb914-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb914-117">JSON representation</span></span>

<span data-ttu-id="fb914-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb914-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationError"
}-->

```json
{
  "code": "String",
  "message": "String",
  "tenantActionable": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->