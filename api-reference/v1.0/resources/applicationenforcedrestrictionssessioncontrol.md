---
title: Тип ресурса applicationEnforcedRestrictionsSessionControl
description: Управление сеансом для применения ограничений приложений.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 130644ebf0d72b4870dc78e64455c2dfab446ae5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134969"
---
# <a name="applicationenforcedrestrictionssessioncontrol-resource-type"></a><span data-ttu-id="90d87-103">Тип ресурса applicationEnforcedRestrictionsSessionControl</span><span class="sxs-lookup"><span data-stu-id="90d87-103">applicationEnforcedRestrictionsSessionControl resource type</span></span>

<span data-ttu-id="90d87-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90d87-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="90d87-105">Управление сеансом для применения ограничений приложений.</span><span class="sxs-lookup"><span data-stu-id="90d87-105">Session control to enforce application restrictions.</span></span> <span data-ttu-id="90d87-106">Наследуется от [контроля сеанса условного доступа.](conditionalaccesssessioncontrol.md)</span><span class="sxs-lookup"><span data-stu-id="90d87-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="90d87-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="90d87-107">Properties</span></span>

| <span data-ttu-id="90d87-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="90d87-108">Property</span></span>     | <span data-ttu-id="90d87-109">Тип</span><span class="sxs-lookup"><span data-stu-id="90d87-109">Type</span></span>        | <span data-ttu-id="90d87-110">Описание</span><span class="sxs-lookup"><span data-stu-id="90d87-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="90d87-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="90d87-111">isEnabled</span></span>     |<span data-ttu-id="90d87-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d87-112">Boolean</span></span>      | <span data-ttu-id="90d87-113">Указывает, включено ли управление сеансом.</span><span class="sxs-lookup"><span data-stu-id="90d87-113">Specifies whether the session control is enabled or not.</span></span> |

## <a name="relationships"></a><span data-ttu-id="90d87-114">Связи</span><span class="sxs-lookup"><span data-stu-id="90d87-114">Relationships</span></span>

<span data-ttu-id="90d87-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="90d87-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="90d87-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="90d87-116">JSON representation</span></span>

<span data-ttu-id="90d87-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90d87-117">The following is a JSON representation of the resource.</span></span>

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

