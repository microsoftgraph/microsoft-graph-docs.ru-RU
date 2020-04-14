---
title: Тип ресурса Аппликатионенфорцедрестриктионссессионконтрол
description: Управление сеансами для применения ограничений приложений.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 258da369c6a254aa2cff1f611564eb3121d3633b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472231"
---
# <a name="applicationenforcedrestrictionssessioncontrol-resource-type"></a><span data-ttu-id="acc90-103">Тип ресурса Аппликатионенфорцедрестриктионссессионконтрол</span><span class="sxs-lookup"><span data-stu-id="acc90-103">applicationEnforcedRestrictionsSessionControl resource type</span></span>

<span data-ttu-id="acc90-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acc90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acc90-105">Управление сеансами для применения ограничений приложений.</span><span class="sxs-lookup"><span data-stu-id="acc90-105">Session control to enforce application restrictions.</span></span> <span data-ttu-id="acc90-106">Инехритс из [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="acc90-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="acc90-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="acc90-107">Properties</span></span>

| <span data-ttu-id="acc90-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="acc90-108">Property</span></span>     | <span data-ttu-id="acc90-109">Тип</span><span class="sxs-lookup"><span data-stu-id="acc90-109">Type</span></span>        | <span data-ttu-id="acc90-110">Описание</span><span class="sxs-lookup"><span data-stu-id="acc90-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="acc90-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="acc90-111">isEnabled</span></span>     |<span data-ttu-id="acc90-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="acc90-112">Boolean</span></span>      | <span data-ttu-id="acc90-113">Указывает, включен ли элемент управления сеансом.</span><span class="sxs-lookup"><span data-stu-id="acc90-113">Specifies whether the session control is enabled or not.</span></span> |

## <a name="relationships"></a><span data-ttu-id="acc90-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="acc90-114">Relationships</span></span>

<span data-ttu-id="acc90-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="acc90-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="acc90-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="acc90-116">JSON representation</span></span>

<span data-ttu-id="acc90-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="acc90-117">The following is a JSON representation of the resource.</span></span>

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
