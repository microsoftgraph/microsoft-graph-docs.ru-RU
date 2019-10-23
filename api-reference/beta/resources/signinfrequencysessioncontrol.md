---
title: Тип ресурса Сигнинфрекуенцисессионконтрол
description: Управление сеансами для применения частоты входа.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ab4eaa619117aa350dcb28be9afd43e1aa2fbc8a
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638780"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="7d6e5-103">Тип ресурса Сигнинфрекуенцисессионконтрол</span><span class="sxs-lookup"><span data-stu-id="7d6e5-103">signInFrequencySessionControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d6e5-104">Управление сеансами для обеспечения частоты входа.</span><span class="sxs-lookup"><span data-stu-id="7d6e5-104">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="7d6e5-105">Инехритс из [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="7d6e5-105">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7d6e5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d6e5-106">Properties</span></span>

| <span data-ttu-id="7d6e5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d6e5-107">Property</span></span>     | <span data-ttu-id="7d6e5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7d6e5-108">Type</span></span>        | <span data-ttu-id="7d6e5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7d6e5-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7d6e5-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="7d6e5-110">isEnabled</span></span>     |<span data-ttu-id="7d6e5-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d6e5-111">Boolean</span></span>      | <span data-ttu-id="7d6e5-112">Указывает, включен ли элемент управления сеансом.</span><span class="sxs-lookup"><span data-stu-id="7d6e5-112">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="7d6e5-113">type</span><span class="sxs-lookup"><span data-stu-id="7d6e5-113">type</span></span>          |<span data-ttu-id="7d6e5-114">String</span><span class="sxs-lookup"><span data-stu-id="7d6e5-114">String</span></span>       | <span data-ttu-id="7d6e5-115">Возможные значения: `days`, `hours`.</span><span class="sxs-lookup"><span data-stu-id="7d6e5-115">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="7d6e5-116">value</span><span class="sxs-lookup"><span data-stu-id="7d6e5-116">value</span></span>         |<span data-ttu-id="7d6e5-117">Int32</span><span class="sxs-lookup"><span data-stu-id="7d6e5-117">Int32</span></span>        | <span data-ttu-id="7d6e5-118">Количество `days` или `hours`.</span><span class="sxs-lookup"><span data-stu-id="7d6e5-118">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d6e5-119">Связи</span><span class="sxs-lookup"><span data-stu-id="7d6e5-119">Relationships</span></span>

<span data-ttu-id="7d6e5-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7d6e5-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d6e5-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7d6e5-121">JSON representation</span></span>

<span data-ttu-id="7d6e5-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d6e5-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInFrequencySessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "type": "String",
  "value": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInFrequencySessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->