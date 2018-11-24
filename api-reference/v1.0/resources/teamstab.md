# <a name="teamstab-resource-type"></a><span data-ttu-id="863a1-101">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="863a1-101">teamsTab resource type</span></span>



<span data-ttu-id="863a1-102">TeamsTab — [вкладку](../resources/teamstab.md) , которая прикрепленных (вложенный) [канала](channel.md) в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="863a1-102">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="863a1-103">Методы</span><span class="sxs-lookup"><span data-stu-id="863a1-103">Methods</span></span>

| <span data-ttu-id="863a1-104">Метод</span><span class="sxs-lookup"><span data-stu-id="863a1-104">Method</span></span>       | <span data-ttu-id="863a1-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="863a1-105">Return Type</span></span>  |<span data-ttu-id="863a1-106">Описание</span><span class="sxs-lookup"><span data-stu-id="863a1-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="863a1-107">Список вкладок</span><span class="sxs-lookup"><span data-stu-id="863a1-107">List tabs</span></span>](../api/teamstab_list.md) | [<span data-ttu-id="863a1-108">teamsTab</span><span class="sxs-lookup"><span data-stu-id="863a1-108">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="863a1-109">Списки вкладок прикрепленных к каналу.</span><span class="sxs-lookup"><span data-stu-id="863a1-109">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="863a1-110">Получить вкладки</span><span class="sxs-lookup"><span data-stu-id="863a1-110">Get tab</span></span>](../api/teamstab_get.md) | [<span data-ttu-id="863a1-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="863a1-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="863a1-112">Считывает вкладки, прикрепленных к каналу.</span><span class="sxs-lookup"><span data-stu-id="863a1-112">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="863a1-113">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="863a1-113">Add tab</span></span>](../api/teamstab_add.md) | [<span data-ttu-id="863a1-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="863a1-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="863a1-115">Добавляет (PIN) вкладки на канал.</span><span class="sxs-lookup"><span data-stu-id="863a1-115">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="863a1-116">Удалить вкладку ""</span><span class="sxs-lookup"><span data-stu-id="863a1-116">Remove tab</span></span>](../api/teamstab_delete.md) | <span data-ttu-id="863a1-117">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="863a1-117">None</span></span> | <span data-ttu-id="863a1-118">Удаляет (отключит) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="863a1-118">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="863a1-119">Вкладка "обновления"</span><span class="sxs-lookup"><span data-stu-id="863a1-119">Update tab</span></span>](../api/teamstab_update.md) | [<span data-ttu-id="863a1-120">teamsTab</span><span class="sxs-lookup"><span data-stu-id="863a1-120">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="863a1-121">Обновляет свойства вкладки.</span><span class="sxs-lookup"><span data-stu-id="863a1-121">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="863a1-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="863a1-122">Properties</span></span>

|<span data-ttu-id="863a1-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="863a1-123">Property</span></span>|<span data-ttu-id="863a1-124">Тип</span><span class="sxs-lookup"><span data-stu-id="863a1-124">Type</span></span>|<span data-ttu-id="863a1-125">Описание</span><span class="sxs-lookup"><span data-stu-id="863a1-125">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="863a1-126">id</span><span class="sxs-lookup"><span data-stu-id="863a1-126">id</span></span>              |   <span data-ttu-id="863a1-127">строка</span><span class="sxs-lookup"><span data-stu-id="863a1-127">string</span></span>                  |  <span data-ttu-id="863a1-128">Идентификатор, который уникальным образом определяет определенный экземпляр канала вкладку чтения только.</span><span class="sxs-lookup"><span data-stu-id="863a1-128">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="863a1-129">displayName</span><span class="sxs-lookup"><span data-stu-id="863a1-129">displayName</span></span>            |   <span data-ttu-id="863a1-130">строка</span><span class="sxs-lookup"><span data-stu-id="863a1-130">string</span></span>                  |  <span data-ttu-id="863a1-131">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="863a1-131">Name of the tab.</span></span>     |
|  <span data-ttu-id="863a1-132">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="863a1-132">sortOrderIndex</span></span>  |   <span data-ttu-id="863a1-133">целое</span><span class="sxs-lookup"><span data-stu-id="863a1-133">int</span></span>                     |  <span data-ttu-id="863a1-134">Индекс порядок, используемый для сортировки вкладок</span><span class="sxs-lookup"><span data-stu-id="863a1-134">Index of the order used for sorting tabs</span></span>     |
|  <span data-ttu-id="863a1-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="863a1-135">webUrl</span></span>          |   <span data-ttu-id="863a1-136">string</span><span class="sxs-lookup"><span data-stu-id="863a1-136">string</span></span>                  |  <span data-ttu-id="863a1-137">Прямая ссылка URL-адрес экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="863a1-137">Deep link url of the tab instance.</span></span> <span data-ttu-id="863a1-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="863a1-138">Read only.</span></span>     |
|  <span data-ttu-id="863a1-139">configuration</span><span class="sxs-lookup"><span data-stu-id="863a1-139">configuration</span></span>        |   [<span data-ttu-id="863a1-140">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="863a1-140">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="863a1-141">Контейнер для пользовательских параметров, применяемых на вкладке. Вкладка считается настроены только после этого свойства.</span><span class="sxs-lookup"><span data-stu-id="863a1-141">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="863a1-142">Связи</span><span class="sxs-lookup"><span data-stu-id="863a1-142">Relationships</span></span>

| <span data-ttu-id="863a1-143">Связь</span><span class="sxs-lookup"><span data-stu-id="863a1-143">Relationship</span></span> | <span data-ttu-id="863a1-144">Тип</span><span class="sxs-lookup"><span data-stu-id="863a1-144">Type</span></span>   | <span data-ttu-id="863a1-145">Описание</span><span class="sxs-lookup"><span data-stu-id="863a1-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="863a1-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="863a1-146">teamsApp</span></span>|[<span data-ttu-id="863a1-147">teamsApp</span><span class="sxs-lookup"><span data-stu-id="863a1-147">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="863a1-148">Приложения, связанного с вкладки. Это нельзя изменить после создания вкладки.</span><span class="sxs-lookup"><span data-stu-id="863a1-148">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="863a1-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="863a1-149">JSON representation</span></span>

<span data-ttu-id="863a1-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="863a1-150">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
  "sortOrderIndex": "string",
  "webUrl": "string",
  "configuration" : "teamsTabConfiguration"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="863a1-151">См. также</span><span class="sxs-lookup"><span data-stu-id="863a1-151">See also</span></span>

[<span data-ttu-id="863a1-152">Настройка типов встроенную вкладку</span><span class="sxs-lookup"><span data-stu-id="863a1-152">Configuring the built-in tab types</span></span>](../../../concepts/teams-configuring-builtin-tabs.md)
