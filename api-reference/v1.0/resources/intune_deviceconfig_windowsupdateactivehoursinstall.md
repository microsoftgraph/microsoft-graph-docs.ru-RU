# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="d060f-101">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="d060f-101">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="d060f-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d060f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d060f-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d060f-103">Not yet documented</span></span>

<span data-ttu-id="d060f-104">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="d060f-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d060f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d060f-105">Properties</span></span>
|<span data-ttu-id="d060f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d060f-106">Property</span></span>|<span data-ttu-id="d060f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d060f-107">Type</span></span>|<span data-ttu-id="d060f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d060f-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d060f-109">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="d060f-109">activeHoursStart</span></span>|<span data-ttu-id="d060f-110">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d060f-110">TimeOfDay</span></span>|<span data-ttu-id="d060f-111">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="d060f-111">Active Hours Start</span></span>|
|<span data-ttu-id="d060f-112">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="d060f-112">activeHoursEnd</span></span>|<span data-ttu-id="d060f-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d060f-113">TimeOfDay</span></span>|<span data-ttu-id="d060f-114">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="d060f-114">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="d060f-115">Связи</span><span class="sxs-lookup"><span data-stu-id="d060f-115">Relationships</span></span>
<span data-ttu-id="d060f-116">Нет</span><span class="sxs-lookup"><span data-stu-id="d060f-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d060f-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d060f-117">JSON Representation</span></span>
<span data-ttu-id="d060f-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d060f-118">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.windowsUpdateInstallScheduleType",
  "@odata.type": "microsoft.graph.windowsUpdateActiveHoursInstall"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateActiveHoursInstall",
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)"
}
```



