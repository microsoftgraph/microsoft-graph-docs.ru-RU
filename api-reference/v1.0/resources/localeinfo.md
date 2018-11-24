# <a name="localeinfo-resource-type"></a><span data-ttu-id="3f8c9-101">Тип ресурса localeInfo</span><span class="sxs-lookup"><span data-stu-id="3f8c9-101">localeInfo resource type</span></span>

<span data-ttu-id="3f8c9-102">Сведения о языковом стандарте, в частности предпочитаемом языке и стране или регионе, вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="3f8c9-102">Information about the locale, including the preferred language and country/region, of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="3f8c9-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f8c9-103">Properties</span></span>
| <span data-ttu-id="3f8c9-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f8c9-104">Property</span></span>     | <span data-ttu-id="3f8c9-105">Тип</span><span class="sxs-lookup"><span data-stu-id="3f8c9-105">Type</span></span>   |<span data-ttu-id="3f8c9-106">Описание</span><span class="sxs-lookup"><span data-stu-id="3f8c9-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f8c9-107">locale</span><span class="sxs-lookup"><span data-stu-id="3f8c9-107">locale</span></span>|<span data-ttu-id="3f8c9-108">string</span><span class="sxs-lookup"><span data-stu-id="3f8c9-108">string</span></span>|<span data-ttu-id="3f8c9-p101">Представления языкового стандарта для пользователя, которое включает предпочитаемый язык и страну или регион. Пример: "en-us". В языковом компоненте используются коды из двух букв, определенные в стандарте [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), а в компоненте страны — коды из стандарта [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span><span class="sxs-lookup"><span data-stu-id="3f8c9-p101">A locale representation for the user, which includes the user's preferred language and country/region. For example, "en-us". The language component follows 2-letter codes as defined in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), and the country component follows 2-letter codes as defined in [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).</span></span>|
|<span data-ttu-id="3f8c9-112">displayName</span><span class="sxs-lookup"><span data-stu-id="3f8c9-112">displayName</span></span>|<span data-ttu-id="3f8c9-113">строка</span><span class="sxs-lookup"><span data-stu-id="3f8c9-113">string</span></span>|<span data-ttu-id="3f8c9-114">Имя, представляющее языковой стандарт пользователя на естественном языке, например "Английский (США)".</span><span class="sxs-lookup"><span data-stu-id="3f8c9-114">A name representing the user's locale in natural language, for example, "English (United States)".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3f8c9-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f8c9-115">JSON representation</span></span>

<span data-ttu-id="3f8c9-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f8c9-116">Here is a JSON representation of the resource.</span></span>

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