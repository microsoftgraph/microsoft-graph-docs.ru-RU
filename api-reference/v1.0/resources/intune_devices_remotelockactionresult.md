# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="8e2f4-101">Тип ресурса remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="8e2f4-101">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="8e2f4-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8e2f4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e2f4-103">Результат блокирования с ПИН-кодом разблокировки</span><span class="sxs-lookup"><span data-stu-id="8e2f4-103">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="8e2f4-104">Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8e2f4-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8e2f4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e2f4-105">Properties</span></span>
|<span data-ttu-id="8e2f4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e2f4-106">Property</span></span>|<span data-ttu-id="8e2f4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8e2f4-107">Type</span></span>|<span data-ttu-id="8e2f4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8e2f4-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e2f4-109">actionName</span><span class="sxs-lookup"><span data-stu-id="8e2f4-109">actionName</span></span>|<span data-ttu-id="8e2f4-110">String (строка)</span><span class="sxs-lookup"><span data-stu-id="8e2f4-110">String</span></span>|<span data-ttu-id="8e2f4-111">Название действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8e2f4-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="8e2f4-112">actionState</span><span class="sxs-lookup"><span data-stu-id="8e2f4-112">actionState</span></span>|[<span data-ttu-id="8e2f4-113">actionState</span><span class="sxs-lookup"><span data-stu-id="8e2f4-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="8e2f4-114">|||UNTRANSLATED_CONTENT_START|||State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md).|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="8e2f4-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: , , , , , , .</span></span> <span data-ttu-id="8e2f4-115">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="8e2f4-115">The possible values are `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`, , , , , or .</span></span>|
|<span data-ttu-id="8e2f4-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8e2f4-116">startDateTime</span></span>|<span data-ttu-id="8e2f4-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e2f4-117">DateTimeOffset</span></span>|<span data-ttu-id="8e2f4-118">Время начала действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8e2f4-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="8e2f4-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e2f4-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="8e2f4-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e2f4-120">DateTimeOffset</span></span>|<span data-ttu-id="8e2f4-121">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8e2f4-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="8e2f4-122">unlockPin</span><span class="sxs-lookup"><span data-stu-id="8e2f4-122">unlockPin</span></span>|<span data-ttu-id="8e2f4-123">String (строка)</span><span class="sxs-lookup"><span data-stu-id="8e2f4-123">String</span></span>|<span data-ttu-id="8e2f4-124">ПИН-код для разблокировки клиента</span><span class="sxs-lookup"><span data-stu-id="8e2f4-124">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e2f4-125">Связи</span><span class="sxs-lookup"><span data-stu-id="8e2f4-125">Relationships</span></span>
<span data-ttu-id="8e2f4-126">Нет</span><span class="sxs-lookup"><span data-stu-id="8e2f4-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8e2f4-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e2f4-127">JSON Representation</span></span>
<span data-ttu-id="8e2f4-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e2f4-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceActionResult",
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



