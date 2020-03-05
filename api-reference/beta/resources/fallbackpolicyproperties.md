---
title: Тип ресурса Фаллбаккполиципропертиес
description: 'Позволяет указать резервную политику для необработанных уведомлений с высоким приоритетом для необработанных конечных точек iOS, с дополнительными свойствами для указания времени ожидания (задержки) и соответствующим визуальным содержимым уведомления. '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 3922fc08bf30dde7daa7e01d1f810cb3e45d5d81
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498541"
---
# <a name="fallbackpolicyproperties-resource-type"></a><span data-ttu-id="04c7b-103">Тип ресурса Фаллбаккполиципропертиес</span><span class="sxs-lookup"><span data-stu-id="04c7b-103">fallbackPolicyProperties resource type</span></span>

<span data-ttu-id="04c7b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="04c7b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04c7b-105">Позволяет указать резервную политику для необработанных уведомлений с высоким приоритетом для необработанных конечных точек iOS, с дополнительными свойствами для указания времени ожидания (задержки) и соответствующим визуальным содержимым уведомления.</span><span class="sxs-lookup"><span data-stu-id="04c7b-105">Allows fallback policy to be specified for high-priority raw notifications on iOS endpoints only, with additional properties for specifying fallback wait time (delay) and corresponding visual notification content.</span></span> 

## <a name="properties"></a><span data-ttu-id="04c7b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="04c7b-106">Properties</span></span>

| <span data-ttu-id="04c7b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="04c7b-107">Property</span></span>     | <span data-ttu-id="04c7b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="04c7b-108">Type</span></span>        | <span data-ttu-id="04c7b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="04c7b-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="04c7b-110">платформтипес</span><span class="sxs-lookup"><span data-stu-id="04c7b-110">platformTypes</span></span> | <span data-ttu-id="04c7b-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="04c7b-111">String collection</span></span> | <span data-ttu-id="04c7b-112">Задает платформы, на которых разработчику необходимо включить резервное уведомление с необработанным всплывающим уведомлением.</span><span class="sxs-lookup"><span data-stu-id="04c7b-112">Specifies the platforms that a developer wants to enable raw-to-visual toast notification fallback on.</span></span> <span data-ttu-id="04c7b-113">В настоящее время, если указан **фаллбаккполици** , **таржетполици. платформтипес** должен `iOS` включать и (необязательно) другие платформы.</span><span class="sxs-lookup"><span data-stu-id="04c7b-113">Currently, if **fallbackPolicy** is specified, **targetPolicy.platformTypes** must include `iOS` and optionally other platforms.</span></span> <span data-ttu-id="04c7b-114">Кроме того, необходимо указать **фаллбаккполици. ендпоинтфаллбакк. платформтипес** , и в настоящее время `iOS`единственная поддерживаемая платформа.</span><span class="sxs-lookup"><span data-stu-id="04c7b-114">In addition, **fallbackPolicy.endpointFallback.platformTypes** is required and the only supported platform is currently `iOS`.</span></span> |
| <span data-ttu-id="04c7b-115">фаллбаккделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="04c7b-115">fallbackDelayInSeconds</span></span> | <span data-ttu-id="04c7b-116">Int32</span><span class="sxs-lookup"><span data-stu-id="04c7b-116">Int32</span></span> | <span data-ttu-id="04c7b-117">Эта задержка представляет период времени (в секундах), по истечении которого непосредственный всплывающий уведомление будет отправлено в качестве резерва для каждой подписки на устройство iOS, которая не извлекает необработанное уведомление.</span><span class="sxs-lookup"><span data-stu-id="04c7b-117">This delay represents the amount of time that will pass (in seconds) before a direct toast notification will be sent as a fallback to each users� iOS device subscription that does not fetch the raw notification.</span></span> <span data-ttu-id="04c7b-118">Значение должно находиться в диапазоне от 60 до 600.</span><span class="sxs-lookup"><span data-stu-id="04c7b-118">The value must be between 60 and 600.</span></span> |
| <span data-ttu-id="04c7b-119">висуалконтент</span><span class="sxs-lookup"><span data-stu-id="04c7b-119">visualContent</span></span> | [<span data-ttu-id="04c7b-120">висуалпропертиес</span><span class="sxs-lookup"><span data-stu-id="04c7b-120">visualProperties</span></span>](visualproperties.md)|<span data-ttu-id="04c7b-121">Визуальное содержимое инициированной резервной системы уведомления о необработанном пользователе в iOS.</span><span class="sxs-lookup"><span data-stu-id="04c7b-121">The visual content of a fallback initiated, raw-to-visual user notification on iOS.</span></span> |
 


## <a name="json-representation"></a><span data-ttu-id="04c7b-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04c7b-122">JSON representation</span></span>

<span data-ttu-id="04c7b-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04c7b-123">The following is a JSON representation of the resource.</span></span>

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