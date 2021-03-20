---
title: signInFrequencySessionControl type
description: Управление сеансом для обеспечения частоты подписей.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 1f224c1e9ba72e114fd9c9bcacdd74670713837d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945629"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="e067e-103">signInFrequencySessionControl type</span><span class="sxs-lookup"><span data-stu-id="e067e-103">signInFrequencySessionControl resource type</span></span>

<span data-ttu-id="e067e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e067e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e067e-105">Управление сеансами для обеспечения частоты входов.</span><span class="sxs-lookup"><span data-stu-id="e067e-105">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="e067e-106">Наследуется от [управления сеансами условного доступа.](conditionalaccesssessioncontrol.md)</span><span class="sxs-lookup"><span data-stu-id="e067e-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e067e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e067e-107">Properties</span></span>

| <span data-ttu-id="e067e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e067e-108">Property</span></span>     | <span data-ttu-id="e067e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e067e-109">Type</span></span>        | <span data-ttu-id="e067e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e067e-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e067e-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e067e-111">isEnabled</span></span>     |<span data-ttu-id="e067e-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="e067e-112">Boolean</span></span>      | <span data-ttu-id="e067e-113">Указывает, включено ли управление сеансом.</span><span class="sxs-lookup"><span data-stu-id="e067e-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="e067e-114">type</span><span class="sxs-lookup"><span data-stu-id="e067e-114">type</span></span>          |<span data-ttu-id="e067e-115">signinFrequencyType</span><span class="sxs-lookup"><span data-stu-id="e067e-115">signinFrequencyType</span></span>       | <span data-ttu-id="e067e-116">Возможные значения: `days`, `hours`.</span><span class="sxs-lookup"><span data-stu-id="e067e-116">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="e067e-117">value</span><span class="sxs-lookup"><span data-stu-id="e067e-117">value</span></span>         |<span data-ttu-id="e067e-118">Int32</span><span class="sxs-lookup"><span data-stu-id="e067e-118">Int32</span></span>        | <span data-ttu-id="e067e-119">Количество `days` или `hours` .</span><span class="sxs-lookup"><span data-stu-id="e067e-119">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e067e-120">Связи</span><span class="sxs-lookup"><span data-stu-id="e067e-120">Relationships</span></span>

<span data-ttu-id="e067e-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e067e-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e067e-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e067e-122">JSON representation</span></span>

<span data-ttu-id="e067e-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e067e-123">The following is a JSON representation of the resource.</span></span>

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


