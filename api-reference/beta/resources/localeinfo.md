---
title: Тип ресурса localeInfo
description: Сведения о языковом стандарте, в частности предпочитаемом языке и стране или регионе, вошедшего пользователя.
localization_priority: Normal
ms.openlocfilehash: cfd5b0e318a2f78d382dccd10b23da167d8b5c8a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888202"
---
# <a name="localeinfo-resource-type"></a><span data-ttu-id="4f9a7-103">Тип ресурса localeInfo</span><span class="sxs-lookup"><span data-stu-id="4f9a7-103">localeInfo resource type</span></span>

> <span data-ttu-id="4f9a7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4f9a7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f9a7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f9a7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4f9a7-106">Сведения о языковом стандарте, в частности предпочитаемом языке и стране или регионе, вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f9a7-106">Information about the locale, including the preferred language and country/region, of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="4f9a7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f9a7-107">Properties</span></span>
| <span data-ttu-id="4f9a7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f9a7-108">Property</span></span>     | <span data-ttu-id="4f9a7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4f9a7-109">Type</span></span>   |<span data-ttu-id="4f9a7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4f9a7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f9a7-111">locale</span><span class="sxs-lookup"><span data-stu-id="4f9a7-111">locale</span></span>|<span data-ttu-id="4f9a7-112">string</span><span class="sxs-lookup"><span data-stu-id="4f9a7-112">string</span></span>|<span data-ttu-id="4f9a7-p102">Представления языкового стандарта для пользователя, которое включает предпочитаемый язык и страну или регион. Пример: "en-us". В языковом компоненте используются коды из двух букв, определенные в стандарте [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), а в компоненте страны — коды из стандарта [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span><span class="sxs-lookup"><span data-stu-id="4f9a7-p102">A locale representation for the user, which includes the user's preferred language and country/region. For example, "en-us". The language component follows 2-letter codes as defined in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), and the country component follows 2-letter codes as defined in [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span></span>|
|<span data-ttu-id="4f9a7-116">displayName</span><span class="sxs-lookup"><span data-stu-id="4f9a7-116">displayName</span></span>|<span data-ttu-id="4f9a7-117">строка</span><span class="sxs-lookup"><span data-stu-id="4f9a7-117">string</span></span>|<span data-ttu-id="4f9a7-118">Имя, представляющее языковой стандарт пользователя на естественном языке, например "Английский (США)".</span><span class="sxs-lookup"><span data-stu-id="4f9a7-118">A name representing the user's locale in natural language, for example, "English (United States)".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f9a7-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f9a7-119">JSON representation</span></span>

<span data-ttu-id="4f9a7-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f9a7-120">Here is a JSON representation of the resource.</span></span>

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
