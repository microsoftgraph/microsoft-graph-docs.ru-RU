# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="1b4f8-101">Тип ресурса windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="1b4f8-101">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="1b4f8-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1b4f8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b4f8-103">Результат последнего сканирования, выполненного Защитником Windows</span><span class="sxs-lookup"><span data-stu-id="1b4f8-103">Windows Defender last scan result</span></span>

<span data-ttu-id="1b4f8-104">Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1b4f8-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1b4f8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b4f8-105">Properties</span></span>
|<span data-ttu-id="1b4f8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b4f8-106">Property</span></span>|<span data-ttu-id="1b4f8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1b4f8-107">Type</span></span>|<span data-ttu-id="1b4f8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1b4f8-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b4f8-109">actionName</span><span class="sxs-lookup"><span data-stu-id="1b4f8-109">actionName</span></span>|<span data-ttu-id="1b4f8-110">String</span><span class="sxs-lookup"><span data-stu-id="1b4f8-110">String</span></span>|<span data-ttu-id="1b4f8-111">Название действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="1b4f8-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="1b4f8-112">actionState</span><span class="sxs-lookup"><span data-stu-id="1b4f8-112">actionState</span></span>|[<span data-ttu-id="1b4f8-113">actionState</span><span class="sxs-lookup"><span data-stu-id="1b4f8-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="1b4f8-114">Состояние действие унаследованные от [deviceActionResult](../resources/intune_devices_deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="1b4f8-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md).</span></span> <span data-ttu-id="1b4f8-115">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="1b4f8-115">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1b4f8-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1b4f8-116">startDateTime</span></span>|<span data-ttu-id="1b4f8-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b4f8-117">DateTimeOffset</span></span>|<span data-ttu-id="1b4f8-118">Время начала действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1b4f8-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="1b4f8-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b4f8-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="1b4f8-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b4f8-120">DateTimeOffset</span></span>|<span data-ttu-id="1b4f8-121">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="1b4f8-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="1b4f8-122">scanType</span><span class="sxs-lookup"><span data-stu-id="1b4f8-122">scanType</span></span>|<span data-ttu-id="1b4f8-123">String</span><span class="sxs-lookup"><span data-stu-id="1b4f8-123">String</span></span>|<span data-ttu-id="1b4f8-124">Тип сканирования (полное или краткое).</span><span class="sxs-lookup"><span data-stu-id="1b4f8-124">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b4f8-125">Связи</span><span class="sxs-lookup"><span data-stu-id="1b4f8-125">Relationships</span></span>
<span data-ttu-id="1b4f8-126">None</span><span class="sxs-lookup"><span data-stu-id="1b4f8-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1b4f8-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1b4f8-127">JSON Representation</span></span>
<span data-ttu-id="1b4f8-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b4f8-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult"
}
-->
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



