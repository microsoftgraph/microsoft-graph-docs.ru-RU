---
title: Тип ресурса Локализеддескриптион
description: Представляет локализованное описание термина в банке терминов.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 738555750c22f3ffdd5fbd43c8b1849888e0a40f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973619"
---
# <a name="localizeddescription-resource-type"></a><span data-ttu-id="d26c6-103">Тип ресурса Локализеддескриптион</span><span class="sxs-lookup"><span data-stu-id="d26c6-103">localizedDescription resource type</span></span>

<span data-ttu-id="d26c6-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="d26c6-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d26c6-105">Представляет локализованное описание [термина] в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="d26c6-105">Represents the localized description used to describe a [term] in the term [store].</span></span>


## <a name="properties"></a><span data-ttu-id="d26c6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d26c6-106">Properties</span></span>
|<span data-ttu-id="d26c6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d26c6-107">Property</span></span>|<span data-ttu-id="d26c6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d26c6-108">Type</span></span>|<span data-ttu-id="d26c6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d26c6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d26c6-110">description</span><span class="sxs-lookup"><span data-stu-id="d26c6-110">description</span></span>|<span data-ttu-id="d26c6-111">String</span><span class="sxs-lookup"><span data-stu-id="d26c6-111">String</span></span>|<span data-ttu-id="d26c6-112">Описание на языке локализации.</span><span class="sxs-lookup"><span data-stu-id="d26c6-112">The description in the localized language.</span></span>|
|<span data-ttu-id="d26c6-113">лангуажетаг</span><span class="sxs-lookup"><span data-stu-id="d26c6-113">languageTag</span></span>|<span data-ttu-id="d26c6-114">String</span><span class="sxs-lookup"><span data-stu-id="d26c6-114">String</span></span>|<span data-ttu-id="d26c6-115">Тег языка для метки.</span><span class="sxs-lookup"><span data-stu-id="d26c6-115">The language tag for the label.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d26c6-116">Связи</span><span class="sxs-lookup"><span data-stu-id="d26c6-116">Relationships</span></span>
<span data-ttu-id="d26c6-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d26c6-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d26c6-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d26c6-118">JSON representation</span></span>
<span data-ttu-id="d26c6-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d26c6-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.termStore.localizedDescription"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.localizedDescription",
  "description": "String",
  "languageTag": "String"
}
```

[microsoft.graph.termStore.term]: termStore-term.md
[microsoft.graph.termStore.store]: termStore-store.md
[банком]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md
[восстановлен]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md

<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedDescriptionFacet is the facet for containing the description of a set",
  "keywords": "termLocalizedDescriptionFacet,facet,resource",
  "section": "documentation",
  "tocPath": "TermLocalizedDescriptionFacet",
  "tocBookmarks": {
    "Resources/termStore.termLocalizedDescription": "#"
  },
  "suppressions": []
}
-->


