---
title: тип ресурса translationLanguageOverride
description: Ресурс, представляющий запись в переопределяемом списке языка перевода.
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: c9fa8d600ee3fb503446965d78491563c4ceae2e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954953"
---
# <a name="translationlanguageoverride-resource-type"></a><span data-ttu-id="3ba9d-103">тип ресурса translationLanguageOverride</span><span class="sxs-lookup"><span data-stu-id="3ba9d-103">translationLanguageOverride resource type</span></span>

<span data-ttu-id="3ba9d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ba9d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ba9d-105">Представляет любые переопределения перевода для языка.</span><span class="sxs-lookup"><span data-stu-id="3ba9d-105">Represents any translation override for a language.</span></span>

## <a name="properties"></a><span data-ttu-id="3ba9d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ba9d-106">Properties</span></span>

|<span data-ttu-id="3ba9d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ba9d-107">Property</span></span>             |<span data-ttu-id="3ba9d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3ba9d-108">Type</span></span>                                         |<span data-ttu-id="3ba9d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3ba9d-109">Description</span></span>                                                            |
|---------------------|-------------------------------------------------------------|-----------------------------------------------------------------------|
|<span data-ttu-id="3ba9d-110">LanguageTag</span><span class="sxs-lookup"><span data-stu-id="3ba9d-110">languageTag</span></span>          |<span data-ttu-id="3ba9d-111">Строка</span><span class="sxs-lookup"><span data-stu-id="3ba9d-111">String</span></span>                                       |<span data-ttu-id="3ba9d-112">Язык для применения переопределения.</span><span class="sxs-lookup"><span data-stu-id="3ba9d-112">The language to apply the override.</span></span><br><br><span data-ttu-id="3ba9d-113">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3ba9d-113">Returned by default.</span></span> <span data-ttu-id="3ba9d-114">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="3ba9d-114">Not nullable.</span></span>       |                   
|<span data-ttu-id="3ba9d-115">translationBehavior</span><span class="sxs-lookup"><span data-stu-id="3ba9d-115">translationBehavior</span></span>  |[<span data-ttu-id="3ba9d-116">translationBehavior</span><span class="sxs-lookup"><span data-stu-id="3ba9d-116">translationBehavior</span></span>](translationPreferences.md#translationbehavior-values)        |<span data-ttu-id="3ba9d-117">Переопределять поведение перевода для языка, если таково.</span><span class="sxs-lookup"><span data-stu-id="3ba9d-117">The translation override behavior for the language, if any.</span></span><br><br><span data-ttu-id="3ba9d-118">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3ba9d-118">Returned by default.</span></span> <span data-ttu-id="3ba9d-119">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="3ba9d-119">Not nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ba9d-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ba9d-120">JSON representation</span></span>

<span data-ttu-id="3ba9d-121">Ниже приводится определение ресурса JSON.</span><span class="sxs-lookup"><span data-stu-id="3ba9d-121">The following is a JSON definition of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.translationLanguageOverride"
}-->

```json
{
    "languageTag": "string",
    "translationBehavior": "string"
}
```
<!-- {
  "type": "#page.annotation",
  "description": translationLanguageOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


