---
title: Тип ресурса Сигнинфрекуенцисессионконтрол
description: Управление сеансами для применения частоты входа.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8095469ddb29c79be3a22b84e58d7e4e52cd8d5c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067160"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="feb6c-103">Тип ресурса Сигнинфрекуенцисессионконтрол</span><span class="sxs-lookup"><span data-stu-id="feb6c-103">signInFrequencySessionControl resource type</span></span>

<span data-ttu-id="feb6c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="feb6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="feb6c-105">Управление сеансами для обеспечения частоты входа.</span><span class="sxs-lookup"><span data-stu-id="feb6c-105">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="feb6c-106">Наследуется от [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="feb6c-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="feb6c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="feb6c-107">Properties</span></span>

| <span data-ttu-id="feb6c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="feb6c-108">Property</span></span>     | <span data-ttu-id="feb6c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="feb6c-109">Type</span></span>        | <span data-ttu-id="feb6c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="feb6c-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="feb6c-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="feb6c-111">isEnabled</span></span>     |<span data-ttu-id="feb6c-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="feb6c-112">Boolean</span></span>      | <span data-ttu-id="feb6c-113">Указывает, включен ли элемент управления сеансом.</span><span class="sxs-lookup"><span data-stu-id="feb6c-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="feb6c-114">type</span><span class="sxs-lookup"><span data-stu-id="feb6c-114">type</span></span>          |<span data-ttu-id="feb6c-115">String</span><span class="sxs-lookup"><span data-stu-id="feb6c-115">String</span></span>       | <span data-ttu-id="feb6c-116">Возможные значения: `days`, `hours`.</span><span class="sxs-lookup"><span data-stu-id="feb6c-116">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="feb6c-117">value</span><span class="sxs-lookup"><span data-stu-id="feb6c-117">value</span></span>         |<span data-ttu-id="feb6c-118">Int32</span><span class="sxs-lookup"><span data-stu-id="feb6c-118">Int32</span></span>        | <span data-ttu-id="feb6c-119">Количество `days` или `hours` .</span><span class="sxs-lookup"><span data-stu-id="feb6c-119">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="feb6c-120">Связи</span><span class="sxs-lookup"><span data-stu-id="feb6c-120">Relationships</span></span>

<span data-ttu-id="feb6c-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="feb6c-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="feb6c-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="feb6c-122">JSON representation</span></span>

<span data-ttu-id="feb6c-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="feb6c-123">The following is a JSON representation of the resource.</span></span>

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


