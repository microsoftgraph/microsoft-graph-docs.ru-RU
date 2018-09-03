# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="1a782-101">Тип ресурса deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="1a782-101">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="1a782-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1a782-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a782-103">Результат удаления пользователя с общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="1a782-103">Delete user from shared apple device action result</span></span>

<span data-ttu-id="1a782-104">Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1a782-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1a782-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a782-105">Properties</span></span>
|<span data-ttu-id="1a782-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a782-106">Property</span></span>|<span data-ttu-id="1a782-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1a782-107">Type</span></span>|<span data-ttu-id="1a782-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1a782-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a782-109">actionName</span><span class="sxs-lookup"><span data-stu-id="1a782-109">actionName</span></span>|<span data-ttu-id="1a782-110">Строковый</span><span class="sxs-lookup"><span data-stu-id="1a782-110">String</span></span>|<span data-ttu-id="1a782-111">Название действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1a782-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="1a782-112">actionState</span><span class="sxs-lookup"><span data-stu-id="1a782-112">actionState</span></span>|[<span data-ttu-id="1a782-113">actionState</span><span class="sxs-lookup"><span data-stu-id="1a782-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="1a782-114">Состояние [ действия, унаследованного от deviceActionResult.](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1a782-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: , , , , , , .</span></span> <span data-ttu-id="1a782-115">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="1a782-115">The possible values are `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`, , , , , or .</span></span>|
|<span data-ttu-id="1a782-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1a782-116">startDateTime</span></span>|<span data-ttu-id="1a782-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a782-117">DateTimeOffset</span></span>|<span data-ttu-id="1a782-118">Время начала действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1a782-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="1a782-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a782-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="1a782-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a782-120">DateTimeOffset</span></span>|<span data-ttu-id="1a782-121">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1a782-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="1a782-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1a782-122">userPrincipalName</span></span>|<span data-ttu-id="1a782-123">Строковый</span><span class="sxs-lookup"><span data-stu-id="1a782-123">String</span></span>|<span data-ttu-id="1a782-124">Имя участника-пользователя для удаляемого пользователя</span><span class="sxs-lookup"><span data-stu-id="1a782-124">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a782-125">Связи</span><span class="sxs-lookup"><span data-stu-id="1a782-125">Relationships</span></span>
<span data-ttu-id="1a782-126">Нет</span><span class="sxs-lookup"><span data-stu-id="1a782-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1a782-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a782-127">JSON Representation</span></span>
<span data-ttu-id="1a782-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a782-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceActionResult",
  "@odata.type": "microsoft.graph.deleteUserFromSharedAppleDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deleteUserFromSharedAppleDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



