# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="9330a-101">Тип ресурса remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="9330a-101">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="9330a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9330a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9330a-103">Результат блокирования с ПИН-кодом разблокировки</span><span class="sxs-lookup"><span data-stu-id="9330a-103">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="9330a-104">Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9330a-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9330a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9330a-105">Properties</span></span>
|<span data-ttu-id="9330a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9330a-106">Property</span></span>|<span data-ttu-id="9330a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9330a-107">Type</span></span>|<span data-ttu-id="9330a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9330a-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9330a-109">actionName</span><span class="sxs-lookup"><span data-stu-id="9330a-109">actionName</span></span>|<span data-ttu-id="9330a-110">String (строка)</span><span class="sxs-lookup"><span data-stu-id="9330a-110">String</span></span>|<span data-ttu-id="9330a-111">Название действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9330a-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="9330a-112">actionState</span><span class="sxs-lookup"><span data-stu-id="9330a-112">actionState</span></span>|[<span data-ttu-id="9330a-113">actionState</span><span class="sxs-lookup"><span data-stu-id="9330a-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="9330a-p101">Состояние действия наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md). Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="9330a-p101">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9330a-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9330a-116">startDateTime</span></span>|<span data-ttu-id="9330a-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9330a-117">DateTimeOffset</span></span>|<span data-ttu-id="9330a-118">Время начала действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9330a-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="9330a-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9330a-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="9330a-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9330a-120">DateTimeOffset</span></span>|<span data-ttu-id="9330a-121">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9330a-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="9330a-122">unlockPin</span><span class="sxs-lookup"><span data-stu-id="9330a-122">unlockPin</span></span>|<span data-ttu-id="9330a-123">String (строка)</span><span class="sxs-lookup"><span data-stu-id="9330a-123">String</span></span>|<span data-ttu-id="9330a-124">ПИН-код для разблокировки клиента</span><span class="sxs-lookup"><span data-stu-id="9330a-124">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="9330a-125">Связи</span><span class="sxs-lookup"><span data-stu-id="9330a-125">Relationships</span></span>
<span data-ttu-id="9330a-126">Нет</span><span class="sxs-lookup"><span data-stu-id="9330a-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9330a-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9330a-127">JSON Representation</span></span>
<span data-ttu-id="9330a-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9330a-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.remoteLockActionResult"
}-->
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








