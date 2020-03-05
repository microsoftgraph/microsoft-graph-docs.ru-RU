---
title: Тип ресурса Сигнинфрекуенцисессионконтрол
description: Управление сеансами для применения частоты входа.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e13a5d46b6dfcd24b24f93e9e9870fbe89f2ee84
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520592"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="e553a-103">Тип ресурса Сигнинфрекуенцисессионконтрол</span><span class="sxs-lookup"><span data-stu-id="e553a-103">signInFrequencySessionControl resource type</span></span>

<span data-ttu-id="e553a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e553a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e553a-105">Управление сеансами для обеспечения частоты входа.</span><span class="sxs-lookup"><span data-stu-id="e553a-105">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="e553a-106">Инехритс из [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="e553a-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e553a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e553a-107">Properties</span></span>

| <span data-ttu-id="e553a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e553a-108">Property</span></span>     | <span data-ttu-id="e553a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e553a-109">Type</span></span>        | <span data-ttu-id="e553a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e553a-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e553a-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e553a-111">isEnabled</span></span>     |<span data-ttu-id="e553a-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="e553a-112">Boolean</span></span>      | <span data-ttu-id="e553a-113">Указывает, включен ли элемент управления сеансом.</span><span class="sxs-lookup"><span data-stu-id="e553a-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="e553a-114">type</span><span class="sxs-lookup"><span data-stu-id="e553a-114">type</span></span>          |<span data-ttu-id="e553a-115">String</span><span class="sxs-lookup"><span data-stu-id="e553a-115">String</span></span>       | <span data-ttu-id="e553a-116">Возможные значения: `days`, `hours`.</span><span class="sxs-lookup"><span data-stu-id="e553a-116">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="e553a-117">value</span><span class="sxs-lookup"><span data-stu-id="e553a-117">value</span></span>         |<span data-ttu-id="e553a-118">Int32</span><span class="sxs-lookup"><span data-stu-id="e553a-118">Int32</span></span>        | <span data-ttu-id="e553a-119">Количество `days` или `hours`.</span><span class="sxs-lookup"><span data-stu-id="e553a-119">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e553a-120">Связи</span><span class="sxs-lookup"><span data-stu-id="e553a-120">Relationships</span></span>

<span data-ttu-id="e553a-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e553a-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e553a-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e553a-122">JSON representation</span></span>

<span data-ttu-id="e553a-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e553a-123">The following is a JSON representation of the resource.</span></span>

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