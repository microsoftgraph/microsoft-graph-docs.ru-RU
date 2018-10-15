# <a name="profilephoto-resource-type"></a><span data-ttu-id="b75c6-101">Тип ресурса profilePhoto</span><span class="sxs-lookup"><span data-stu-id="b75c6-101">profilePhoto resource type</span></span>
<span data-ttu-id="b75c6-p101">Фотография профиля пользователя, группы или контакта Outlook из Exchange Online. Это двоичные данные, не представленные в кодировке base-64.</span><span class="sxs-lookup"><span data-stu-id="b75c6-p101">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="b75c6-104">Поддерживаемые размеры фотографий в формате HD для Exchange Online: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 и 648x648.</span><span class="sxs-lookup"><span data-stu-id="b75c6-104">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="b75c6-105">Методы</span><span class="sxs-lookup"><span data-stu-id="b75c6-105">Methods</span></span>

| <span data-ttu-id="b75c6-106">Метод</span><span class="sxs-lookup"><span data-stu-id="b75c6-106">Method</span></span>       | <span data-ttu-id="b75c6-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b75c6-107">Return Type</span></span>  |<span data-ttu-id="b75c6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b75c6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b75c6-109">Получение объекта profilePhoto</span><span class="sxs-lookup"><span data-stu-id="b75c6-109">Get profilePhoto</span></span>](../api/profilephoto_get.md) | [<span data-ttu-id="b75c6-110">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="b75c6-110">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="b75c6-111">Получение указанного объекта **profilePhoto** или его метаданных (свойств profilePhoto).</span><span class="sxs-lookup"><span data-stu-id="b75c6-111">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="b75c6-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="b75c6-112">Update</span></span>](../api/profilephoto_update.md) | [<span data-ttu-id="b75c6-113">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="b75c6-113">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="b75c6-p102">Назначение фотографии указанному пользователю, группе или контакту. Фотография должна быть представлена в двоичном формате. Она заменяет текущую фотографию (если она существует).</span><span class="sxs-lookup"><span data-stu-id="b75c6-p102">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="b75c6-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="b75c6-117">Properties</span></span>
| <span data-ttu-id="b75c6-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="b75c6-118">Property</span></span>     | <span data-ttu-id="b75c6-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b75c6-119">Type</span></span>   |<span data-ttu-id="b75c6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b75c6-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b75c6-121">id</span><span class="sxs-lookup"><span data-stu-id="b75c6-121">id</span></span>|<span data-ttu-id="b75c6-122">строка</span><span class="sxs-lookup"><span data-stu-id="b75c6-122">string</span></span>|<span data-ttu-id="b75c6-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b75c6-123">Read-only.</span></span>|
|<span data-ttu-id="b75c6-124">height</span><span class="sxs-lookup"><span data-stu-id="b75c6-124">height</span></span>|<span data-ttu-id="b75c6-125">int32</span><span class="sxs-lookup"><span data-stu-id="b75c6-125">int32</span></span>|<span data-ttu-id="b75c6-p103">Высота фотографии. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b75c6-p103">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="b75c6-128">width</span><span class="sxs-lookup"><span data-stu-id="b75c6-128">width</span></span>|<span data-ttu-id="b75c6-129">int32</span><span class="sxs-lookup"><span data-stu-id="b75c6-129">int32</span></span>|<span data-ttu-id="b75c6-p104">Ширина фотографии. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b75c6-p104">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b75c6-132">Связи</span><span class="sxs-lookup"><span data-stu-id="b75c6-132">Relationships</span></span>
<span data-ttu-id="b75c6-133">Нет</span><span class="sxs-lookup"><span data-stu-id="b75c6-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b75c6-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b75c6-134">JSON representation</span></span>

<span data-ttu-id="b75c6-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b75c6-135">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "isMediaEntity": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profilePhoto"
}-->

```json
{
  "id": "240X240",
  "height": 240,
  "width": 240
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
