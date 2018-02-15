# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="96fa6-101">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="96fa6-101">deviceActionResult resource type</span></span>

> <span data-ttu-id="96fa6-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="96fa6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96fa6-103">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="96fa6-103">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="96fa6-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="96fa6-104">Properties</span></span>
|<span data-ttu-id="96fa6-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="96fa6-105">Property</span></span>|<span data-ttu-id="96fa6-106">Тип</span><span class="sxs-lookup"><span data-stu-id="96fa6-106">Type</span></span>|<span data-ttu-id="96fa6-107">Описание</span><span class="sxs-lookup"><span data-stu-id="96fa6-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96fa6-108">actionName</span><span class="sxs-lookup"><span data-stu-id="96fa6-108">actionName</span></span>|<span data-ttu-id="96fa6-109">String</span><span class="sxs-lookup"><span data-stu-id="96fa6-109">String</span></span>|<span data-ttu-id="96fa6-110">Название действия</span><span class="sxs-lookup"><span data-stu-id="96fa6-110">Action name</span></span>|
|<span data-ttu-id="96fa6-111">actionState</span><span class="sxs-lookup"><span data-stu-id="96fa6-111">actionState</span></span>|<span data-ttu-id="96fa6-112">String</span><span class="sxs-lookup"><span data-stu-id="96fa6-112">String</span></span>|<span data-ttu-id="96fa6-113">Состояние действия. Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="96fa6-113">State of the action Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="96fa6-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="96fa6-114">startDateTime</span></span>|<span data-ttu-id="96fa6-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96fa6-115">DateTimeOffset</span></span>|<span data-ttu-id="96fa6-116">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="96fa6-116">Time the action was initiated</span></span>|
|<span data-ttu-id="96fa6-117">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="96fa6-117">lastUpdatedDateTime</span></span>|<span data-ttu-id="96fa6-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96fa6-118">DateTimeOffset</span></span>|<span data-ttu-id="96fa6-119">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="96fa6-119">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="96fa6-120">Связи</span><span class="sxs-lookup"><span data-stu-id="96fa6-120">Relationships</span></span>
<span data-ttu-id="96fa6-121">Нет</span><span class="sxs-lookup"><span data-stu-id="96fa6-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="96fa6-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="96fa6-122">JSON Representation</span></span>
<span data-ttu-id="96fa6-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96fa6-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```



