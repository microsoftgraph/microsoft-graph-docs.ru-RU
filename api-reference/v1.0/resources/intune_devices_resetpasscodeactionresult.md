# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="17453-101">Тип ресурса resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="17453-101">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="17453-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="17453-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17453-103">Результат сброса секретного кода</span><span class="sxs-lookup"><span data-stu-id="17453-103">Reset passcode action result</span></span>

<span data-ttu-id="17453-104">Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="17453-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="17453-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="17453-105">Properties</span></span>
|<span data-ttu-id="17453-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="17453-106">Property</span></span>|<span data-ttu-id="17453-107">Тип</span><span class="sxs-lookup"><span data-stu-id="17453-107">Type</span></span>|<span data-ttu-id="17453-108">Описание</span><span class="sxs-lookup"><span data-stu-id="17453-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17453-109">actionName</span><span class="sxs-lookup"><span data-stu-id="17453-109">actionName</span></span>|<span data-ttu-id="17453-110">String</span><span class="sxs-lookup"><span data-stu-id="17453-110">String</span></span>|<span data-ttu-id="17453-111">Название действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="17453-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="17453-112">actionState</span><span class="sxs-lookup"><span data-stu-id="17453-112">actionState</span></span>|<span data-ttu-id="17453-113">String</span><span class="sxs-lookup"><span data-stu-id="17453-113">String</span></span>|<span data-ttu-id="17453-114">Состояние действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md). Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="17453-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="17453-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="17453-115">startDateTime</span></span>|<span data-ttu-id="17453-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17453-116">DateTimeOffset</span></span>|<span data-ttu-id="17453-117">Время начала действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="17453-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="17453-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="17453-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="17453-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17453-119">DateTimeOffset</span></span>|<span data-ttu-id="17453-120">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="17453-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="17453-121">passcode</span><span class="sxs-lookup"><span data-stu-id="17453-121">passcode</span></span>|<span data-ttu-id="17453-122">String</span><span class="sxs-lookup"><span data-stu-id="17453-122">String</span></span>|<span data-ttu-id="17453-123">Новый секретный код для устройства</span><span class="sxs-lookup"><span data-stu-id="17453-123">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="17453-124">Связи</span><span class="sxs-lookup"><span data-stu-id="17453-124">Relationships</span></span>
<span data-ttu-id="17453-125">Нет</span><span class="sxs-lookup"><span data-stu-id="17453-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="17453-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="17453-126">JSON Representation</span></span>
<span data-ttu-id="17453-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17453-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



