---
title: Тип ресурса applicationEnforcedRestrictionsSessionControl
description: Управление сеансом для применения ограничений приложений.
localization_priority: Normal
author: sureshja
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f7f20950b3773e660cfc1b0ed4fdec338546e09a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134773"
---
# <a name="applicationenforcedrestrictionssessioncontrol-resource-type"></a><span data-ttu-id="d0f8a-103">Тип ресурса applicationEnforcedRestrictionsSessionControl</span><span class="sxs-lookup"><span data-stu-id="d0f8a-103">applicationEnforcedRestrictionsSessionControl resource type</span></span>

<span data-ttu-id="d0f8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0f8a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0f8a-105">Управление сеансом для применения ограничений приложений.</span><span class="sxs-lookup"><span data-stu-id="d0f8a-105">Session control to enforce application restrictions.</span></span> <span data-ttu-id="d0f8a-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="d0f8a-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d0f8a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0f8a-107">Properties</span></span>

| <span data-ttu-id="d0f8a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0f8a-108">Property</span></span>     | <span data-ttu-id="d0f8a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d0f8a-109">Type</span></span>        | <span data-ttu-id="d0f8a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d0f8a-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d0f8a-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="d0f8a-111">isEnabled</span></span>     |<span data-ttu-id="d0f8a-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0f8a-112">Boolean</span></span>      | <span data-ttu-id="d0f8a-113">Указывает, включено ли управление сеансом.</span><span class="sxs-lookup"><span data-stu-id="d0f8a-113">Specifies whether the session control is enabled or not.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d0f8a-114">Связи</span><span class="sxs-lookup"><span data-stu-id="d0f8a-114">Relationships</span></span>

<span data-ttu-id="d0f8a-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d0f8a-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0f8a-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d0f8a-116">JSON representation</span></span>

<span data-ttu-id="d0f8a-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0f8a-117">The following is a JSON representation of the resource.</span></span>

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


