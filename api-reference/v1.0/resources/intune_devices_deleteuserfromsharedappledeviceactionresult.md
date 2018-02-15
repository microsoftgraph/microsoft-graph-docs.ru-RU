# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="dca2d-101">Тип ресурса deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="dca2d-101">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="dca2d-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dca2d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dca2d-103">Результат удаления пользователя с общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="dca2d-103">Delete user from shared apple device action result</span></span>

<span data-ttu-id="dca2d-104">Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="dca2d-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dca2d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="dca2d-105">Properties</span></span>
|<span data-ttu-id="dca2d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="dca2d-106">Property</span></span>|<span data-ttu-id="dca2d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="dca2d-107">Type</span></span>|<span data-ttu-id="dca2d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="dca2d-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dca2d-109">actionName</span><span class="sxs-lookup"><span data-stu-id="dca2d-109">actionName</span></span>|<span data-ttu-id="dca2d-110">String</span><span class="sxs-lookup"><span data-stu-id="dca2d-110">String</span></span>|<span data-ttu-id="dca2d-111">Название действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="dca2d-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="dca2d-112">actionState</span><span class="sxs-lookup"><span data-stu-id="dca2d-112">actionState</span></span>|<span data-ttu-id="dca2d-113">String</span><span class="sxs-lookup"><span data-stu-id="dca2d-113">String</span></span>|<span data-ttu-id="dca2d-114">Состояние действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md). Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="dca2d-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="dca2d-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="dca2d-115">startDateTime</span></span>|<span data-ttu-id="dca2d-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dca2d-116">DateTimeOffset</span></span>|<span data-ttu-id="dca2d-117">Время начала действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="dca2d-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="dca2d-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="dca2d-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="dca2d-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dca2d-119">DateTimeOffset</span></span>|<span data-ttu-id="dca2d-120">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="dca2d-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="dca2d-121">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dca2d-121">userPrincipalName</span></span>|<span data-ttu-id="dca2d-122">String</span><span class="sxs-lookup"><span data-stu-id="dca2d-122">String</span></span>|<span data-ttu-id="dca2d-123">Имя участника-пользователя для удаляемого пользователя</span><span class="sxs-lookup"><span data-stu-id="dca2d-123">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="dca2d-124">Связи</span><span class="sxs-lookup"><span data-stu-id="dca2d-124">Relationships</span></span>
<span data-ttu-id="dca2d-125">Нет</span><span class="sxs-lookup"><span data-stu-id="dca2d-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dca2d-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dca2d-126">JSON Representation</span></span>
<span data-ttu-id="dca2d-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dca2d-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



