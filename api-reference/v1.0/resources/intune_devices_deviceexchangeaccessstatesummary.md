# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="2a617-101">Тип ресурса deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="2a617-101">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="2a617-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2a617-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a617-103">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="2a617-103">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="2a617-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a617-104">Properties</span></span>
|<span data-ttu-id="2a617-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a617-105">Property</span></span>|<span data-ttu-id="2a617-106">Тип</span><span class="sxs-lookup"><span data-stu-id="2a617-106">Type</span></span>|<span data-ttu-id="2a617-107">Описание</span><span class="sxs-lookup"><span data-stu-id="2a617-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a617-108">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a617-108">allowedDeviceCount</span></span>|<span data-ttu-id="2a617-109">Int32</span><span class="sxs-lookup"><span data-stu-id="2a617-109">Int32</span></span>|<span data-ttu-id="2a617-110">Общее количество устройств с состоянием доступа к Exchange "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="2a617-110">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="2a617-111">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a617-111">blockedDeviceCount</span></span>|<span data-ttu-id="2a617-112">Int32</span><span class="sxs-lookup"><span data-stu-id="2a617-112">Int32</span></span>|<span data-ttu-id="2a617-113">Общее количество устройств с состоянием доступа к Exchange "Заблокировано".</span><span class="sxs-lookup"><span data-stu-id="2a617-113">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="2a617-114">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a617-114">quarantinedDeviceCount</span></span>|<span data-ttu-id="2a617-115">Int32</span><span class="sxs-lookup"><span data-stu-id="2a617-115">Int32</span></span>|<span data-ttu-id="2a617-116">Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".</span><span class="sxs-lookup"><span data-stu-id="2a617-116">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="2a617-117">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a617-117">unknownDeviceCount</span></span>|<span data-ttu-id="2a617-118">Int32</span><span class="sxs-lookup"><span data-stu-id="2a617-118">Int32</span></span>|<span data-ttu-id="2a617-119">Общее количество устройств с состоянием доступа к Exchange "Неизвестно".</span><span class="sxs-lookup"><span data-stu-id="2a617-119">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="2a617-120">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a617-120">unavailableDeviceCount</span></span>|<span data-ttu-id="2a617-121">Int32</span><span class="sxs-lookup"><span data-stu-id="2a617-121">Int32</span></span>|<span data-ttu-id="2a617-122">Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.</span><span class="sxs-lookup"><span data-stu-id="2a617-122">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a617-123">Связи</span><span class="sxs-lookup"><span data-stu-id="2a617-123">Relationships</span></span>
<span data-ttu-id="2a617-124">Нет</span><span class="sxs-lookup"><span data-stu-id="2a617-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2a617-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a617-125">JSON Representation</span></span>
<span data-ttu-id="2a617-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a617-126">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": 1024,
  "blockedDeviceCount": 1024,
  "quarantinedDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "unavailableDeviceCount": 1024
}
```








