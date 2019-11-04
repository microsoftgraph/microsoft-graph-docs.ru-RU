---
title: Тип ресурса Фаллбаккполиципропертиес
description: 'Позволяет указать резервную политику для необработанных уведомлений с высоким приоритетом для необработанных конечных точек iOS, с дополнительными свойствами для указания времени ожидания (задержки) и соответствующим визуальным содержимым уведомления. '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: a3ce59a23b5aec6dd43b370c3b67e9439b11937e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938964"
---
# <a name="fallbackpolicyproperties-resource-type"></a><span data-ttu-id="6fabd-103">Тип ресурса Фаллбаккполиципропертиес</span><span class="sxs-lookup"><span data-stu-id="6fabd-103">fallbackPolicyProperties resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fabd-104">Позволяет указать резервную политику для необработанных уведомлений с высоким приоритетом для необработанных конечных точек iOS, с дополнительными свойствами для указания времени ожидания (задержки) и соответствующим визуальным содержимым уведомления.</span><span class="sxs-lookup"><span data-stu-id="6fabd-104">Allows fallback policy to be specified for high-priority raw notifications on iOS endpoints only, with additional properties for specifying fallback wait time (delay) and corresponding visual notification content.</span></span> 

## <a name="properties"></a><span data-ttu-id="6fabd-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6fabd-105">Properties</span></span>

| <span data-ttu-id="6fabd-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fabd-106">Property</span></span>     | <span data-ttu-id="6fabd-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6fabd-107">Type</span></span>        | <span data-ttu-id="6fabd-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6fabd-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6fabd-109">платформтипес</span><span class="sxs-lookup"><span data-stu-id="6fabd-109">platformTypes</span></span> | <span data-ttu-id="6fabd-110">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6fabd-110">String collection</span></span> | <span data-ttu-id="6fabd-111">Задает платформы, на которых разработчику необходимо включить резервное уведомление с необработанным всплывающим уведомлением.</span><span class="sxs-lookup"><span data-stu-id="6fabd-111">Specifies the platforms that a developer wants to enable raw-to-visual toast notification fallback on.</span></span> <span data-ttu-id="6fabd-112">В настоящее время, если указан **фаллбаккполици** , **таржетполици. платформтипес** должен `iOS` включать и (необязательно) другие платформы.</span><span class="sxs-lookup"><span data-stu-id="6fabd-112">Currently, if **fallbackPolicy** is specified, **targetPolicy.platformTypes** must include `iOS` and optionally other platforms.</span></span> <span data-ttu-id="6fabd-113">Кроме того, необходимо указать **фаллбаккполици. ендпоинтфаллбакк. платформтипес** , и в настоящее время `iOS`единственная поддерживаемая платформа.</span><span class="sxs-lookup"><span data-stu-id="6fabd-113">In addition, **fallbackPolicy.endpointFallback.platformTypes** is required and the only supported platform is currently `iOS`.</span></span> |
| <span data-ttu-id="6fabd-114">фаллбаккделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="6fabd-114">fallbackDelayInSeconds</span></span> | <span data-ttu-id="6fabd-115">Int32</span><span class="sxs-lookup"><span data-stu-id="6fabd-115">Int32</span></span> | <span data-ttu-id="6fabd-116">Эта задержка представляет период времени (в секундах), по истечении которого непосредственный всплывающий уведомление будет отправлено в качестве резерва для каждой подписки на устройство iOS, которая не извлекает необработанное уведомление.</span><span class="sxs-lookup"><span data-stu-id="6fabd-116">This delay represents the amount of time that will pass (in seconds) before a direct toast notification will be sent as a fallback to each users� iOS device subscription that does not fetch the raw notification.</span></span> <span data-ttu-id="6fabd-117">Значение должно находиться в диапазоне от 60 до 600.</span><span class="sxs-lookup"><span data-stu-id="6fabd-117">The value must be between 60 and 600.</span></span> |
| <span data-ttu-id="6fabd-118">висуалконтент</span><span class="sxs-lookup"><span data-stu-id="6fabd-118">visualContent</span></span> | [<span data-ttu-id="6fabd-119">висуалпропертиес</span><span class="sxs-lookup"><span data-stu-id="6fabd-119">visualProperties</span></span>](visualproperties.md)|<span data-ttu-id="6fabd-120">Визуальное содержимое инициированной резервной системы уведомления о необработанном пользователе в iOS.</span><span class="sxs-lookup"><span data-stu-id="6fabd-120">The visual content of a fallback initiated, raw-to-visual user notification on iOS.</span></span> |
 


## <a name="json-representation"></a><span data-ttu-id="6fabd-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6fabd-121">JSON representation</span></span>

<span data-ttu-id="6fabd-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6fabd-122">The following is a JSON representation of the resource.</span></span>

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