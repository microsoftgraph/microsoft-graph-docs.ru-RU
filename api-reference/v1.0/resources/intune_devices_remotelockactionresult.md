# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="bd7a3-101">Тип ресурса remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="bd7a3-101">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="bd7a3-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bd7a3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd7a3-103">Результат блокирования с ПИН-кодом разблокировки</span><span class="sxs-lookup"><span data-stu-id="bd7a3-103">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="bd7a3-104">Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bd7a3-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bd7a3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd7a3-105">Properties</span></span>
|<span data-ttu-id="bd7a3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd7a3-106">Property</span></span>|<span data-ttu-id="bd7a3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="bd7a3-107">Type</span></span>|<span data-ttu-id="bd7a3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="bd7a3-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd7a3-109">actionName</span><span class="sxs-lookup"><span data-stu-id="bd7a3-109">actionName</span></span>|<span data-ttu-id="bd7a3-110">String</span><span class="sxs-lookup"><span data-stu-id="bd7a3-110">String</span></span>|<span data-ttu-id="bd7a3-111">Название действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bd7a3-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="bd7a3-112">actionState</span><span class="sxs-lookup"><span data-stu-id="bd7a3-112">actionState</span></span>|<span data-ttu-id="bd7a3-113">String</span><span class="sxs-lookup"><span data-stu-id="bd7a3-113">String</span></span>|<span data-ttu-id="bd7a3-114">Состояние действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md). Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="bd7a3-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="bd7a3-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bd7a3-115">startDateTime</span></span>|<span data-ttu-id="bd7a3-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd7a3-116">DateTimeOffset</span></span>|<span data-ttu-id="bd7a3-117">Время начала действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bd7a3-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="bd7a3-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd7a3-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="bd7a3-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd7a3-119">DateTimeOffset</span></span>|<span data-ttu-id="bd7a3-120">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bd7a3-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="bd7a3-121">unlockPin</span><span class="sxs-lookup"><span data-stu-id="bd7a3-121">unlockPin</span></span>|<span data-ttu-id="bd7a3-122">String</span><span class="sxs-lookup"><span data-stu-id="bd7a3-122">String</span></span>|<span data-ttu-id="bd7a3-123">ПИН-код для разблокировки клиента</span><span class="sxs-lookup"><span data-stu-id="bd7a3-123">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd7a3-124">Связи</span><span class="sxs-lookup"><span data-stu-id="bd7a3-124">Relationships</span></span>
<span data-ttu-id="bd7a3-125">Нет</span><span class="sxs-lookup"><span data-stu-id="bd7a3-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bd7a3-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd7a3-126">JSON Representation</span></span>
<span data-ttu-id="bd7a3-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd7a3-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteLockActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteLockActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "unlockPin": "String"
}
```



