# <a name="timezonebase-resource-type"></a><span data-ttu-id="18b09-101">Тип ресурса timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="18b09-101">timeZoneBase resource type</span></span>

<span data-ttu-id="18b09-102">Основное представление часового пояса.</span><span class="sxs-lookup"><span data-stu-id="18b09-102">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="18b09-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="18b09-103">Properties</span></span>
| <span data-ttu-id="18b09-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="18b09-104">Property</span></span>     | <span data-ttu-id="18b09-105">Тип</span><span class="sxs-lookup"><span data-stu-id="18b09-105">Type</span></span>   |<span data-ttu-id="18b09-106">Описание</span><span class="sxs-lookup"><span data-stu-id="18b09-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="18b09-107">name</span><span class="sxs-lookup"><span data-stu-id="18b09-107">name</span></span> | <span data-ttu-id="18b09-108">string</span><span class="sxs-lookup"><span data-stu-id="18b09-108">string</span></span> | <span data-ttu-id="18b09-109">Имя часового пояса</span><span class="sxs-lookup"><span data-stu-id="18b09-109">The name of a time zone.</span></span> <span data-ttu-id="18b09-110">(стандартного, например "Гавайско-Алеутское время (зима)" или особого, например "Особый часовой пояс").</span><span class="sxs-lookup"><span data-stu-id="18b09-110">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="18b09-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18b09-111">JSON representation</span></span>

<span data-ttu-id="18b09-112">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18b09-112">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->