# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="27f22-101">Тип ресурса importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="27f22-101">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="27f22-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="27f22-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27f22-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="27f22-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="27f22-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="27f22-104">Properties</span></span>
|<span data-ttu-id="27f22-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="27f22-105">Property</span></span>|<span data-ttu-id="27f22-106">Тип</span><span class="sxs-lookup"><span data-stu-id="27f22-106">Type</span></span>|<span data-ttu-id="27f22-107">Описание</span><span class="sxs-lookup"><span data-stu-id="27f22-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27f22-108">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="27f22-108">deviceImportStatus</span></span>|[<span data-ttu-id="27f22-109">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="27f22-109">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="27f22-110">Состояние устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="27f22-110">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="27f22-111">Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="27f22-111">The possible values are `unknown`, `pending`, `partial`, `complete`, `error`, , , , , , , or .</span></span>|
|<span data-ttu-id="27f22-112">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="27f22-112">deviceRegistrationId</span></span>|<span data-ttu-id="27f22-113">Строка</span><span class="sxs-lookup"><span data-stu-id="27f22-113">String</span></span>|<span data-ttu-id="27f22-114">Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="27f22-114">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="27f22-115">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="27f22-115">deviceErrorCode</span></span>|<span data-ttu-id="27f22-116">Int32</span><span class="sxs-lookup"><span data-stu-id="27f22-116">Int32</span></span>|<span data-ttu-id="27f22-117">Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="27f22-117">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="27f22-118">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="27f22-118">deviceErrorName</span></span>|<span data-ttu-id="27f22-119">Строка</span><span class="sxs-lookup"><span data-stu-id="27f22-119">String</span></span>|<span data-ttu-id="27f22-120">Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="27f22-120">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="27f22-121">Связи</span><span class="sxs-lookup"><span data-stu-id="27f22-121">Relationships</span></span>
<span data-ttu-id="27f22-122">Нет</span><span class="sxs-lookup"><span data-stu-id="27f22-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="27f22-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27f22-123">JSON Representation</span></span>
<span data-ttu-id="27f22-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27f22-124">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
  "deviceImportStatus": "String",
  "deviceRegistrationId": "String",
  "deviceErrorCode": 1024,
  "deviceErrorName": "String"
}
```



