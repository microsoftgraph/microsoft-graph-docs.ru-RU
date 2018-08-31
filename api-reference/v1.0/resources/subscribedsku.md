# <a name="subscribedsku-resource-type"></a><span data-ttu-id="74913-101">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="74913-101">subscribedSku resource type</span></span>

<span data-ttu-id="74913-102">Содержит сведения о сервисе SKU, на который подписана компания.</span><span class="sxs-lookup"><span data-stu-id="74913-102">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="74913-p101">В подписанных SKU поддерживается только операция чтения. Создание, обновление и удаление не поддерживаются. Выражения фильтра запроса не поддерживаются. Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="74913-p101">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="74913-106">Методы</span><span class="sxs-lookup"><span data-stu-id="74913-106">Methods</span></span>
| <span data-ttu-id="74913-107">Метод</span><span class="sxs-lookup"><span data-stu-id="74913-107">Method</span></span>           | <span data-ttu-id="74913-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="74913-108">Return Type</span></span>    |<span data-ttu-id="74913-109">Описание</span><span class="sxs-lookup"><span data-stu-id="74913-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="74913-110">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="74913-110">Get subscribedSku</span></span>](../api/subscribedsku_get.md) | [<span data-ttu-id="74913-111">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="74913-111">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="74913-112">Чтение свойств и связей объекта subscribedSku.</span><span class="sxs-lookup"><span data-stu-id="74913-112">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="74913-113">Список  subscribedsku</span><span class="sxs-lookup"><span data-stu-id="74913-113">List subscribedSku</span></span>](../api/subscribedsku_list.md) | <span data-ttu-id="74913-114">Коллекция [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="74913-114">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="74913-115">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="74913-115">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="74913-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="74913-116">Properties</span></span>
| <span data-ttu-id="74913-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="74913-117">Property</span></span>     | <span data-ttu-id="74913-118">Тип</span><span class="sxs-lookup"><span data-stu-id="74913-118">Type</span></span>   |<span data-ttu-id="74913-119">Описание</span><span class="sxs-lookup"><span data-stu-id="74913-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74913-120">appliesTo</span><span class="sxs-lookup"><span data-stu-id="74913-120">appliesTo</span></span>|<span data-ttu-id="74913-121">String (строка)</span><span class="sxs-lookup"><span data-stu-id="74913-121">String</span></span>| <span data-ttu-id="74913-122">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="74913-122">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="74913-123">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="74913-123">capabilityStatus</span></span>|<span data-ttu-id="74913-124">String (строка)</span><span class="sxs-lookup"><span data-stu-id="74913-124">String</span></span>| <span data-ttu-id="74913-125">Например, Enabled.</span><span class="sxs-lookup"><span data-stu-id="74913-125">For example, "Enabled".</span></span> |
|<span data-ttu-id="74913-126">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="74913-126">consumedUnits</span></span>|<span data-ttu-id="74913-127">Int32</span><span class="sxs-lookup"><span data-stu-id="74913-127">Int32</span></span>| <span data-ttu-id="74913-128">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="74913-128">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="74913-129">id</span><span class="sxs-lookup"><span data-stu-id="74913-129">id</span></span>|<span data-ttu-id="74913-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="74913-130">String</span></span>| <span data-ttu-id="74913-p102">Уникальный идентификатор объекта sku, подписка на который выполнена. Ключ, значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="74913-p102">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="74913-133">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="74913-133">prepaidUnits</span></span>|[<span data-ttu-id="74913-134">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="74913-134">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="74913-135">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="74913-135">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="74913-136">servicePlans</span><span class="sxs-lookup"><span data-stu-id="74913-136">servicePlans</span></span>|<span data-ttu-id="74913-137">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="74913-137">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="74913-p103">Сведения о планах обслуживания, доступных в отношении SKU. Значение NULL не допускается</span><span class="sxs-lookup"><span data-stu-id="74913-p103">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="74913-140">skuId</span><span class="sxs-lookup"><span data-stu-id="74913-140">skuId</span></span>|<span data-ttu-id="74913-141">Guid</span><span class="sxs-lookup"><span data-stu-id="74913-141">Guid</span></span>| <span data-ttu-id="74913-142">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="74913-142">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="74913-143">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="74913-143">skuPartNumber</span></span>|<span data-ttu-id="74913-144">String (строка)</span><span class="sxs-lookup"><span data-stu-id="74913-144">String</span></span>| <span data-ttu-id="74913-145">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="74913-145">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="74913-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="74913-146">Relationships</span></span>
<span data-ttu-id="74913-147">Нет</span><span class="sxs-lookup"><span data-stu-id="74913-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74913-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74913-148">JSON representation</span></span>

<span data-ttu-id="74913-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74913-149">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscribedSku",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "appliesTo": "string",
  "capabilityStatus": "string",
  "consumedUnits": 1024,
  "id": "string (identifier)",
  "prepaidUnits": {"@odata.type": "microsoft.graph.licenseUnitsDetail"},
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "guid",
  "skuPartNumber": "string"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
