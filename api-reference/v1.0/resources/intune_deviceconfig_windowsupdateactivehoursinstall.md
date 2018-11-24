# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="2f2d5-101">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="2f2d5-101">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="2f2d5-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2f2d5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f2d5-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2f2d5-103">Not yet documented</span></span>

<span data-ttu-id="2f2d5-104">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="2f2d5-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2f2d5-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f2d5-105">Properties</span></span>
|<span data-ttu-id="2f2d5-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f2d5-106">Property</span></span>|<span data-ttu-id="2f2d5-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2f2d5-107">Type</span></span>|<span data-ttu-id="2f2d5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2f2d5-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f2d5-109">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="2f2d5-109">activeHoursStart</span></span>|<span data-ttu-id="2f2d5-110">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2f2d5-110">TimeOfDay</span></span>|<span data-ttu-id="2f2d5-111">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="2f2d5-111">Active Hours Start</span></span>|
|<span data-ttu-id="2f2d5-112">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="2f2d5-112">activeHoursEnd</span></span>|<span data-ttu-id="2f2d5-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2f2d5-113">TimeOfDay</span></span>|<span data-ttu-id="2f2d5-114">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="2f2d5-114">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f2d5-115">Связи</span><span class="sxs-lookup"><span data-stu-id="2f2d5-115">Relationships</span></span>
<span data-ttu-id="2f2d5-116">Нет</span><span class="sxs-lookup"><span data-stu-id="2f2d5-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2f2d5-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f2d5-117">JSON Representation</span></span>
<span data-ttu-id="2f2d5-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f2d5-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateActiveHoursInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateActiveHoursInstall",
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)"
}
```



