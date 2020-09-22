---
title: Тип ресурса Локализеднаме
description: Представляет локализованное имя, используемое в банке терминов, которое определяет имя на локализованном языке.
author: mohitpcad
ms.author: mopathak
localization_priority: Normal
ms.prod: sharepoint-taxonomy
doc_type: resourcePageType
ms.openlocfilehash: 5c9e6d4cd614c242e8f915fde71eadd07aa5de15
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973608"
---
# <a name="localizedname-resource-type"></a><span data-ttu-id="bf416-103">Тип ресурса Локализеднаме</span><span class="sxs-lookup"><span data-stu-id="bf416-103">localizedName resource type</span></span>

<span data-ttu-id="bf416-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="bf416-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf416-105">Представляет локализованное имя, используемое в [банке]терминов, которое определяет имя на локализованном языке.</span><span class="sxs-lookup"><span data-stu-id="bf416-105">Represents the localized name used in the term [store], which identifies the name in the localized language.</span></span> <span data-ttu-id="bf416-106">Дополнительные сведения см. в разделе [локализедлабел].</span><span class="sxs-lookup"><span data-stu-id="bf416-106">For more information, see [localizedLabel].</span></span>

## <a name="properties"></a><span data-ttu-id="bf416-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf416-107">Properties</span></span>
|<span data-ttu-id="bf416-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf416-108">Property</span></span>|<span data-ttu-id="bf416-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bf416-109">Type</span></span>|<span data-ttu-id="bf416-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bf416-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf416-111">лангуажетаг</span><span class="sxs-lookup"><span data-stu-id="bf416-111">languageTag</span></span>|<span data-ttu-id="bf416-112">String</span><span class="sxs-lookup"><span data-stu-id="bf416-112">String</span></span>|<span data-ttu-id="bf416-113">Тег языка для метки.</span><span class="sxs-lookup"><span data-stu-id="bf416-113">The language tag for the label.</span></span>|
|<span data-ttu-id="bf416-114">name</span><span class="sxs-lookup"><span data-stu-id="bf416-114">name</span></span>|<span data-ttu-id="bf416-115">String</span><span class="sxs-lookup"><span data-stu-id="bf416-115">String</span></span>|<span data-ttu-id="bf416-116">Имя на языке локализации.</span><span class="sxs-lookup"><span data-stu-id="bf416-116">The name in the localized language.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf416-117">Связи</span><span class="sxs-lookup"><span data-stu-id="bf416-117">Relationships</span></span>
<span data-ttu-id="bf416-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bf416-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf416-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bf416-119">JSON representation</span></span>
<span data-ttu-id="bf416-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf416-120">The following is a JSON representation of the resource.</span></span>
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


