---
title: Тип ресурса Сигнинфрекуенцисессионконтрол
description: Управление сеансами для применения частоты входа.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f53fd9f930beaaf6812a18725441e1cd338b2e6d
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434993"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="b9d75-103">Тип ресурса Сигнинфрекуенцисессионконтрол</span><span class="sxs-lookup"><span data-stu-id="b9d75-103">signInFrequencySessionControl resource type</span></span>

<span data-ttu-id="b9d75-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9d75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9d75-105">Управление сеансами для обеспечения частоты входа.</span><span class="sxs-lookup"><span data-stu-id="b9d75-105">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="b9d75-106">Наследуется от [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="b9d75-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b9d75-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9d75-107">Properties</span></span>

| <span data-ttu-id="b9d75-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9d75-108">Property</span></span>     | <span data-ttu-id="b9d75-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b9d75-109">Type</span></span>        | <span data-ttu-id="b9d75-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b9d75-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b9d75-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b9d75-111">isEnabled</span></span>     |<span data-ttu-id="b9d75-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9d75-112">Boolean</span></span>      | <span data-ttu-id="b9d75-113">Указывает, включен ли элемент управления сеансом.</span><span class="sxs-lookup"><span data-stu-id="b9d75-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="b9d75-114">type</span><span class="sxs-lookup"><span data-stu-id="b9d75-114">type</span></span>          |<span data-ttu-id="b9d75-115">String</span><span class="sxs-lookup"><span data-stu-id="b9d75-115">String</span></span>       | <span data-ttu-id="b9d75-116">Возможные значения: `days`, `hours`.</span><span class="sxs-lookup"><span data-stu-id="b9d75-116">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="b9d75-117">value</span><span class="sxs-lookup"><span data-stu-id="b9d75-117">value</span></span>         |<span data-ttu-id="b9d75-118">Int32</span><span class="sxs-lookup"><span data-stu-id="b9d75-118">Int32</span></span>        | <span data-ttu-id="b9d75-119">Количество `days` или `hours` .</span><span class="sxs-lookup"><span data-stu-id="b9d75-119">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9d75-120">Связи</span><span class="sxs-lookup"><span data-stu-id="b9d75-120">Relationships</span></span>

<span data-ttu-id="b9d75-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b9d75-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9d75-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b9d75-122">JSON representation</span></span>

<span data-ttu-id="b9d75-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9d75-123">The following is a JSON representation of the resource.</span></span>

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
