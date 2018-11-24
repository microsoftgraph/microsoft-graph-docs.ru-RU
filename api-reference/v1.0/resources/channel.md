# <a name="channel-resource-type"></a><span data-ttu-id="722df-101">Тип ресурса канала</span><span class="sxs-lookup"><span data-stu-id="722df-101">channel resource type</span></span>



<span data-ttu-id="722df-102">Канал представляет коллекцию сообщений в пределах [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="722df-102">A channel is a collection of messages within a [team](../resources/team.md).</span></span> <span data-ttu-id="722df-103">Канал представляет раздел и логическая изоляции обсуждения в группе.</span><span class="sxs-lookup"><span data-stu-id="722df-103">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="722df-104">Примеры может быть канала «Пятница Lunch группы» и «Архитектура обсуждений» канала.</span><span class="sxs-lookup"><span data-stu-id="722df-104">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="722df-105">Методы</span><span class="sxs-lookup"><span data-stu-id="722df-105">Methods</span></span>

| <span data-ttu-id="722df-106">Метод</span><span class="sxs-lookup"><span data-stu-id="722df-106">Method</span></span>       | <span data-ttu-id="722df-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="722df-107">Return Type</span></span>  |<span data-ttu-id="722df-108">Описание</span><span class="sxs-lookup"><span data-stu-id="722df-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="722df-109">Список каналов</span><span class="sxs-lookup"><span data-stu-id="722df-109">List channels</span></span>](../api/channel_list.md) | <span data-ttu-id="722df-110">Коллекция [канала](channel.md)</span><span class="sxs-lookup"><span data-stu-id="722df-110">[channel](channel.md) collection</span></span> | <span data-ttu-id="722df-111">Получите список каналов в данной группы.</span><span class="sxs-lookup"><span data-stu-id="722df-111">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="722df-112">Создание канала</span><span class="sxs-lookup"><span data-stu-id="722df-112">Create channel</span></span>](../api/channel_post.md) | [<span data-ttu-id="722df-113">канал</span><span class="sxs-lookup"><span data-stu-id="722df-113">channel</span></span>](channel.md) | <span data-ttu-id="722df-114">Создайте новый канал, включая отображаемое имя и описание.</span><span class="sxs-lookup"><span data-stu-id="722df-114">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="722df-115">Получение канала</span><span class="sxs-lookup"><span data-stu-id="722df-115">Get channel</span></span>](../api/channel_get.md) | [<span data-ttu-id="722df-116">канал</span><span class="sxs-lookup"><span data-stu-id="722df-116">channel</span></span>](channel.md) | <span data-ttu-id="722df-117">Чтение свойства и связи канала.</span><span class="sxs-lookup"><span data-stu-id="722df-117">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="722df-118">Обновление канала</span><span class="sxs-lookup"><span data-stu-id="722df-118">Update channel</span></span>](../api/channel_patch.md) | [<span data-ttu-id="722df-119">канал</span><span class="sxs-lookup"><span data-stu-id="722df-119">channel</span></span>](channel.md) | <span data-ttu-id="722df-120">Обновление свойств канала.</span><span class="sxs-lookup"><span data-stu-id="722df-120">Update properties of the channel.</span></span>|
|[<span data-ttu-id="722df-121">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="722df-121">Delete channel</span></span>](../api/channel_delete.md) | <span data-ttu-id="722df-122">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="722df-122">None</span></span> | <span data-ttu-id="722df-123">Удаление канала.</span><span class="sxs-lookup"><span data-stu-id="722df-123">Delete a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="722df-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="722df-124">Properties</span></span>
| <span data-ttu-id="722df-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="722df-125">Property</span></span>     | <span data-ttu-id="722df-126">Тип</span><span class="sxs-lookup"><span data-stu-id="722df-126">Type</span></span>   |<span data-ttu-id="722df-127">Описание</span><span class="sxs-lookup"><span data-stu-id="722df-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="722df-128">описание</span><span class="sxs-lookup"><span data-stu-id="722df-128">description</span></span>|<span data-ttu-id="722df-129">String</span><span class="sxs-lookup"><span data-stu-id="722df-129">String</span></span>|<span data-ttu-id="722df-130">Необязательное текстовое описание для канала.</span><span class="sxs-lookup"><span data-stu-id="722df-130">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="722df-131">displayName</span><span class="sxs-lookup"><span data-stu-id="722df-131">displayName</span></span>|<span data-ttu-id="722df-132">String</span><span class="sxs-lookup"><span data-stu-id="722df-132">String</span></span>|<span data-ttu-id="722df-133">Имя канала, как оно будет отображаться для пользователей в группах Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="722df-133">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="722df-134">id</span><span class="sxs-lookup"><span data-stu-id="722df-134">id</span></span>|<span data-ttu-id="722df-135">String</span><span class="sxs-lookup"><span data-stu-id="722df-135">String</span></span>|<span data-ttu-id="722df-136">Уникальный идентификатор, каналов.</span><span class="sxs-lookup"><span data-stu-id="722df-136">The channels's unique identifier.</span></span> <span data-ttu-id="722df-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="722df-137">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="722df-138">Связи</span><span class="sxs-lookup"><span data-stu-id="722df-138">Relationships</span></span>
| <span data-ttu-id="722df-139">Связь</span><span class="sxs-lookup"><span data-stu-id="722df-139">Relationship</span></span> | <span data-ttu-id="722df-140">Тип</span><span class="sxs-lookup"><span data-stu-id="722df-140">Type</span></span>   |<span data-ttu-id="722df-141">Описание</span><span class="sxs-lookup"><span data-stu-id="722df-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="722df-142">вкладки</span><span class="sxs-lookup"><span data-stu-id="722df-142">tabs</span></span>|<span data-ttu-id="722df-143">[teamsTab](../resources/teamstab.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="722df-143">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="722df-144">Коллекция всех вкладок в канале.</span><span class="sxs-lookup"><span data-stu-id="722df-144">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="722df-145">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="722df-145">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="722df-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="722df-146">JSON representation</span></span>

<span data-ttu-id="722df-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="722df-147">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
