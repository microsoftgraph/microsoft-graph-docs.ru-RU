---
title: Тип ресурса Локализеднаме
description: Представляет локализованное имя, используемое в банке терминов, которое определяет имя на локализованном языке.
author: mohitpcad
ms.author: mopathak
localization_priority: Normal
ms.prod: sharepoint-taxonomy
doc_type: resourcePageType
ms.openlocfilehash: cc29deb6e6db5f5664e6fb6bed69195b7183e026
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539383"
---
# <a name="localizedname-resource-type"></a><span data-ttu-id="d7af5-103">Тип ресурса Локализеднаме</span><span class="sxs-lookup"><span data-stu-id="d7af5-103">localizedName resource type</span></span>

<span data-ttu-id="d7af5-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="d7af5-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7af5-105">Представляет локализованное имя, используемое в [банке]терминов, которое определяет имя на локализованном языке.</span><span class="sxs-lookup"><span data-stu-id="d7af5-105">Represents the localized name used in the term [store], which identifies the name in the localized language.</span></span> <span data-ttu-id="d7af5-106">Дополнительные сведения см. в разделе [локализедлабел].</span><span class="sxs-lookup"><span data-stu-id="d7af5-106">For more information, see [localizedLabel].</span></span>

## <a name="properties"></a><span data-ttu-id="d7af5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7af5-107">Properties</span></span>
|<span data-ttu-id="d7af5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7af5-108">Property</span></span>|<span data-ttu-id="d7af5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d7af5-109">Type</span></span>|<span data-ttu-id="d7af5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d7af5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7af5-111">лангуажетаг</span><span class="sxs-lookup"><span data-stu-id="d7af5-111">languageTag</span></span>|<span data-ttu-id="d7af5-112">String</span><span class="sxs-lookup"><span data-stu-id="d7af5-112">String</span></span>|<span data-ttu-id="d7af5-113">Тег языка для метки.</span><span class="sxs-lookup"><span data-stu-id="d7af5-113">The language tag for the label.</span></span>|
|<span data-ttu-id="d7af5-114">name</span><span class="sxs-lookup"><span data-stu-id="d7af5-114">name</span></span>|<span data-ttu-id="d7af5-115">String</span><span class="sxs-lookup"><span data-stu-id="d7af5-115">String</span></span>|<span data-ttu-id="d7af5-116">Имя на языке локализации.</span><span class="sxs-lookup"><span data-stu-id="d7af5-116">The name in the localized language.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7af5-117">Связи</span><span class="sxs-lookup"><span data-stu-id="d7af5-117">Relationships</span></span>
<span data-ttu-id="d7af5-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d7af5-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7af5-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d7af5-119">JSON representation</span></span>
<span data-ttu-id="d7af5-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7af5-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.termStore.localizedName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.localizedName",
  "name": "String",
  "languageTag": "String"
}
```

[microsoft.graph.termStore.localizedLabel]: termstore-localizedlabel.md
[microsoft.graph.termstore.store]: termstore-store.md
[восстановлен]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md
[локализедлабел]: ../resources/termstore-localizedlabel.md
[localizedLabel]: ../resources/termstore-localizedlabel.md

<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedName is the facet for containing the name of termGroup",
  "keywords": "termLocalizedLNameFacet,facet,resource",
  "section": "documentation",
  "tocPath": "TermLocalizedNameFacet",
  "tocBookmarks": {
    "Resources/termStore.termLocalizedName": "#"
  },
  "suppressions": []
}
-->
