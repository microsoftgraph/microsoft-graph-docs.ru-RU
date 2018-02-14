# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="896e6-101">Тип ресурса windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="896e6-101">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="896e6-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="896e6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="896e6-103">Результат последнего сканирования, выполненного Защитником Windows</span><span class="sxs-lookup"><span data-stu-id="896e6-103">Windows Defender last scan result</span></span>

<span data-ttu-id="896e6-104">Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="896e6-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="896e6-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="896e6-105">Properties</span></span>
|<span data-ttu-id="896e6-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="896e6-106">Property</span></span>|<span data-ttu-id="896e6-107">Тип</span><span class="sxs-lookup"><span data-stu-id="896e6-107">Type</span></span>|<span data-ttu-id="896e6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="896e6-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="896e6-109">actionName</span><span class="sxs-lookup"><span data-stu-id="896e6-109">actionName</span></span>|<span data-ttu-id="896e6-110">String</span><span class="sxs-lookup"><span data-stu-id="896e6-110">String</span></span>|<span data-ttu-id="896e6-111">Название действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="896e6-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="896e6-112">actionState</span><span class="sxs-lookup"><span data-stu-id="896e6-112">actionState</span></span>|<span data-ttu-id="896e6-113">String</span><span class="sxs-lookup"><span data-stu-id="896e6-113">String</span></span>|<span data-ttu-id="896e6-114">Состояние действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md). Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="896e6-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="896e6-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="896e6-115">startDateTime</span></span>|<span data-ttu-id="896e6-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="896e6-116">DateTimeOffset</span></span>|<span data-ttu-id="896e6-117">Время начала действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="896e6-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="896e6-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="896e6-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="896e6-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="896e6-119">DateTimeOffset</span></span>|<span data-ttu-id="896e6-120">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="896e6-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="896e6-121">scanType</span><span class="sxs-lookup"><span data-stu-id="896e6-121">scanType</span></span>|<span data-ttu-id="896e6-122">String</span><span class="sxs-lookup"><span data-stu-id="896e6-122">String</span></span>|<span data-ttu-id="896e6-123">Тип сканирования (полное или краткое).</span><span class="sxs-lookup"><span data-stu-id="896e6-123">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="896e6-124">Связи</span><span class="sxs-lookup"><span data-stu-id="896e6-124">Relationships</span></span>
<span data-ttu-id="896e6-125">Отсутствуют</span><span class="sxs-lookup"><span data-stu-id="896e6-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="896e6-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="896e6-126">JSON Representation</span></span>
<span data-ttu-id="896e6-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="896e6-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



