---
title: Тип ресурса Фаллбаккполици
description: 'Позволяет указать резервную политику только для конечных точек iOS и предназначена для использования для необработанных уведомлений с высоким приоритетом. '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: d9f3f545c8566d4fe363e4dfabaa41f382a96a59
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938971"
---
# <a name="fallbackpolicy-resource-type"></a><span data-ttu-id="6d4ee-103">Тип ресурса Фаллбаккполици</span><span class="sxs-lookup"><span data-stu-id="6d4ee-103">fallbackPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d4ee-104">Позволяет указать резервную политику только для конечных точек iOS и предназначена для использования для необработанных уведомлений с высоким приоритетом, которые могут не доставляться на устройства из-за ограничений, определенных платформой (например, режим экономии заряда).</span><span class="sxs-lookup"><span data-stu-id="6d4ee-104">Allows fallback policy to be specified for iOS endpoints only and is designed to be used for high-priority raw notifications that might not be delivered to devices due to platform specific restrictions (e.g. battery saver mode).</span></span>

## <a name="properties"></a><span data-ttu-id="6d4ee-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d4ee-105">Properties</span></span>

| <span data-ttu-id="6d4ee-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d4ee-106">Property</span></span>     | <span data-ttu-id="6d4ee-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6d4ee-107">Type</span></span>        | <span data-ttu-id="6d4ee-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6d4ee-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6d4ee-109">ендпоинтфаллбакк</span><span class="sxs-lookup"><span data-stu-id="6d4ee-109">endpointFallback</span></span> | [<span data-ttu-id="6d4ee-110">фаллбаккполиципропертиес</span><span class="sxs-lookup"><span data-stu-id="6d4ee-110">fallbackPolicyProperties</span></span>](fallbackpolicyproperties.md) | <span data-ttu-id="6d4ee-111">Объект политики Ендпоинтфаллбакк обрабатывает политику резервного использования уведомлений на уровне конечной точки и в настоящее время ограничивается iOS.</span><span class="sxs-lookup"><span data-stu-id="6d4ee-111">EndpointFallback policy object handles notification fallback policy at an end point level and is currently limited to iOS.</span></span> |   


## <a name="json-representation"></a><span data-ttu-id="6d4ee-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d4ee-112">JSON representation</span></span>

<span data-ttu-id="6d4ee-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d4ee-113">The following is a JSON representation of the resource.</span></span>

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
