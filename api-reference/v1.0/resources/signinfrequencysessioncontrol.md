---
title: signInFrequencySessionControl type
description: Управление сеансом для обеспечения частоты подписей.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 15255f44971694ff2b815e8f49e1800b91502af3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961932"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="f3dc6-103">signInFrequencySessionControl type</span><span class="sxs-lookup"><span data-stu-id="f3dc6-103">signInFrequencySessionControl resource type</span></span>

<span data-ttu-id="f3dc6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3dc6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f3dc6-105">Управление сеансами для обеспечения частоты входов.</span><span class="sxs-lookup"><span data-stu-id="f3dc6-105">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="f3dc6-106">Наследуется от [управления сеансами условного доступа.](conditionalaccesssessioncontrol.md)</span><span class="sxs-lookup"><span data-stu-id="f3dc6-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f3dc6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3dc6-107">Properties</span></span>

| <span data-ttu-id="f3dc6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3dc6-108">Property</span></span>     | <span data-ttu-id="f3dc6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f3dc6-109">Type</span></span>        | <span data-ttu-id="f3dc6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f3dc6-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f3dc6-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="f3dc6-111">isEnabled</span></span>     |<span data-ttu-id="f3dc6-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3dc6-112">Boolean</span></span>      | <span data-ttu-id="f3dc6-113">Указывает, включено ли управление сеансом.</span><span class="sxs-lookup"><span data-stu-id="f3dc6-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="f3dc6-114">type</span><span class="sxs-lookup"><span data-stu-id="f3dc6-114">type</span></span>          |<span data-ttu-id="f3dc6-115">signinFrequencyType</span><span class="sxs-lookup"><span data-stu-id="f3dc6-115">signinFrequencyType</span></span>| <span data-ttu-id="f3dc6-116">Возможные значения: `days`, `hours`.</span><span class="sxs-lookup"><span data-stu-id="f3dc6-116">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="f3dc6-117">value</span><span class="sxs-lookup"><span data-stu-id="f3dc6-117">value</span></span>         |<span data-ttu-id="f3dc6-118">Int32</span><span class="sxs-lookup"><span data-stu-id="f3dc6-118">Int32</span></span>        | <span data-ttu-id="f3dc6-119">Количество `days` или `hours` .</span><span class="sxs-lookup"><span data-stu-id="f3dc6-119">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3dc6-120">Связи</span><span class="sxs-lookup"><span data-stu-id="f3dc6-120">Relationships</span></span>

<span data-ttu-id="f3dc6-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f3dc6-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3dc6-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f3dc6-122">JSON representation</span></span>

<span data-ttu-id="f3dc6-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3dc6-123">The following is a JSON representation of the resource.</span></span>

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

