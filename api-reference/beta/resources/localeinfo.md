---
title: Тип ресурса localeInfo
description: Сведения о языковом стандарте, в частности предпочитаемом языке и стране или регионе, вошедшего пользователя.
localization_priority: Normal
ms.openlocfilehash: 7414130c1ed1e85353c653d9bbd36a0e488bcea9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578162"
---
# <a name="localeinfo-resource-type"></a><span data-ttu-id="b0a77-103">Тип ресурса localeInfo</span><span class="sxs-lookup"><span data-stu-id="b0a77-103">localeInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0a77-104">Сведения о языковом стандарте, в частности предпочитаемом языке и стране или регионе, вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="b0a77-104">Information about the locale, including the preferred language and country/region, of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="b0a77-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0a77-105">Properties</span></span>
| <span data-ttu-id="b0a77-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0a77-106">Property</span></span>     | <span data-ttu-id="b0a77-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b0a77-107">Type</span></span>   |<span data-ttu-id="b0a77-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b0a77-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0a77-109">locale</span><span class="sxs-lookup"><span data-stu-id="b0a77-109">locale</span></span>|<span data-ttu-id="b0a77-110">string</span><span class="sxs-lookup"><span data-stu-id="b0a77-110">string</span></span>|<span data-ttu-id="b0a77-p101">Представления языкового стандарта для пользователя, которое включает предпочитаемый язык и страну или регион. Пример: "en-us". В языковом компоненте используются коды из двух букв, определенные в стандарте [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), а в компоненте страны — коды из стандарта [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span><span class="sxs-lookup"><span data-stu-id="b0a77-p101">A locale representation for the user, which includes the user's preferred language and country/region. For example, "en-us". The language component follows 2-letter codes as defined in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), and the country component follows 2-letter codes as defined in [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span></span>|
|<span data-ttu-id="b0a77-114">displayName</span><span class="sxs-lookup"><span data-stu-id="b0a77-114">displayName</span></span>|<span data-ttu-id="b0a77-115">string</span><span class="sxs-lookup"><span data-stu-id="b0a77-115">string</span></span>|<span data-ttu-id="b0a77-116">Имя, представляющее языковой стандарт пользователя на естественном языке, например "Английский (США)".</span><span class="sxs-lookup"><span data-stu-id="b0a77-116">A name representing the user's locale in natural language, for example, "English (United States)".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0a77-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0a77-117">JSON representation</span></span>

<span data-ttu-id="b0a77-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0a77-118">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/localeinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
