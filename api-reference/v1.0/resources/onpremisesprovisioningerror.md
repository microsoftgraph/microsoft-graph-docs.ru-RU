# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="db0bd-101">Тип ресурса onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="db0bd-101">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="db0bd-102">Представляет ошибки синхронизации службы каталогов для [пользователей](user.md) и [групп](group.md) сущностей при синхронизации локальных каталогов в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="db0bd-102">Represents directory synchronization errors for the [user](user.md) and [group](group.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="db0bd-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="db0bd-103">Properties</span></span>

| <span data-ttu-id="db0bd-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="db0bd-104">Property</span></span> | <span data-ttu-id="db0bd-105">Тип</span><span class="sxs-lookup"><span data-stu-id="db0bd-105">Type</span></span> | <span data-ttu-id="db0bd-106">Описание</span><span class="sxs-lookup"><span data-stu-id="db0bd-106">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="db0bd-107">category</span><span class="sxs-lookup"><span data-stu-id="db0bd-107">category</span></span>|<span data-ttu-id="db0bd-108">String</span><span class="sxs-lookup"><span data-stu-id="db0bd-108">String</span></span>| <span data-ttu-id="db0bd-109">Категория ошибки подготовки.</span><span class="sxs-lookup"><span data-stu-id="db0bd-109">Category of the provisioning error.</span></span> <span data-ttu-id="db0bd-110">Примечание: в настоящее время доступно только одно значение.</span><span class="sxs-lookup"><span data-stu-id="db0bd-110">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="db0bd-111">Возможные значения: *PropertyConflict* - указывает, что значение свойства не является уникальным.</span><span class="sxs-lookup"><span data-stu-id="db0bd-111">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="db0bd-112">Такое же значение для свойства содержат другие объекты.</span><span class="sxs-lookup"><span data-stu-id="db0bd-112">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="db0bd-113">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="db0bd-113">occurredDateTime</span></span>|<span data-ttu-id="db0bd-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db0bd-114">DateTimeOffset</span></span>| <span data-ttu-id="db0bd-115">Дата и время возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="db0bd-115">The time at which the error occurred.</span></span> |
|<span data-ttu-id="db0bd-116">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="db0bd-116">propertyCausingError</span></span>|<span data-ttu-id="db0bd-117">String</span><span class="sxs-lookup"><span data-stu-id="db0bd-117">String</span></span>| <span data-ttu-id="db0bd-118">Имя свойства каталогов, вызвавшего ошибку.</span><span class="sxs-lookup"><span data-stu-id="db0bd-118">Name of the directory property causing the error.</span></span> <span data-ttu-id="db0bd-119">Текущие возможные значения: *UserPrincipalName* или *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="db0bd-119">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="db0bd-120">value</span><span class="sxs-lookup"><span data-stu-id="db0bd-120">value</span></span>|<span data-ttu-id="db0bd-121">String</span><span class="sxs-lookup"><span data-stu-id="db0bd-121">String</span></span>| <span data-ttu-id="db0bd-122">Значение свойства, вызвавшего ошибку.</span><span class="sxs-lookup"><span data-stu-id="db0bd-122">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="db0bd-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db0bd-123">JSON representation</span></span>
<span data-ttu-id="db0bd-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db0bd-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->