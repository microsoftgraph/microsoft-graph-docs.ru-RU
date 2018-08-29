# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="4ba8a-101">Тип ресурсов attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="4ba8a-101">attendeeAvailability resource type</span></span>

<span data-ttu-id="4ba8a-102">Тип и занятость участника.</span><span class="sxs-lookup"><span data-stu-id="4ba8a-102">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ba8a-103">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4ba8a-103">JSON representation</span></span>

<span data-ttu-id="4ba8a-104">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="4ba8a-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="4ba8a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ba8a-105">Properties</span></span>
| <span data-ttu-id="4ba8a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ba8a-106">Property</span></span>     | <span data-ttu-id="4ba8a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4ba8a-107">Type</span></span>   |<span data-ttu-id="4ba8a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4ba8a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ba8a-109">участник</span><span class="sxs-lookup"><span data-stu-id="4ba8a-109">attendee</span></span>|[<span data-ttu-id="4ba8a-110">База участника</span><span class="sxs-lookup"><span data-stu-id="4ba8a-110">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="4ba8a-111">Тип участника (сведения о том, является ли участник пользователем или ресурсом, а также о том, обязательный ли он, если объект представляет пользователя).</span><span class="sxs-lookup"><span data-stu-id="4ba8a-111">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="4ba8a-112">доступность</span><span class="sxs-lookup"><span data-stu-id="4ba8a-112">availability</span></span>|<span data-ttu-id="4ba8a-113">статус "Свободен-занят"</span><span class="sxs-lookup"><span data-stu-id="4ba8a-113">freeBusyStatus values</span></span>| <span data-ttu-id="4ba8a-114">Состояние доступности участника.</span><span class="sxs-lookup"><span data-stu-id="4ba8a-114">The availability status of the attendee. Possible values are: , , , , , .</span></span> <span data-ttu-id="4ba8a-115">Допустимые значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`,`unknown`.</span><span class="sxs-lookup"><span data-stu-id="4ba8a-115">The possible values are `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`, , , , , , or .</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
