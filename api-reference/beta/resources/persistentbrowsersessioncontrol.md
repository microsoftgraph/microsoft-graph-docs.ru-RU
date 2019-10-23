---
title: Тип ресурса Персистентбровсерсессионконтрол
description: Элемент управления сеансом, чтобы определить, следует ли сохранять файлы cookie.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7e2e9304aa8c7e7c8d59602a5710596b14e74636
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638612"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a><span data-ttu-id="61df5-103">Тип ресурса Персистентбровсерсессионконтрол</span><span class="sxs-lookup"><span data-stu-id="61df5-103">persistentBrowserSessionControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61df5-104">Элемент управления сеансом, чтобы определить, следует ли сохранять файлы cookie.</span><span class="sxs-lookup"><span data-stu-id="61df5-104">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="61df5-105">Инехритс из [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="61df5-105">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="61df5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="61df5-106">Properties</span></span>

| <span data-ttu-id="61df5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="61df5-107">Property</span></span>     | <span data-ttu-id="61df5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="61df5-108">Type</span></span>        | <span data-ttu-id="61df5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="61df5-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="61df5-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="61df5-110">isEnabled</span></span>     |<span data-ttu-id="61df5-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="61df5-111">Boolean</span></span>      | <span data-ttu-id="61df5-112">Указывает, включен ли элемент управления сеансом.</span><span class="sxs-lookup"><span data-stu-id="61df5-112">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="61df5-113">mode</span><span class="sxs-lookup"><span data-stu-id="61df5-113">mode</span></span>|<span data-ttu-id="61df5-114">String</span><span class="sxs-lookup"><span data-stu-id="61df5-114">String</span></span>| <span data-ttu-id="61df5-115">Возможные значения: `always`, `never`.</span><span class="sxs-lookup"><span data-stu-id="61df5-115">Possible values are: `always`, `never`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61df5-116">Связи</span><span class="sxs-lookup"><span data-stu-id="61df5-116">Relationships</span></span>

<span data-ttu-id="61df5-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="61df5-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="61df5-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="61df5-118">JSON representation</span></span>

<span data-ttu-id="61df5-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61df5-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.persistentBrowserSessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "mode": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "persistentBrowserSessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->