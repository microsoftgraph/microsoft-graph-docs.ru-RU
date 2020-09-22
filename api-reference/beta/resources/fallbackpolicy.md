---
title: Тип ресурса Фаллбаккполици
description: 'Позволяет указать резервную политику только для конечных точек iOS и предназначена для использования для необработанных уведомлений с высоким приоритетом. '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 8d39f9b69eb4ebdfcab883adec10b70100efba4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071222"
---
# <a name="fallbackpolicy-resource-type"></a><span data-ttu-id="37be6-103">Тип ресурса Фаллбаккполици</span><span class="sxs-lookup"><span data-stu-id="37be6-103">fallbackPolicy resource type</span></span>

<span data-ttu-id="37be6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37be6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37be6-105">Позволяет указать резервную политику только для конечных точек iOS и предназначена для использования для необработанных уведомлений с высоким приоритетом, которые могут не доставляться на устройства из-за ограничений, определенных платформой (например, режим экономии заряда).</span><span class="sxs-lookup"><span data-stu-id="37be6-105">Allows fallback policy to be specified for iOS endpoints only and is designed to be used for high-priority raw notifications that might not be delivered to devices due to platform specific restrictions (e.g. battery saver mode).</span></span>

## <a name="properties"></a><span data-ttu-id="37be6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="37be6-106">Properties</span></span>

| <span data-ttu-id="37be6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="37be6-107">Property</span></span>     | <span data-ttu-id="37be6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="37be6-108">Type</span></span>        | <span data-ttu-id="37be6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="37be6-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="37be6-110">ендпоинтфаллбакк</span><span class="sxs-lookup"><span data-stu-id="37be6-110">endpointFallback</span></span> | [<span data-ttu-id="37be6-111">фаллбаккполиципропертиес</span><span class="sxs-lookup"><span data-stu-id="37be6-111">fallbackpolicyProperties</span></span>](fallbackpolicyproperties.md) | <span data-ttu-id="37be6-112">Объект политики Ендпоинтфаллбакк обрабатывает политику резервного использования уведомлений на уровне конечной точки и в настоящее время ограничивается iOS.</span><span class="sxs-lookup"><span data-stu-id="37be6-112">EndpointFallback policy object handles notification fallback policy at an end point level and is currently limited to iOS.</span></span> |   


## <a name="json-representation"></a><span data-ttu-id="37be6-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37be6-113">JSON representation</span></span>

<span data-ttu-id="37be6-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37be6-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fallbackpolicy",
  "baseType": null
}-->

```json
{
  "endpointFallback": {"@odata.type": "microsoft.graph.fallbackpolicyProperties"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fallbackpolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


