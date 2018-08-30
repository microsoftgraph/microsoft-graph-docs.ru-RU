# <a name="licensedetails-resource-type"></a><span data-ttu-id="31ac1-101">Тип ресурса licenseDetails</span><span class="sxs-lookup"><span data-stu-id="31ac1-101">licenseDetails resource type</span></span>

<span data-ttu-id="31ac1-102">Содержит сведения о лицензии, назначенной пользователю.</span><span class="sxs-lookup"><span data-stu-id="31ac1-102">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="31ac1-103">Методы</span><span class="sxs-lookup"><span data-stu-id="31ac1-103">Methods</span></span>

| <span data-ttu-id="31ac1-104">Метод</span><span class="sxs-lookup"><span data-stu-id="31ac1-104">Method</span></span>           | <span data-ttu-id="31ac1-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="31ac1-105">Return Type</span></span>    |<span data-ttu-id="31ac1-106">Описание</span><span class="sxs-lookup"><span data-stu-id="31ac1-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="31ac1-107">Перечисление licenseDetails</span><span class="sxs-lookup"><span data-stu-id="31ac1-107">List licenseDetails</span></span>](../api/user_list_licensedetails.md) | <span data-ttu-id="31ac1-108">Коллекция licenseDetails</span><span class="sxs-lookup"><span data-stu-id="31ac1-108">licenseDetails collection</span></span> |<span data-ttu-id="31ac1-109">Получение списка объектов licenseDetails для пользователя.</span><span class="sxs-lookup"><span data-stu-id="31ac1-109">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails_get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="31ac1-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="31ac1-110">Properties</span></span>
| <span data-ttu-id="31ac1-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="31ac1-111">Property</span></span>     | <span data-ttu-id="31ac1-112">Тип</span><span class="sxs-lookup"><span data-stu-id="31ac1-112">Type</span></span>   |<span data-ttu-id="31ac1-113">Описание</span><span class="sxs-lookup"><span data-stu-id="31ac1-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31ac1-114">id</span><span class="sxs-lookup"><span data-stu-id="31ac1-114">id</span></span>|<span data-ttu-id="31ac1-115">Строка</span><span class="sxs-lookup"><span data-stu-id="31ac1-115">String</span></span>| <span data-ttu-id="31ac1-p101">Уникальный идентификатор объекта сведений о лицензии. Только для чтения, ключевое, не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="31ac1-p101">The unique identifier for the license detail object. Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="31ac1-118">servicePlans</span><span class="sxs-lookup"><span data-stu-id="31ac1-118">servicePlans</span></span>|<span data-ttu-id="31ac1-119">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="31ac1-119">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="31ac1-p102">Сведения о планах обслуживания, назначенных вместе с лицензией. Только для чтения, не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="31ac1-p102">Information about the service plans assigned with the license. Read-only, Not nullable</span></span> |
|<span data-ttu-id="31ac1-122">skuId</span><span class="sxs-lookup"><span data-stu-id="31ac1-122">skuId</span></span>|<span data-ttu-id="31ac1-123">Guid</span><span class="sxs-lookup"><span data-stu-id="31ac1-123">Guid</span></span>| <span data-ttu-id="31ac1-p103">Уникальный идентификатор (GUID) для SKU службы. Имеет то же значение, что и свойство skuId в связанном объекте [SubscribedSku](subscribedsku.md). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31ac1-p103">Unique identifier (GUID) for the service SKU. Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object. Read-only</span></span> |
|<span data-ttu-id="31ac1-127">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="31ac1-127">skuPartNumber</span></span>|<span data-ttu-id="31ac1-128">Строка</span><span class="sxs-lookup"><span data-stu-id="31ac1-128">String</span></span>| <span data-ttu-id="31ac1-p104">Уникальное отображаемое имя SKU. Имеет то же значение, что и свойство skuPartNumber в связанном объекте [SubscribedSku](subscribedsku.md). Пример: AAD_Premium. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31ac1-p104">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="31ac1-132">Связи</span><span class="sxs-lookup"><span data-stu-id="31ac1-132">Relationships</span></span>
<span data-ttu-id="31ac1-133">Нет</span><span class="sxs-lookup"><span data-stu-id="31ac1-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="31ac1-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31ac1-134">JSON representation</span></span>
<span data-ttu-id="31ac1-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31ac1-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->