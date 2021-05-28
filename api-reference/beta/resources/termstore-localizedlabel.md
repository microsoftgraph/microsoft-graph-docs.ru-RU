---
title: тип локализованных ресурсовLabel
description: Представляет метку для термина в магазине терминов.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4d7de3c9567c20659af4c863d2cf1ac248beff6b
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696312"
---
# <a name="localizedlabel-resource-type"></a><span data-ttu-id="af788-103">тип локализованных ресурсовLabel</span><span class="sxs-lookup"><span data-stu-id="af788-103">localizedLabel resource type</span></span>

<span data-ttu-id="af788-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="af788-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af788-105">Представляет метку для [термина в] магазине [терминов].</span><span class="sxs-lookup"><span data-stu-id="af788-105">Represents the label for a [term] in the term [store].</span></span>

<span data-ttu-id="af788-106">Определяет метки, связанные с заданным термином.</span><span class="sxs-lookup"><span data-stu-id="af788-106">Identifies the labels associated with a given term.</span></span>

## <a name="properties"></a><span data-ttu-id="af788-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="af788-107">Properties</span></span>
|<span data-ttu-id="af788-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="af788-108">Property</span></span>|<span data-ttu-id="af788-109">Тип</span><span class="sxs-lookup"><span data-stu-id="af788-109">Type</span></span>|<span data-ttu-id="af788-110">Описание</span><span class="sxs-lookup"><span data-stu-id="af788-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af788-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="af788-111">isDefault</span></span>|<span data-ttu-id="af788-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="af788-112">Boolean</span></span>|<span data-ttu-id="af788-113">Указывает, является ли метка меткой по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="af788-113">Indicates whether the label is the default label.</span></span>|
|<span data-ttu-id="af788-114">LanguageTag</span><span class="sxs-lookup"><span data-stu-id="af788-114">languageTag</span></span>|<span data-ttu-id="af788-115">String</span><span class="sxs-lookup"><span data-stu-id="af788-115">String</span></span>|<span data-ttu-id="af788-116">Тег языка для метки.</span><span class="sxs-lookup"><span data-stu-id="af788-116">The language tag for the label.</span></span>|
|<span data-ttu-id="af788-117">name</span><span class="sxs-lookup"><span data-stu-id="af788-117">name</span></span>|<span data-ttu-id="af788-118">String</span><span class="sxs-lookup"><span data-stu-id="af788-118">String</span></span>|<span data-ttu-id="af788-119">Имя метки.</span><span class="sxs-lookup"><span data-stu-id="af788-119">The name of the label.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af788-120">Связи</span><span class="sxs-lookup"><span data-stu-id="af788-120">Relationships</span></span>
<span data-ttu-id="af788-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="af788-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="af788-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="af788-122">JSON representation</span></span>
<span data-ttu-id="af788-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af788-123">The following is a JSON representation of the resource.</span></span>
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
[термин]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md
[магазин]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md


<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedLabelFacet is the facet for containing the label of a term",
  "keywords": "termLocalizedLabelFacet,facet,resource",
  "section": "documentation",
  "tocPath": "termstorelocalizedlabel",
  "tocBookmarks": {
    "Resources/termStore.termstorelocalizedlabel&quot;: &quot;#"
  },
  "suppressions": []
}
-->


