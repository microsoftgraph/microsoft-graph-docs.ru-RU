---
title: Тип ресурса Термсекспиратион
description: Предоставляет дополнительные параметры при настройке запланированного срока действия соглашения.
localization_priority: Normal
ms.prod: microsoft-identity-platform
author: raprakasMSFT
doc_type: resourcePageType
ms.openlocfilehash: b3b5de1d52c4a3abb1eee7d7199a539795ba1ac3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026105"
---
# <a name="termsexpiration-resource-type"></a><span data-ttu-id="720bf-103">Тип ресурса Термсекспиратион</span><span class="sxs-lookup"><span data-stu-id="720bf-103">termsExpiration resource type</span></span>

<span data-ttu-id="720bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="720bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="720bf-105">Предоставляет дополнительные параметры при настройке запланированного срока действия соглашения.</span><span class="sxs-lookup"><span data-stu-id="720bf-105">Provides additional settings when setting the scheduled expiration of the agreement.</span></span>

## <a name="properties"></a><span data-ttu-id="720bf-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="720bf-106">Properties</span></span>

| <span data-ttu-id="720bf-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="720bf-107">Property</span></span>                     | <span data-ttu-id="720bf-108">Тип</span><span class="sxs-lookup"><span data-stu-id="720bf-108">Type</span></span>                      | <span data-ttu-id="720bf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="720bf-109">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="720bf-110">startDateTime</span><span class="sxs-lookup"><span data-stu-id="720bf-110">startDateTime</span></span>|<span data-ttu-id="720bf-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="720bf-111">DateTimeOffset</span></span> | <span data-ttu-id="720bf-112">Дата и время истечения срока действия соглашения для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="720bf-112">The DateTime when the agreement is set to expire for all users.</span></span> <span data-ttu-id="720bf-113">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="720bf-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="720bf-114">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="720bf-114">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
| <span data-ttu-id="720bf-115">повторяем</span><span class="sxs-lookup"><span data-stu-id="720bf-115">frequency</span></span>| <span data-ttu-id="720bf-116">Длительность</span><span class="sxs-lookup"><span data-stu-id="720bf-116">Duration</span></span> | <span data-ttu-id="720bf-117">Представляет частоту, с которой истекает срок действия терминов, после его первого истечения срока действия, как задано в "startDateTime".</span><span class="sxs-lookup"><span data-stu-id="720bf-117">This represents the frequency at which the terms will expire, after its first expiration as set in 'startDateTime'.</span></span> <span data-ttu-id="720bf-118">Значение представляется в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="720bf-118">The value is represented in ISO 8601 format for durations.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="720bf-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="720bf-119">JSON representation</span></span>

<span data-ttu-id="720bf-120">Ниже представлено представление этого ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="720bf-120">The following is a JSON representation of this resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.termsExpiration",
  "baseType": ""
}-->

```json
{
   "startDateTime": "2018-10-01T00:00:00.0000000Z",
   "frequency": ""
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "termsExpiration complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


