---
title: тип ресурса termsExpiration
description: Предоставляет дополнительные параметры при настройке запланированного срока действия соглашения.
localization_priority: Normal
ms.prod: governance
author: raprakasMSFT
doc_type: resourcePageType
ms.openlocfilehash: 29489f3e225b24cc57c20826d9a6071c2a501154
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721728"
---
# <a name="termsexpiration-resource-type"></a><span data-ttu-id="1af15-103">тип ресурса termsExpiration</span><span class="sxs-lookup"><span data-stu-id="1af15-103">termsExpiration resource type</span></span>

<span data-ttu-id="1af15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1af15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1af15-105">Предоставляет дополнительные параметры при настройке запланированного срока действия соглашения.</span><span class="sxs-lookup"><span data-stu-id="1af15-105">Provides additional settings when setting the scheduled expiration of the agreement.</span></span>

## <a name="properties"></a><span data-ttu-id="1af15-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1af15-106">Properties</span></span>

| <span data-ttu-id="1af15-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1af15-107">Property</span></span>                     | <span data-ttu-id="1af15-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1af15-108">Type</span></span>                      | <span data-ttu-id="1af15-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1af15-109">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="1af15-110">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1af15-110">startDateTime</span></span>|<span data-ttu-id="1af15-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1af15-111">DateTimeOffset</span></span> | <span data-ttu-id="1af15-112">DateTime, когда срок действия соглашения истекает для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="1af15-112">The DateTime when the agreement is set to expire for all users.</span></span> <span data-ttu-id="1af15-113">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="1af15-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1af15-114">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="1af15-114">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
| <span data-ttu-id="1af15-115">частота</span><span class="sxs-lookup"><span data-stu-id="1af15-115">frequency</span></span>| <span data-ttu-id="1af15-116">Duration</span><span class="sxs-lookup"><span data-stu-id="1af15-116">Duration</span></span> | <span data-ttu-id="1af15-117">Представляет частоту, с которой срок действия терминов истекает после его первого истечения, как установлено **в startDateTime.**</span><span class="sxs-lookup"><span data-stu-id="1af15-117">Represents the frequency at which the terms will expire, after its first expiration as set in **startDateTime**.</span></span> <span data-ttu-id="1af15-118">Значение представлено в формате ISO 8601 для длительности.</span><span class="sxs-lookup"><span data-stu-id="1af15-118">The value is represented in ISO 8601 format for durations.</span></span> <span data-ttu-id="1af15-119">Например, `PT1M` представляет период времени 1 месяц.</span><span class="sxs-lookup"><span data-stu-id="1af15-119">For example, `PT1M` represents a time period of 1 month.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1af15-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1af15-120">JSON representation</span></span>

<span data-ttu-id="1af15-121">Ниже приводится представление JSON этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="1af15-121">The following is a JSON representation of this resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.termsExpiration",
}-->

```json
{
   "startDateTime": "2018-10-01T00:00:00.0000000Z",
   "frequency": "Duration"
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


