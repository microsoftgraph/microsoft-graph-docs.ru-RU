# <a name="recentnotebook-resource-type"></a><span data-ttu-id="55c6a-101">Тип ресурса recentNotebook</span><span class="sxs-lookup"><span data-stu-id="55c6a-101">recentNotebook resource type</span></span>

<span data-ttu-id="55c6a-102">Недавно открытая записная книжка OneNote.</span><span class="sxs-lookup"><span data-stu-id="55c6a-102">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="55c6a-103">Ресурс **recentNotebook** похож на ресурс [notebook](notebook.md), но имеет меньше свойств.</span><span class="sxs-lookup"><span data-stu-id="55c6a-103">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="55c6a-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="55c6a-104">Properties</span></span>
| <span data-ttu-id="55c6a-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="55c6a-105">Property</span></span>     | <span data-ttu-id="55c6a-106">Тип</span><span class="sxs-lookup"><span data-stu-id="55c6a-106">Type</span></span>   |<span data-ttu-id="55c6a-107">Описание</span><span class="sxs-lookup"><span data-stu-id="55c6a-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55c6a-108">name</span><span class="sxs-lookup"><span data-stu-id="55c6a-108">name</span></span>|<span data-ttu-id="55c6a-109">String</span><span class="sxs-lookup"><span data-stu-id="55c6a-109">String</span></span>|<span data-ttu-id="55c6a-110">Имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="55c6a-110">The name of the notebook.</span></span>|
|<span data-ttu-id="55c6a-111">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="55c6a-111">lastAccessedTime</span></span>|<span data-ttu-id="55c6a-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55c6a-112">DateTimeOffset</span></span>|<span data-ttu-id="55c6a-113">Дата и время последнего изменения записной книжки.</span><span class="sxs-lookup"><span data-stu-id="55c6a-113">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="55c6a-114">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="55c6a-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="55c6a-115">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="55c6a-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="55c6a-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55c6a-116">Read-only.</span></span>|
|<span data-ttu-id="55c6a-117">links</span><span class="sxs-lookup"><span data-stu-id="55c6a-117">links</span></span>|[<span data-ttu-id="55c6a-118">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="55c6a-118">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="55c6a-119">Ссылки для открытия записной книжки.</span><span class="sxs-lookup"><span data-stu-id="55c6a-119">Links for opening the notebook.</span></span> <span data-ttu-id="55c6a-120">Ссылка `oneNoteClientURL` открывает записную книжку в клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="55c6a-120">The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed.</span></span> <span data-ttu-id="55c6a-121">Ссылка `oneNoteWebURL` открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="55c6a-121">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="55c6a-122">sourceService</span><span class="sxs-lookup"><span data-stu-id="55c6a-122">sourceService</span></span>|<span data-ttu-id="55c6a-123">String</span><span class="sxs-lookup"><span data-stu-id="55c6a-123">String</span></span>|<span data-ttu-id="55c6a-124">Внутреннее хранилище, в котором находится записная книжка (`OneDriveForBusiness` или `OneDrive`).</span><span class="sxs-lookup"><span data-stu-id="55c6a-124">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55c6a-125">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="55c6a-125">JSON representation</span></span>

<span data-ttu-id="55c6a-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55c6a-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebook"
}-->

```json
{
  "displayName": "String",
  "lastAccessedTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.recentNotebookLinks"},
  "sourceService": "String"
}

```

## <a name="methods"></a><span data-ttu-id="55c6a-127">Методы</span><span class="sxs-lookup"><span data-stu-id="55c6a-127">Methods</span></span>

| <span data-ttu-id="55c6a-128">Метод</span><span class="sxs-lookup"><span data-stu-id="55c6a-128">Method</span></span>           | <span data-ttu-id="55c6a-129">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="55c6a-129">Return Type</span></span>    |<span data-ttu-id="55c6a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="55c6a-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="55c6a-131">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="55c6a-131">getRecentNotebooks</span></span>](../api/notebook_getrecentnotebooks.md) | <span data-ttu-id="55c6a-132">Коллекция [notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="55c6a-132">[Notebook](notebook.md) collection</span></span> | <span data-ttu-id="55c6a-133">Получите коллекцию записных книжек, которые недавно открывал пользователь.</span><span class="sxs-lookup"><span data-stu-id="55c6a-133">Get a collection of the most recently accessed notebooks for the user.</span></span> |
