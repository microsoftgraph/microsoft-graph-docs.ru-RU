---
title: Тип ресурса synchronizationError
description: Представляет ошибки, возникшей во время синхронизации.
localization_priority: Normal
ms.openlocfilehash: cc6b58444ac56303bfd2e41f1fcae17658f6aea9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847245"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="51bc3-103">Тип ресурса synchronizationError</span><span class="sxs-lookup"><span data-stu-id="51bc3-103">synchronizationError resource type</span></span>

> <span data-ttu-id="51bc3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="51bc3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51bc3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51bc3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51bc3-106">Представляет ошибки, возникшей во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="51bc3-106">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="51bc3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="51bc3-107">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="51bc3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="51bc3-108">Property</span></span>     | <span data-ttu-id="51bc3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="51bc3-109">Type</span></span>   |<span data-ttu-id="51bc3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="51bc3-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51bc3-111">code</span><span class="sxs-lookup"><span data-stu-id="51bc3-111">code</span></span>|<span data-ttu-id="51bc3-112">Строка</span><span class="sxs-lookup"><span data-stu-id="51bc3-112">String</span></span>||
|<span data-ttu-id="51bc3-113">message</span><span class="sxs-lookup"><span data-stu-id="51bc3-113">message</span></span>|<span data-ttu-id="51bc3-114">String</span><span class="sxs-lookup"><span data-stu-id="51bc3-114">String</span></span>||
|<span data-ttu-id="51bc3-115">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="51bc3-115">tenantActionable</span></span>|<span data-ttu-id="51bc3-116">Логический</span><span class="sxs-lookup"><span data-stu-id="51bc3-116">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="51bc3-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51bc3-117">JSON representation</span></span>

<span data-ttu-id="51bc3-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51bc3-118">The following is a JSON representation of the resource.</span></span>

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
