---
title: Тип ресурса localeInfo
description: Сведения о языковом стандарте, в частности предпочитаемом языке и стране или регионе, вошедшего пользователя.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 75797fa96e28c20b5d9bbec3178b64ebfc75218d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079125"
---
# <a name="localeinfo-resource-type"></a><span data-ttu-id="ed54b-103">Тип ресурса localeInfo</span><span class="sxs-lookup"><span data-stu-id="ed54b-103">localeInfo resource type</span></span>

<span data-ttu-id="ed54b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed54b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed54b-105">Сведения о языковом стандарте, в частности предпочитаемом языке и стране или регионе, вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="ed54b-105">Information about the locale, including the preferred language and country/region, of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="ed54b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed54b-106">Properties</span></span>
| <span data-ttu-id="ed54b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed54b-107">Property</span></span>     | <span data-ttu-id="ed54b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ed54b-108">Type</span></span>   |<span data-ttu-id="ed54b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ed54b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed54b-110">языковые стандарты</span><span class="sxs-lookup"><span data-stu-id="ed54b-110">locale</span></span>|<span data-ttu-id="ed54b-111">string</span><span class="sxs-lookup"><span data-stu-id="ed54b-111">string</span></span>|<span data-ttu-id="ed54b-p101">Представления языкового стандарта для пользователя, которое включает предпочитаемый язык и страну или регион. Пример: "en-us". В языковом компоненте используются коды из двух букв, определенные в стандарте [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), а в компоненте страны — коды из стандарта [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span><span class="sxs-lookup"><span data-stu-id="ed54b-p101">A locale representation for the user, which includes the user's preferred language and country/region. For example, "en-us". The language component follows 2-letter codes as defined in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), and the country component follows 2-letter codes as defined in [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span></span>|
|<span data-ttu-id="ed54b-115">displayName</span><span class="sxs-lookup"><span data-stu-id="ed54b-115">displayName</span></span>|<span data-ttu-id="ed54b-116">string</span><span class="sxs-lookup"><span data-stu-id="ed54b-116">string</span></span>|<span data-ttu-id="ed54b-117">Имя, представляющее языковой стандарт пользователя на естественном языке, например "Английский (США)".</span><span class="sxs-lookup"><span data-stu-id="ed54b-117">A name representing the user's locale in natural language, for example, "English (United States)".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed54b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed54b-118">JSON representation</span></span>

<span data-ttu-id="ed54b-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed54b-119">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "localeInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

