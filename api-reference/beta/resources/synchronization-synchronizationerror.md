---
title: Тип ресурса synchronizationError
description: Представляет ошибку, которая произошла в процессе синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: a49f2cf9b9d3e621533490127a5b2674ab43bf14
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131490"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="626bc-103">Тип ресурса synchronizationError</span><span class="sxs-lookup"><span data-stu-id="626bc-103">synchronizationError resource type</span></span>

<span data-ttu-id="626bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="626bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="626bc-105">Представляет ошибку, которая произошла в процессе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="626bc-105">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="626bc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="626bc-106">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="626bc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="626bc-107">Property</span></span>     | <span data-ttu-id="626bc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="626bc-108">Type</span></span>   |<span data-ttu-id="626bc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="626bc-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="626bc-110">code</span><span class="sxs-lookup"><span data-stu-id="626bc-110">code</span></span>|<span data-ttu-id="626bc-111">Строка</span><span class="sxs-lookup"><span data-stu-id="626bc-111">String</span></span>||
|<span data-ttu-id="626bc-112">message</span><span class="sxs-lookup"><span data-stu-id="626bc-112">message</span></span>|<span data-ttu-id="626bc-113">String</span><span class="sxs-lookup"><span data-stu-id="626bc-113">String</span></span>||
|<span data-ttu-id="626bc-114">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="626bc-114">tenantActionable</span></span>|<span data-ttu-id="626bc-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="626bc-115">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="626bc-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="626bc-116">JSON representation</span></span>

<span data-ttu-id="626bc-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="626bc-117">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


