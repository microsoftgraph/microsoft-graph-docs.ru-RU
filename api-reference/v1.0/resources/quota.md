# <a name="quota-resource-type"></a><span data-ttu-id="746c9-101">Тип ресурса quota</span><span class="sxs-lookup"><span data-stu-id="746c9-101">Quota resource type</span></span>

<span data-ttu-id="746c9-102">Ресурс **quota** предоставляет сведения об ограничениях дискового пространства в ресурсе [Drive](drive.md).</span><span class="sxs-lookup"><span data-stu-id="746c9-102">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="746c9-103">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="746c9-103">JSON representation</span></span>

<span data-ttu-id="746c9-104">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="746c9-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.quota"
}-->

```json
{
  "deleted": 1024,
  "remaining": 1024,
  "state": "normal | nearing | critical | exceeded",
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a><span data-ttu-id="746c9-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="746c9-105">Properties</span></span>

| <span data-ttu-id="746c9-106">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="746c9-106">Property name</span></span> | <span data-ttu-id="746c9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="746c9-107">Type</span></span>   | <span data-ttu-id="746c9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="746c9-108">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="746c9-109">total</span><span class="sxs-lookup"><span data-stu-id="746c9-109">total</span></span>         | <span data-ttu-id="746c9-110">Int64</span><span class="sxs-lookup"><span data-stu-id="746c9-110">Int64</span></span>  | <span data-ttu-id="746c9-p101">Общий объем разрешенного дискового пространства в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="746c9-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="746c9-113">used</span><span class="sxs-lookup"><span data-stu-id="746c9-113">used</span></span>          | <span data-ttu-id="746c9-114">Int64</span><span class="sxs-lookup"><span data-stu-id="746c9-114">Int64</span></span>  | <span data-ttu-id="746c9-p102">Общий объем использованного дискового пространства в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="746c9-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="746c9-117">remaining</span><span class="sxs-lookup"><span data-stu-id="746c9-117">remaining</span></span>     | <span data-ttu-id="746c9-118">Int64</span><span class="sxs-lookup"><span data-stu-id="746c9-118">Int64</span></span>  | <span data-ttu-id="746c9-p103">Общий объем дискового пространства, оставшегося до достижения максимальной квоты, в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="746c9-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="746c9-121">deleted</span><span class="sxs-lookup"><span data-stu-id="746c9-121">deleted</span></span>       | <span data-ttu-id="746c9-122">Int64</span><span class="sxs-lookup"><span data-stu-id="746c9-122">Int64</span></span>  | <span data-ttu-id="746c9-p104">Общий объем дискового пространства, занятого файлами в корзине, в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="746c9-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="746c9-125">состояние</span><span class="sxs-lookup"><span data-stu-id="746c9-125">state</span></span>         | <span data-ttu-id="746c9-126">string</span><span class="sxs-lookup"><span data-stu-id="746c9-126">string</span></span> | <span data-ttu-id="746c9-p105">Значение перечисления, указывающее состояние дискового пространства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="746c9-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |

## <a name="state-enumeration"></a><span data-ttu-id="746c9-129">Перечисление state</span><span class="sxs-lookup"><span data-stu-id="746c9-129">State Enumeration</span></span>

| <span data-ttu-id="746c9-130">Значение</span><span class="sxs-lookup"><span data-stu-id="746c9-130">Value</span></span>      | <span data-ttu-id="746c9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="746c9-131">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="746c9-132">На диске еще много свободного дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="746c9-132">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="746c9-133">Объем свободного дискового пространства менее 10 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="746c9-133">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="746c9-134">Объем свободного дискового пространства менее 1 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="746c9-134">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="746c9-p106">Объем использованного дискового пространства превышает максимально допустимый объем дискового пространства. Вам не удастся добавлять новые файлы или папки на диск, пока объем использованного дискового пространства не станет меньше общего объема дискового пространства или пока вы не приобретете дополнительное дисковое пространство.</span><span class="sxs-lookup"><span data-stu-id="746c9-p106">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "quota resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
