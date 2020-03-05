---
title: Тип ресурса Фаллбаккполици
description: 'Позволяет указать резервную политику только для конечных точек iOS и предназначена для использования для необработанных уведомлений с высоким приоритетом. '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 822a5d24acbec878b864c70d357f76a1fa115e4b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498576"
---
# <a name="fallbackpolicy-resource-type"></a><span data-ttu-id="999c9-103">Тип ресурса Фаллбаккполици</span><span class="sxs-lookup"><span data-stu-id="999c9-103">fallbackPolicy resource type</span></span>

<span data-ttu-id="999c9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="999c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="999c9-105">Позволяет указать резервную политику только для конечных точек iOS и предназначена для использования для необработанных уведомлений с высоким приоритетом, которые могут не доставляться на устройства из-за ограничений, определенных платформой (например, режим экономии заряда).</span><span class="sxs-lookup"><span data-stu-id="999c9-105">Allows fallback policy to be specified for iOS endpoints only and is designed to be used for high-priority raw notifications that might not be delivered to devices due to platform specific restrictions (e.g. battery saver mode).</span></span>

## <a name="properties"></a><span data-ttu-id="999c9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="999c9-106">Properties</span></span>

| <span data-ttu-id="999c9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="999c9-107">Property</span></span>     | <span data-ttu-id="999c9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="999c9-108">Type</span></span>        | <span data-ttu-id="999c9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="999c9-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="999c9-110">ендпоинтфаллбакк</span><span class="sxs-lookup"><span data-stu-id="999c9-110">endpointFallback</span></span> | [<span data-ttu-id="999c9-111">фаллбаккполиципропертиес</span><span class="sxs-lookup"><span data-stu-id="999c9-111">fallbackPolicyProperties</span></span>](fallbackpolicyproperties.md) | <span data-ttu-id="999c9-112">Объект политики Ендпоинтфаллбакк обрабатывает политику резервного использования уведомлений на уровне конечной точки и в настоящее время ограничивается iOS.</span><span class="sxs-lookup"><span data-stu-id="999c9-112">EndpointFallback policy object handles notification fallback policy at an end point level and is currently limited to iOS.</span></span> |   


## <a name="json-representation"></a><span data-ttu-id="999c9-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="999c9-113">JSON representation</span></span>

<span data-ttu-id="999c9-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="999c9-114">The following is a JSON representation of the resource.</span></span>

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
