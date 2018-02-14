# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="41d48-101">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="41d48-101">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="41d48-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="41d48-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41d48-103">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="41d48-103">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="41d48-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="41d48-104">Properties</span></span>
|<span data-ttu-id="41d48-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="41d48-105">Property</span></span>|<span data-ttu-id="41d48-106">Тип</span><span class="sxs-lookup"><span data-stu-id="41d48-106">Type</span></span>|<span data-ttu-id="41d48-107">Описание</span><span class="sxs-lookup"><span data-stu-id="41d48-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41d48-108">androidCount</span><span class="sxs-lookup"><span data-stu-id="41d48-108">androidCount</span></span>|<span data-ttu-id="41d48-109">Int32</span><span class="sxs-lookup"><span data-stu-id="41d48-109">Int32</span></span>|<span data-ttu-id="41d48-110">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="41d48-110">Number of android device count.</span></span>|
|<span data-ttu-id="41d48-111">iosCount</span><span class="sxs-lookup"><span data-stu-id="41d48-111">iosCount</span></span>|<span data-ttu-id="41d48-112">Int32</span><span class="sxs-lookup"><span data-stu-id="41d48-112">Int32</span></span>|<span data-ttu-id="41d48-113">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="41d48-113">Number of iOS device count.</span></span>|
|<span data-ttu-id="41d48-114">macOSCount</span><span class="sxs-lookup"><span data-stu-id="41d48-114">macOSCount</span></span>|<span data-ttu-id="41d48-115">Int32</span><span class="sxs-lookup"><span data-stu-id="41d48-115">Int32</span></span>|<span data-ttu-id="41d48-116">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="41d48-116">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="41d48-117">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="41d48-117">windowsMobileCount</span></span>|<span data-ttu-id="41d48-118">Int32</span><span class="sxs-lookup"><span data-stu-id="41d48-118">Int32</span></span>|<span data-ttu-id="41d48-119">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="41d48-119">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="41d48-120">windowsCount</span><span class="sxs-lookup"><span data-stu-id="41d48-120">windowsCount</span></span>|<span data-ttu-id="41d48-121">Int32</span><span class="sxs-lookup"><span data-stu-id="41d48-121">Int32</span></span>|<span data-ttu-id="41d48-122">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="41d48-122">Number of Windows device count.</span></span>|
|<span data-ttu-id="41d48-123">unknownCount</span><span class="sxs-lookup"><span data-stu-id="41d48-123">unknownCount</span></span>|<span data-ttu-id="41d48-124">Int32</span><span class="sxs-lookup"><span data-stu-id="41d48-124">Int32</span></span>|<span data-ttu-id="41d48-125">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="41d48-125">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41d48-126">Связи</span><span class="sxs-lookup"><span data-stu-id="41d48-126">Relationships</span></span>
<span data-ttu-id="41d48-127">Нет</span><span class="sxs-lookup"><span data-stu-id="41d48-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="41d48-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="41d48-128">JSON Representation</span></span>
<span data-ttu-id="41d48-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41d48-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024
}
```



