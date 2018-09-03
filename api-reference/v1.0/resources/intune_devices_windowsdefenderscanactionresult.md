# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="68e58-101">Тип ресурса windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="68e58-101">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="68e58-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="68e58-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68e58-103">Результат последнего сканирования, выполненного Защитником Windows</span><span class="sxs-lookup"><span data-stu-id="68e58-103">Windows Defender last scan result</span></span>

<span data-ttu-id="68e58-104">Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="68e58-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="68e58-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="68e58-105">Properties</span></span>
|<span data-ttu-id="68e58-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="68e58-106">Property</span></span>|<span data-ttu-id="68e58-107">Тип</span><span class="sxs-lookup"><span data-stu-id="68e58-107">Type</span></span>|<span data-ttu-id="68e58-108">Описание</span><span class="sxs-lookup"><span data-stu-id="68e58-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68e58-109">actionName</span><span class="sxs-lookup"><span data-stu-id="68e58-109">actionName</span></span>|<span data-ttu-id="68e58-110">String (строка​)</span><span class="sxs-lookup"><span data-stu-id="68e58-110">String</span></span>|<span data-ttu-id="68e58-111">Название действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="68e58-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="68e58-112">actionState</span><span class="sxs-lookup"><span data-stu-id="68e58-112">actionState</span></span>|[<span data-ttu-id="68e58-113">actionState</span><span class="sxs-lookup"><span data-stu-id="68e58-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="68e58-114">Состояние действия унаследованного от [deviceActionResult](../resources/intune_devices_deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="68e58-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: , , , , , , .</span></span> <span data-ttu-id="68e58-115">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="68e58-115">The possible values are `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`, , , , , or .</span></span>|
|<span data-ttu-id="68e58-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="68e58-116">startDateTime</span></span>|<span data-ttu-id="68e58-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68e58-117">DateTimeOffset</span></span>|<span data-ttu-id="68e58-118">Время начала действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="68e58-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="68e58-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="68e58-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="68e58-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68e58-120">DateTimeOffset</span></span>|<span data-ttu-id="68e58-121">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="68e58-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="68e58-122">scanType</span><span class="sxs-lookup"><span data-stu-id="68e58-122">scanType</span></span>|<span data-ttu-id="68e58-123">String (строка​)</span><span class="sxs-lookup"><span data-stu-id="68e58-123">String</span></span>|<span data-ttu-id="68e58-124">Тип сканирования (полное или краткое).</span><span class="sxs-lookup"><span data-stu-id="68e58-124">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="68e58-125">Связи</span><span class="sxs-lookup"><span data-stu-id="68e58-125">Relationships</span></span>
<span data-ttu-id="68e58-126">Нет</span><span class="sxs-lookup"><span data-stu-id="68e58-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="68e58-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="68e58-127">JSON Representation</span></span>
<span data-ttu-id="68e58-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68e58-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceActionResult",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderScanActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "scanType": "String"
}
```



