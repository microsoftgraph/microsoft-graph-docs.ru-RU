---
title: Тип ресурса localeInfo
description: Сведения о языковом стандарте, в частности предпочитаемом языке и стране или регионе, вошедшего пользователя.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bb6c8adbc76e0024f5168a8dbc52e8f56582dab3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522934"
---
# <a name="localeinfo-resource-type"></a><span data-ttu-id="92f56-103">Тип ресурса localeInfo</span><span class="sxs-lookup"><span data-stu-id="92f56-103">localeInfo resource type</span></span>

<span data-ttu-id="92f56-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="92f56-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92f56-105">Сведения о языковом стандарте, в частности предпочитаемом языке и стране или регионе, вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="92f56-105">Information about the locale, including the preferred language and country/region, of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="92f56-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="92f56-106">Properties</span></span>
| <span data-ttu-id="92f56-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="92f56-107">Property</span></span>     | <span data-ttu-id="92f56-108">Тип</span><span class="sxs-lookup"><span data-stu-id="92f56-108">Type</span></span>   |<span data-ttu-id="92f56-109">Описание</span><span class="sxs-lookup"><span data-stu-id="92f56-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92f56-110">языковые стандарты</span><span class="sxs-lookup"><span data-stu-id="92f56-110">locale</span></span>|<span data-ttu-id="92f56-111">string</span><span class="sxs-lookup"><span data-stu-id="92f56-111">string</span></span>|<span data-ttu-id="92f56-p101">Представления языкового стандарта для пользователя, которое включает предпочитаемый язык и страну или регион. Пример: "en-us". В языковом компоненте используются коды из двух букв, определенные в стандарте [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), а в компоненте страны — коды из стандарта [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span><span class="sxs-lookup"><span data-stu-id="92f56-p101">A locale representation for the user, which includes the user's preferred language and country/region. For example, "en-us". The language component follows 2-letter codes as defined in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), and the country component follows 2-letter codes as defined in [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span></span>|
|<span data-ttu-id="92f56-115">displayName</span><span class="sxs-lookup"><span data-stu-id="92f56-115">displayName</span></span>|<span data-ttu-id="92f56-116">string</span><span class="sxs-lookup"><span data-stu-id="92f56-116">string</span></span>|<span data-ttu-id="92f56-117">Имя, представляющее языковой стандарт пользователя на естественном языке, например "Английский (США)".</span><span class="sxs-lookup"><span data-stu-id="92f56-117">A name representing the user's locale in natural language, for example, "English (United States)".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92f56-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92f56-118">JSON representation</span></span>

<span data-ttu-id="92f56-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92f56-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.localeInfo"
}-->

```json
{
  "locale": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "localeInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
