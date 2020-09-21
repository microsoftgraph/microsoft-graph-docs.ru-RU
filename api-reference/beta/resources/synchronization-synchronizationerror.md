---
title: Тип ресурса Синчронизатионеррор
description: Представляет сообщение об ошибке, возникшей во время процесса синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7c32f3bc22d2357c0eca88e6f693cd958a6dd5ae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013456"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="80f5a-103">Тип ресурса Синчронизатионеррор</span><span class="sxs-lookup"><span data-stu-id="80f5a-103">synchronizationError resource type</span></span>

<span data-ttu-id="80f5a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80f5a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80f5a-105">Представляет сообщение об ошибке, возникшей во время процесса синхронизации.</span><span class="sxs-lookup"><span data-stu-id="80f5a-105">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="80f5a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="80f5a-106">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="80f5a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="80f5a-107">Property</span></span>     | <span data-ttu-id="80f5a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="80f5a-108">Type</span></span>   |<span data-ttu-id="80f5a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="80f5a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80f5a-110">code</span><span class="sxs-lookup"><span data-stu-id="80f5a-110">code</span></span>|<span data-ttu-id="80f5a-111">String</span><span class="sxs-lookup"><span data-stu-id="80f5a-111">String</span></span>||
|<span data-ttu-id="80f5a-112">message</span><span class="sxs-lookup"><span data-stu-id="80f5a-112">message</span></span>|<span data-ttu-id="80f5a-113">String</span><span class="sxs-lookup"><span data-stu-id="80f5a-113">String</span></span>||
|<span data-ttu-id="80f5a-114">тенантактионабле</span><span class="sxs-lookup"><span data-stu-id="80f5a-114">tenantActionable</span></span>|<span data-ttu-id="80f5a-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="80f5a-115">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="80f5a-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="80f5a-116">JSON representation</span></span>

<span data-ttu-id="80f5a-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80f5a-117">The following is a JSON representation of the resource.</span></span>

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


