---
title: Тип ресурса Аппликатионенфорцедрестриктионссессионконтрол
description: Управление сеансами для применения ограничений приложений.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d29f26ece4ae94562dd1e16c4b9f27c77c142fa1
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638528"
---
# <a name="applicationenforcedrestrictionssessioncontrol-resource-type"></a><span data-ttu-id="73902-103">Тип ресурса Аппликатионенфорцедрестриктионссессионконтрол</span><span class="sxs-lookup"><span data-stu-id="73902-103">applicationEnforcedRestrictionsSessionControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73902-104">Управление сеансами для применения ограничений приложений.</span><span class="sxs-lookup"><span data-stu-id="73902-104">Session control to enforce application restrictions.</span></span> <span data-ttu-id="73902-105">Инехритс из [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="73902-105">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="73902-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="73902-106">Properties</span></span>

| <span data-ttu-id="73902-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="73902-107">Property</span></span>     | <span data-ttu-id="73902-108">Тип</span><span class="sxs-lookup"><span data-stu-id="73902-108">Type</span></span>        | <span data-ttu-id="73902-109">Описание</span><span class="sxs-lookup"><span data-stu-id="73902-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="73902-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="73902-110">isEnabled</span></span>     |<span data-ttu-id="73902-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="73902-111">Boolean</span></span>      | <span data-ttu-id="73902-112">Указывает, включен ли элемент управления сеансом.</span><span class="sxs-lookup"><span data-stu-id="73902-112">Specifies whether the session control is enabled or not.</span></span> |

## <a name="relationships"></a><span data-ttu-id="73902-113">Связи</span><span class="sxs-lookup"><span data-stu-id="73902-113">Relationships</span></span>

<span data-ttu-id="73902-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="73902-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="73902-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="73902-115">JSON representation</span></span>

<span data-ttu-id="73902-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73902-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationEnforcedRestrictionsSessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationEnforcedRestrictionsSessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
