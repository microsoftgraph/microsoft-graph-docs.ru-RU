---
title: signInFrequencySessionControl type
description: Управление сеансом для обеспечения частоты подписей.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: bc5123975dc15c7c49f0dcbec507c345cf057850
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761053"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="a9221-103">signInFrequencySessionControl type</span><span class="sxs-lookup"><span data-stu-id="a9221-103">signInFrequencySessionControl resource type</span></span>

<span data-ttu-id="a9221-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9221-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9221-105">Управление сеансами для обеспечения частоты входов.</span><span class="sxs-lookup"><span data-stu-id="a9221-105">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="a9221-106">Наследуется от [управления сеансами условного доступа.](conditionalaccesssessioncontrol.md)</span><span class="sxs-lookup"><span data-stu-id="a9221-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a9221-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9221-107">Properties</span></span>

| <span data-ttu-id="a9221-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9221-108">Property</span></span>     | <span data-ttu-id="a9221-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a9221-109">Type</span></span>        | <span data-ttu-id="a9221-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a9221-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a9221-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="a9221-111">isEnabled</span></span>     |<span data-ttu-id="a9221-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9221-112">Boolean</span></span>      | <span data-ttu-id="a9221-113">Указывает, включено ли управление сеансом.</span><span class="sxs-lookup"><span data-stu-id="a9221-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="a9221-114">type</span><span class="sxs-lookup"><span data-stu-id="a9221-114">type</span></span>          |<span data-ttu-id="a9221-115">String</span><span class="sxs-lookup"><span data-stu-id="a9221-115">String</span></span>       | <span data-ttu-id="a9221-116">Возможные значения: `days`, `hours`.</span><span class="sxs-lookup"><span data-stu-id="a9221-116">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="a9221-117">value</span><span class="sxs-lookup"><span data-stu-id="a9221-117">value</span></span>         |<span data-ttu-id="a9221-118">Int32</span><span class="sxs-lookup"><span data-stu-id="a9221-118">Int32</span></span>        | <span data-ttu-id="a9221-119">Количество `days` или `hours` .</span><span class="sxs-lookup"><span data-stu-id="a9221-119">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9221-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="a9221-120">Relationships</span></span>

<span data-ttu-id="a9221-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a9221-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9221-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a9221-122">JSON representation</span></span>

<span data-ttu-id="a9221-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9221-123">The following is a JSON representation of the resource.</span></span>

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


