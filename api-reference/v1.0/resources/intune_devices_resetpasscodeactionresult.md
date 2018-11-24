# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="c2d55-101">Тип ресурса resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="c2d55-101">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="c2d55-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c2d55-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2d55-103">Результат сброса секретного кода</span><span class="sxs-lookup"><span data-stu-id="c2d55-103">Reset passcode action result</span></span>

<span data-ttu-id="c2d55-104">Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c2d55-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c2d55-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2d55-105">Properties</span></span>
|<span data-ttu-id="c2d55-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2d55-106">Property</span></span>|<span data-ttu-id="c2d55-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c2d55-107">Type</span></span>|<span data-ttu-id="c2d55-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c2d55-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2d55-109">actionName</span><span class="sxs-lookup"><span data-stu-id="c2d55-109">actionName</span></span>|<span data-ttu-id="c2d55-110">String</span><span class="sxs-lookup"><span data-stu-id="c2d55-110">String</span></span>|<span data-ttu-id="c2d55-111">Название действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c2d55-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="c2d55-112">actionState</span><span class="sxs-lookup"><span data-stu-id="c2d55-112">actionState</span></span>|[<span data-ttu-id="c2d55-113">actionState</span><span class="sxs-lookup"><span data-stu-id="c2d55-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="c2d55-114">Состояние действие унаследованные от [deviceActionResult](../resources/intune_devices_deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c2d55-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md).</span></span> <span data-ttu-id="c2d55-115">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="c2d55-115">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c2d55-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c2d55-116">startDateTime</span></span>|<span data-ttu-id="c2d55-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2d55-117">DateTimeOffset</span></span>|<span data-ttu-id="c2d55-118">Время начала действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c2d55-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="c2d55-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2d55-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="c2d55-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2d55-120">DateTimeOffset</span></span>|<span data-ttu-id="c2d55-121">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c2d55-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="c2d55-122">passcode</span><span class="sxs-lookup"><span data-stu-id="c2d55-122">passcode</span></span>|<span data-ttu-id="c2d55-123">String</span><span class="sxs-lookup"><span data-stu-id="c2d55-123">String</span></span>|<span data-ttu-id="c2d55-124">Новый секретный код для устройства</span><span class="sxs-lookup"><span data-stu-id="c2d55-124">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="c2d55-125">Связи</span><span class="sxs-lookup"><span data-stu-id="c2d55-125">Relationships</span></span>
<span data-ttu-id="c2d55-126">None</span><span class="sxs-lookup"><span data-stu-id="c2d55-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c2d55-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2d55-127">JSON Representation</span></span>
<span data-ttu-id="c2d55-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2d55-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resetPasscodeActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resetPasscodeActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "passcode": "String"
}
```



