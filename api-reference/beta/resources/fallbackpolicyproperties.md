---
title: Тип ресурса Фаллбаккполиципропертиес
description: 'Позволяет указать резервную политику для необработанных уведомлений с высоким приоритетом для необработанных конечных точек iOS, с дополнительными свойствами для указания времени ожидания (задержки) и соответствующим визуальным содержимым уведомления. '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: ee32b40f71c2540bb06b8b4478d0f896aac40b85
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071219"
---
# <a name="fallbackpolicyproperties-resource-type"></a><span data-ttu-id="63570-103">Тип ресурса Фаллбаккполиципропертиес</span><span class="sxs-lookup"><span data-stu-id="63570-103">fallbackPolicyProperties resource type</span></span>

<span data-ttu-id="63570-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63570-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63570-105">Позволяет указать резервную политику для необработанных уведомлений с высоким приоритетом для необработанных конечных точек iOS, с дополнительными свойствами для указания времени ожидания (задержки) и соответствующим визуальным содержимым уведомления.</span><span class="sxs-lookup"><span data-stu-id="63570-105">Allows fallback policy to be specified for high-priority raw notifications on iOS endpoints only, with additional properties for specifying fallback wait time (delay) and corresponding visual notification content.</span></span> 

## <a name="properties"></a><span data-ttu-id="63570-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="63570-106">Properties</span></span>

| <span data-ttu-id="63570-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="63570-107">Property</span></span>     | <span data-ttu-id="63570-108">Тип</span><span class="sxs-lookup"><span data-stu-id="63570-108">Type</span></span>        | <span data-ttu-id="63570-109">Описание</span><span class="sxs-lookup"><span data-stu-id="63570-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="63570-110">платформтипес</span><span class="sxs-lookup"><span data-stu-id="63570-110">platformTypes</span></span> | <span data-ttu-id="63570-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="63570-111">String collection</span></span> | <span data-ttu-id="63570-112">Задает платформы, на которых разработчику необходимо включить резервное уведомление с необработанным всплывающим уведомлением.</span><span class="sxs-lookup"><span data-stu-id="63570-112">Specifies the platforms that a developer wants to enable raw-to-visual toast notification fallback on.</span></span> <span data-ttu-id="63570-113">В настоящее время, если указан **фаллбаккполици** , **таржетполици. платформтипес** должен включать `iOS` и (необязательно) другие платформы.</span><span class="sxs-lookup"><span data-stu-id="63570-113">Currently, if **fallbackPolicy** is specified, **targetPolicy.platformTypes** must include `iOS` and optionally other platforms.</span></span> <span data-ttu-id="63570-114">Кроме того, необходимо указать **фаллбаккполици. ендпоинтфаллбакк. платформтипес** , и в настоящее время единственная поддерживаемая платформа `iOS` .</span><span class="sxs-lookup"><span data-stu-id="63570-114">In addition, **fallbackPolicy.endpointFallback.platformTypes** is required and the only supported platform is currently `iOS`.</span></span> |
| <span data-ttu-id="63570-115">фаллбаккделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="63570-115">fallbackDelayInSeconds</span></span> | <span data-ttu-id="63570-116">Int32</span><span class="sxs-lookup"><span data-stu-id="63570-116">Int32</span></span> | <span data-ttu-id="63570-117">Эта задержка представляет период времени (в секундах), по истечении которого непосредственный всплывающий уведомление будет отправлено в качестве резерва для каждой подписки на устройство iOS, которая не извлекает необработанное уведомление.</span><span class="sxs-lookup"><span data-stu-id="63570-117">This delay represents the amount of time that will pass (in seconds) before a direct toast notification will be sent as a fallback to each users� iOS device subscription that does not fetch the raw notification.</span></span> <span data-ttu-id="63570-118">Значение должно находиться в диапазоне от 60 до 600.</span><span class="sxs-lookup"><span data-stu-id="63570-118">The value must be between 60 and 600.</span></span> |
| <span data-ttu-id="63570-119">висуалконтент</span><span class="sxs-lookup"><span data-stu-id="63570-119">visualContent</span></span> | [<span data-ttu-id="63570-120">висуалпропертиес</span><span class="sxs-lookup"><span data-stu-id="63570-120">visualProperties</span></span>](visualproperties.md)|<span data-ttu-id="63570-121">Визуальное содержимое инициированной резервной системы уведомления о необработанном пользователе в iOS.</span><span class="sxs-lookup"><span data-stu-id="63570-121">The visual content of a fallback initiated, raw-to-visual user notification on iOS.</span></span> |
 


## <a name="json-representation"></a><span data-ttu-id="63570-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="63570-122">JSON representation</span></span>

<span data-ttu-id="63570-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63570-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fallbackpolicyProperties",
  "baseType": null
}-->

```json
{
  "platformTypes": ["String"],
  "fallbackDelayInSeconds": 60,
  "visualContent": {"@odata.type": "microsoft.graph.visualProperties"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fallbackpolicyProperties resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

