# <a name="recentnotebook-resource-type"></a><span data-ttu-id="e3893-101">Тип ресурса recentNotebook</span><span class="sxs-lookup"><span data-stu-id="e3893-101">recentNotebook resource type</span></span>

<span data-ttu-id="e3893-102">Недавно открытая записная книжка OneNote.</span><span class="sxs-lookup"><span data-stu-id="e3893-102">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="e3893-103">Ресурс **recentNotebook** похож на ресурс [notebook](notebook.md), но имеет меньше свойств.</span><span class="sxs-lookup"><span data-stu-id="e3893-103">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="e3893-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3893-104">Properties</span></span>
| <span data-ttu-id="e3893-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3893-105">Property</span></span>     | <span data-ttu-id="e3893-106">Тип</span><span class="sxs-lookup"><span data-stu-id="e3893-106">Type</span></span>   |<span data-ttu-id="e3893-107">Описание</span><span class="sxs-lookup"><span data-stu-id="e3893-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3893-108">displayName</span><span class="sxs-lookup"><span data-stu-id="e3893-108">displayName</span></span>|<span data-ttu-id="e3893-109">Строка</span><span class="sxs-lookup"><span data-stu-id="e3893-109">String</span></span>|<span data-ttu-id="e3893-110">Имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="e3893-110">The name of the notebook.</span></span>|
|<span data-ttu-id="e3893-111">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="e3893-111">lastAccessedTime</span></span>|<span data-ttu-id="e3893-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3893-112">DateTimeOffset</span></span>|<span data-ttu-id="e3893-p102">Дата и время последнего изменения записной книжки. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3893-p102">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="e3893-117">links</span><span class="sxs-lookup"><span data-stu-id="e3893-117">links</span></span>|[<span data-ttu-id="e3893-118">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="e3893-118">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="e3893-119">Ссылки для открытия записной книжки.</span><span class="sxs-lookup"><span data-stu-id="e3893-119">Links for opening the notebook.</span></span> <span data-ttu-id="e3893-120">Ссылка `oneNoteClientURL` открывает записную книжку в клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="e3893-120">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="e3893-121">Ссылка `oneNoteWebURL` открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="e3893-121">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="e3893-122">sourceService</span><span class="sxs-lookup"><span data-stu-id="e3893-122">sourceService</span></span>|<span data-ttu-id="e3893-123">onenoteSourceService</span><span class="sxs-lookup"><span data-stu-id="e3893-123">onenoteSourceService values</span></span>|<span data-ttu-id="e3893-124">Внутреннее хранилище, в котором находится записная книжка (`OneDriveForBusiness` или `OneDrive`).</span><span class="sxs-lookup"><span data-stu-id="e3893-124">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3893-125">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e3893-125">JSON representation</span></span>

<span data-ttu-id="e3893-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3893-126">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="e3893-127">Методы</span><span class="sxs-lookup"><span data-stu-id="e3893-127">Methods</span></span>

| <span data-ttu-id="e3893-128">Метод</span><span class="sxs-lookup"><span data-stu-id="e3893-128">Method</span></span>           | <span data-ttu-id="e3893-129">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e3893-129">Return Type</span></span>    |<span data-ttu-id="e3893-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e3893-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e3893-131">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="e3893-131">getRecentNotebooks</span></span>](../api/notebook_getrecentnotebooks.md) | <span data-ttu-id="e3893-132">Коллекция [notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="e3893-132">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="e3893-133">Получите коллекцию записных книжек, которые недавно открывал пользователь.</span><span class="sxs-lookup"><span data-stu-id="e3893-133">Get a collection of the most recently accessed notebooks for the user.</span></span> |
