# <a name="educationstudent-resource-type"></a><span data-ttu-id="7b09b-101">Тип ресурса educationStudent</span><span class="sxs-lookup"><span data-stu-id="7b09b-101">educationStudent resource type</span></span>

<span data-ttu-id="7b09b-102">Добавляются дополнительные сведения в файл [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `student`.</span><span class="sxs-lookup"><span data-stu-id="7b09b-102">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="7b09b-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b09b-103">Properties</span></span>
| <span data-ttu-id="7b09b-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b09b-104">Property</span></span>     | <span data-ttu-id="7b09b-105">Тип</span><span class="sxs-lookup"><span data-stu-id="7b09b-105">Type</span></span>   |<span data-ttu-id="7b09b-106">Описание</span><span class="sxs-lookup"><span data-stu-id="7b09b-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b09b-107">birthDate</span><span class="sxs-lookup"><span data-stu-id="7b09b-107">birthDate</span></span>|<span data-ttu-id="7b09b-108">Date</span><span class="sxs-lookup"><span data-stu-id="7b09b-108">Date</span></span>| <span data-ttu-id="7b09b-109">Дата рождения учащегося.</span><span class="sxs-lookup"><span data-stu-id="7b09b-109">Birth date of the student.</span></span>|
|<span data-ttu-id="7b09b-110">externalId</span><span class="sxs-lookup"><span data-stu-id="7b09b-110">externalId</span></span>|<span data-ttu-id="7b09b-111">String (строка)</span><span class="sxs-lookup"><span data-stu-id="7b09b-111">String</span></span>| <span data-ttu-id="7b09b-112">Идентификатор учащегося в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="7b09b-112">ID of the student in the source system.</span></span>|
|<span data-ttu-id="7b09b-113">gender</span><span class="sxs-lookup"><span data-stu-id="7b09b-113">gender</span></span>|<span data-ttu-id="7b09b-114">educationGender</span><span class="sxs-lookup"><span data-stu-id="7b09b-114">educationGender values</span></span>| <span data-ttu-id="7b09b-115">Возможные значения: `female`, `male`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7b09b-115">The possible values are `female`, `male`, `other`, `unknownFutureValue`, , , , , , , , or .</span></span>|
|<span data-ttu-id="7b09b-116">grade</span><span class="sxs-lookup"><span data-stu-id="7b09b-116">grade</span></span>|<span data-ttu-id="7b09b-117">String (строка)</span><span class="sxs-lookup"><span data-stu-id="7b09b-117">String</span></span>|<span data-ttu-id="7b09b-118">Текущий уровень оценок учащегося.</span><span class="sxs-lookup"><span data-stu-id="7b09b-118">Current grade level of the student.</span></span>|
|<span data-ttu-id="7b09b-119">graduationYear</span><span class="sxs-lookup"><span data-stu-id="7b09b-119">graduationYear</span></span>|<span data-ttu-id="7b09b-120">String (строка)</span><span class="sxs-lookup"><span data-stu-id="7b09b-120">String</span></span>| <span data-ttu-id="7b09b-121">Год выпуска учащегося.</span><span class="sxs-lookup"><span data-stu-id="7b09b-121">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="7b09b-122">studentNumber</span><span class="sxs-lookup"><span data-stu-id="7b09b-122">studentNumber</span></span>|<span data-ttu-id="7b09b-123">String (строка)</span><span class="sxs-lookup"><span data-stu-id="7b09b-123">String</span></span>| <span data-ttu-id="7b09b-124">Номер учащегося.</span><span class="sxs-lookup"><span data-stu-id="7b09b-124">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b09b-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7b09b-125">JSON representation</span></span>

<span data-ttu-id="7b09b-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b09b-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationStudent"
}-->

```json
{
  "birthDate": "String (timestamp)",
  "externalId": "String",
  "gender": "educationGender",
  "grade": "String",
  "graduationYear": "String",
  "studentNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
