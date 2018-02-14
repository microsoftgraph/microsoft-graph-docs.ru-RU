# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="fda96-101">Тип ресурса deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="fda96-101">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="fda96-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fda96-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fda96-103">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="fda96-103">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="fda96-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="fda96-104">Properties</span></span>
|<span data-ttu-id="fda96-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="fda96-105">Property</span></span>|<span data-ttu-id="fda96-106">Тип</span><span class="sxs-lookup"><span data-stu-id="fda96-106">Type</span></span>|<span data-ttu-id="fda96-107">Описание</span><span class="sxs-lookup"><span data-stu-id="fda96-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fda96-108">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fda96-108">allowedDeviceCount</span></span>|<span data-ttu-id="fda96-109">Int32</span><span class="sxs-lookup"><span data-stu-id="fda96-109">Int32</span></span>|<span data-ttu-id="fda96-110">Общее количество устройств с состоянием доступа к Exchange "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="fda96-110">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="fda96-111">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fda96-111">blockedDeviceCount</span></span>|<span data-ttu-id="fda96-112">Int32</span><span class="sxs-lookup"><span data-stu-id="fda96-112">Int32</span></span>|<span data-ttu-id="fda96-113">Общее количество устройств с состоянием доступа к Exchange "Заблокировано".</span><span class="sxs-lookup"><span data-stu-id="fda96-113">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="fda96-114">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fda96-114">quarantinedDeviceCount</span></span>|<span data-ttu-id="fda96-115">Int32</span><span class="sxs-lookup"><span data-stu-id="fda96-115">Int32</span></span>|<span data-ttu-id="fda96-116">Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".</span><span class="sxs-lookup"><span data-stu-id="fda96-116">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="fda96-117">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fda96-117">unknownDeviceCount</span></span>|<span data-ttu-id="fda96-118">Int32</span><span class="sxs-lookup"><span data-stu-id="fda96-118">Int32</span></span>|<span data-ttu-id="fda96-119">Общее количество устройств с состоянием доступа к Exchange "Неизвестно".</span><span class="sxs-lookup"><span data-stu-id="fda96-119">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="fda96-120">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fda96-120">unavailableDeviceCount</span></span>|<span data-ttu-id="fda96-121">Int32</span><span class="sxs-lookup"><span data-stu-id="fda96-121">Int32</span></span>|<span data-ttu-id="fda96-122">Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.</span><span class="sxs-lookup"><span data-stu-id="fda96-122">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fda96-123">Связи</span><span class="sxs-lookup"><span data-stu-id="fda96-123">Relationships</span></span>
<span data-ttu-id="fda96-124">Нет</span><span class="sxs-lookup"><span data-stu-id="fda96-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fda96-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fda96-125">JSON Representation</span></span>
<span data-ttu-id="fda96-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fda96-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}
-->
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



