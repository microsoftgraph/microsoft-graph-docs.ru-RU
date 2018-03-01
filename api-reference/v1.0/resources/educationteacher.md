# <a name="educationteacher-resource-type"></a><span data-ttu-id="91af8-101">Тип ресурса educationTeacher</span><span class="sxs-lookup"><span data-stu-id="91af8-101">educationTeacher resource type</span></span>

<span data-ttu-id="91af8-102">Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.</span><span class="sxs-lookup"><span data-stu-id="91af8-102">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="91af8-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="91af8-103">Properties</span></span>
| <span data-ttu-id="91af8-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="91af8-104">Property</span></span>     | <span data-ttu-id="91af8-105">Тип</span><span class="sxs-lookup"><span data-stu-id="91af8-105">Type</span></span>   |<span data-ttu-id="91af8-106">Описание</span><span class="sxs-lookup"><span data-stu-id="91af8-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91af8-107">externalId</span><span class="sxs-lookup"><span data-stu-id="91af8-107">externalId</span></span>|<span data-ttu-id="91af8-108">String</span><span class="sxs-lookup"><span data-stu-id="91af8-108">String</span></span>| <span data-ttu-id="91af8-109">Идентификатор преподавателя в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="91af8-109">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="91af8-110">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="91af8-110">teacherNumber</span></span>|<span data-ttu-id="91af8-111">String</span><span class="sxs-lookup"><span data-stu-id="91af8-111">String</span></span>|<span data-ttu-id="91af8-112">Номер преподавателя.</span><span class="sxs-lookup"><span data-stu-id="91af8-112">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91af8-113">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="91af8-113">JSON representation</span></span>

<span data-ttu-id="91af8-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91af8-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeacher"
}-->

```json
{
  "externalId": "String",
  "teacherNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->