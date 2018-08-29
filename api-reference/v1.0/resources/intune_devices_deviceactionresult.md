# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="ba96c-101">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="ba96c-101">deviceActionResult resource type</span></span>

> <span data-ttu-id="ba96c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ba96c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ba96c-103">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="ba96c-103">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="ba96c-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba96c-104">Properties</span></span>
|<span data-ttu-id="ba96c-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba96c-105">Property</span></span>|<span data-ttu-id="ba96c-106">Тип</span><span class="sxs-lookup"><span data-stu-id="ba96c-106">Type</span></span>|<span data-ttu-id="ba96c-107">Описание</span><span class="sxs-lookup"><span data-stu-id="ba96c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba96c-108">actionName</span><span class="sxs-lookup"><span data-stu-id="ba96c-108">actionName</span></span>|<span data-ttu-id="ba96c-109">Строка</span><span class="sxs-lookup"><span data-stu-id="ba96c-109">String</span></span>|<span data-ttu-id="ba96c-110">Название действия</span><span class="sxs-lookup"><span data-stu-id="ba96c-110">Action name</span></span>|
|<span data-ttu-id="ba96c-111">actionState</span><span class="sxs-lookup"><span data-stu-id="ba96c-111">actionState</span></span>|[<span data-ttu-id="ba96c-112">actionState</span><span class="sxs-lookup"><span data-stu-id="ba96c-112">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="ba96c-113">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="ba96c-113">State of the action on the device</span></span> <span data-ttu-id="ba96c-114">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="ba96c-114">The possible values are `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`, , , , , or .</span></span>|
|<span data-ttu-id="ba96c-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ba96c-115">startDateTime</span></span>|<span data-ttu-id="ba96c-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba96c-116">DateTimeOffset</span></span>|<span data-ttu-id="ba96c-117">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="ba96c-117">Time the action was initiated</span></span>|
|<span data-ttu-id="ba96c-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba96c-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="ba96c-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba96c-119">DateTimeOffset</span></span>|<span data-ttu-id="ba96c-120">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="ba96c-120">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba96c-121">Связи</span><span class="sxs-lookup"><span data-stu-id="ba96c-121">Relationships</span></span>
<span data-ttu-id="ba96c-122">Нет</span><span class="sxs-lookup"><span data-stu-id="ba96c-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ba96c-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba96c-123">JSON Representation</span></span>
<span data-ttu-id="ba96c-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba96c-124">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```



