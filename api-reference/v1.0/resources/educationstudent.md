# <a name="educationstudent-resource-type"></a><span data-ttu-id="3ca7c-101">Тип ресурса educationStudent</span><span class="sxs-lookup"><span data-stu-id="3ca7c-101">educationStudent resource type</span></span>

<span data-ttu-id="3ca7c-102">Добавляются дополнительные сведения в файл [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `student`.</span><span class="sxs-lookup"><span data-stu-id="3ca7c-102">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="3ca7c-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ca7c-103">Properties</span></span>
| <span data-ttu-id="3ca7c-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ca7c-104">Property</span></span>     | <span data-ttu-id="3ca7c-105">Тип</span><span class="sxs-lookup"><span data-stu-id="3ca7c-105">Type</span></span>   |<span data-ttu-id="3ca7c-106">Описание</span><span class="sxs-lookup"><span data-stu-id="3ca7c-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ca7c-107">birthDate</span><span class="sxs-lookup"><span data-stu-id="3ca7c-107">birthDate</span></span>|<span data-ttu-id="3ca7c-108">Date</span><span class="sxs-lookup"><span data-stu-id="3ca7c-108">Date</span></span>| <span data-ttu-id="3ca7c-109">Дата рождения учащегося.</span><span class="sxs-lookup"><span data-stu-id="3ca7c-109">Birth date of the student.</span></span>|
|<span data-ttu-id="3ca7c-110">externalId</span><span class="sxs-lookup"><span data-stu-id="3ca7c-110">externalId</span></span>|<span data-ttu-id="3ca7c-111">String</span><span class="sxs-lookup"><span data-stu-id="3ca7c-111">String</span></span>| <span data-ttu-id="3ca7c-112">Идентификатор учащегося в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="3ca7c-112">ID of the student in the source system.</span></span>|
|<span data-ttu-id="3ca7c-113">gender</span><span class="sxs-lookup"><span data-stu-id="3ca7c-113">gender</span></span>|`educationGender enumeration`| <span data-ttu-id="3ca7c-114">Возможные значения: `female`, `male`, `other`, `unkownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3ca7c-114">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="3ca7c-115">оценка</span><span class="sxs-lookup"><span data-stu-id="3ca7c-115">QuizInfoPage: grade</span></span>|<span data-ttu-id="3ca7c-116">String</span><span class="sxs-lookup"><span data-stu-id="3ca7c-116">String</span></span>|<span data-ttu-id="3ca7c-117">Текущий уровень оценок учащегося.</span><span class="sxs-lookup"><span data-stu-id="3ca7c-117">Current grade level of the student.</span></span>|
|<span data-ttu-id="3ca7c-118">graduationYear</span><span class="sxs-lookup"><span data-stu-id="3ca7c-118">graduationYear</span></span>|<span data-ttu-id="3ca7c-119">String</span><span class="sxs-lookup"><span data-stu-id="3ca7c-119">String</span></span>| <span data-ttu-id="3ca7c-120">Год выпуска учащегося из школы.</span><span class="sxs-lookup"><span data-stu-id="3ca7c-120">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="3ca7c-121">studentNumber</span><span class="sxs-lookup"><span data-stu-id="3ca7c-121">studentNumber</span></span>|<span data-ttu-id="3ca7c-122">String</span><span class="sxs-lookup"><span data-stu-id="3ca7c-122">String</span></span>| <span data-ttu-id="3ca7c-123">Student Number.</span><span class="sxs-lookup"><span data-stu-id="3ca7c-123">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ca7c-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ca7c-124">JSON representation</span></span>

<span data-ttu-id="3ca7c-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ca7c-125">The following is a JSON representation of the resource.</span></span>

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