---
title: Тип ресурса Сигнинфрекуенцисессионконтрол
description: Управление сеансами для применения частоты входа.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 282c96bb9030f066aadbf0515ec0466da62c502f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466041"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="b9141-103">Тип ресурса Сигнинфрекуенцисессионконтрол</span><span class="sxs-lookup"><span data-stu-id="b9141-103">signInFrequencySessionControl resource type</span></span>

<span data-ttu-id="b9141-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9141-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9141-105">Управление сеансами для обеспечения частоты входа.</span><span class="sxs-lookup"><span data-stu-id="b9141-105">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="b9141-106">Инехритс из [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="b9141-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b9141-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9141-107">Properties</span></span>

| <span data-ttu-id="b9141-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9141-108">Property</span></span>     | <span data-ttu-id="b9141-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b9141-109">Type</span></span>        | <span data-ttu-id="b9141-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b9141-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b9141-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b9141-111">isEnabled</span></span>     |<span data-ttu-id="b9141-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9141-112">Boolean</span></span>      | <span data-ttu-id="b9141-113">Указывает, включен ли элемент управления сеансом.</span><span class="sxs-lookup"><span data-stu-id="b9141-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="b9141-114">type</span><span class="sxs-lookup"><span data-stu-id="b9141-114">type</span></span>          |<span data-ttu-id="b9141-115">String</span><span class="sxs-lookup"><span data-stu-id="b9141-115">String</span></span>       | <span data-ttu-id="b9141-116">Возможные значения: `days`, `hours`.</span><span class="sxs-lookup"><span data-stu-id="b9141-116">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="b9141-117">value</span><span class="sxs-lookup"><span data-stu-id="b9141-117">value</span></span>         |<span data-ttu-id="b9141-118">Int32</span><span class="sxs-lookup"><span data-stu-id="b9141-118">Int32</span></span>        | <span data-ttu-id="b9141-119">Количество `days` или `hours`.</span><span class="sxs-lookup"><span data-stu-id="b9141-119">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9141-120">Связи</span><span class="sxs-lookup"><span data-stu-id="b9141-120">Relationships</span></span>

<span data-ttu-id="b9141-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b9141-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9141-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b9141-122">JSON representation</span></span>

<span data-ttu-id="b9141-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9141-123">The following is a JSON representation of the resource.</span></span>

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