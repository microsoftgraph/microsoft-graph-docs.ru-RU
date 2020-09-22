---
title: Тип ресурса Локализедлабел
description: Представляет метку термина в банке терминов.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: cadad79f6e019a258842fff1be679adf6c85fb3a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973612"
---
# <a name="localizedlabel-resource-type"></a><span data-ttu-id="f806f-103">Тип ресурса Локализедлабел</span><span class="sxs-lookup"><span data-stu-id="f806f-103">localizedLabel resource type</span></span>

<span data-ttu-id="f806f-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="f806f-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f806f-105">Представляет метку [термина] в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="f806f-105">Represents the label for a [term] in the term [store].</span></span>

<span data-ttu-id="f806f-106">Определяет метки, связанные с заданным термином.</span><span class="sxs-lookup"><span data-stu-id="f806f-106">Identifies the labels associated with a given term.</span></span>

## <a name="properties"></a><span data-ttu-id="f806f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f806f-107">Properties</span></span>
|<span data-ttu-id="f806f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f806f-108">Property</span></span>|<span data-ttu-id="f806f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f806f-109">Type</span></span>|<span data-ttu-id="f806f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f806f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f806f-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="f806f-111">isDefault</span></span>|<span data-ttu-id="f806f-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="f806f-112">Boolean</span></span>|<span data-ttu-id="f806f-113">Указывает, является ли метка меткой по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f806f-113">Indicates whether the label is the default label.</span></span>|
|<span data-ttu-id="f806f-114">лангуажетаг</span><span class="sxs-lookup"><span data-stu-id="f806f-114">languageTag</span></span>|<span data-ttu-id="f806f-115">String</span><span class="sxs-lookup"><span data-stu-id="f806f-115">String</span></span>|<span data-ttu-id="f806f-116">Тег ангуаже для метки.</span><span class="sxs-lookup"><span data-stu-id="f806f-116">The anguage tag for the label.</span></span>|
|<span data-ttu-id="f806f-117">name</span><span class="sxs-lookup"><span data-stu-id="f806f-117">name</span></span>|<span data-ttu-id="f806f-118">String</span><span class="sxs-lookup"><span data-stu-id="f806f-118">String</span></span>|<span data-ttu-id="f806f-119">Имя метки.</span><span class="sxs-lookup"><span data-stu-id="f806f-119">The name of the label.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f806f-120">Связи</span><span class="sxs-lookup"><span data-stu-id="f806f-120">Relationships</span></span>
<span data-ttu-id="f806f-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f806f-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f806f-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f806f-122">JSON representation</span></span>
<span data-ttu-id="f806f-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f806f-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.termStore.localizedLabel"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.localizedLabel",
  "name": "String",
  "isDefault": "Boolean",
  "languageTag": "String"
}
```


[microsoft.graph.termStore.term]: termstore-term.md
[microsoft.graph.termStore.localizedName]: termstore-localizedname.md
[microsoft.graph.termStore.store]: termstore-store.md
[банком]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md
[восстановлен]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md


<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedLabelFacet is the facet for containing the label of a term",
  "keywords": "termLocalizedLabelFacet,facet,resource",
  "section": "documentation",
  "tocPath": "termstorelocalizedlabel",
  "tocBookmarks": {
    "Resources/termStore.termstorelocalizedlabel": "#"
  },
  "suppressions": []
}
-->


