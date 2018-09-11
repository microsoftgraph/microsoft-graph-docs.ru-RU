# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="b1566-101">Тип ресурса resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="b1566-101">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="b1566-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b1566-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1566-103">Результат сброса секретного кода</span><span class="sxs-lookup"><span data-stu-id="b1566-103">Reset passcode action result</span></span>

<span data-ttu-id="b1566-104">Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b1566-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b1566-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b1566-105">Properties</span></span>
|<span data-ttu-id="b1566-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1566-106">Property</span></span>|<span data-ttu-id="b1566-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b1566-107">Type</span></span>|<span data-ttu-id="b1566-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b1566-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1566-109">actionName</span><span class="sxs-lookup"><span data-stu-id="b1566-109">actionName</span></span>|<span data-ttu-id="b1566-110">Строка</span><span class="sxs-lookup"><span data-stu-id="b1566-110">String</span></span>|<span data-ttu-id="b1566-111">Название действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b1566-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="b1566-112">actionState</span><span class="sxs-lookup"><span data-stu-id="b1566-112">actionState</span></span>|[<span data-ttu-id="b1566-113">actionState</span><span class="sxs-lookup"><span data-stu-id="b1566-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="b1566-p101">Состояние действия наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md). Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="b1566-p101">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b1566-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b1566-116">startDateTime</span></span>|<span data-ttu-id="b1566-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1566-117">DateTimeOffset</span></span>|<span data-ttu-id="b1566-118">Время начала действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b1566-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="b1566-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1566-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="b1566-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1566-120">DateTimeOffset</span></span>|<span data-ttu-id="b1566-121">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b1566-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="b1566-122">passcode</span><span class="sxs-lookup"><span data-stu-id="b1566-122">passcode</span></span>|<span data-ttu-id="b1566-123">Строка</span><span class="sxs-lookup"><span data-stu-id="b1566-123">String</span></span>|<span data-ttu-id="b1566-124">Новый секретный код для устройства</span><span class="sxs-lookup"><span data-stu-id="b1566-124">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="b1566-125">Связи</span><span class="sxs-lookup"><span data-stu-id="b1566-125">Relationships</span></span>
<span data-ttu-id="b1566-126">Нет</span><span class="sxs-lookup"><span data-stu-id="b1566-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b1566-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b1566-127">JSON Representation</span></span>
<span data-ttu-id="b1566-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1566-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resetPasscodeActionResult"
}-->
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








