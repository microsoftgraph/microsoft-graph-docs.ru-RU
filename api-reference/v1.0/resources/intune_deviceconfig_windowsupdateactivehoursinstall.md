# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="b63eb-101">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="b63eb-101">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="b63eb-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b63eb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b63eb-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b63eb-103">Not yet documented</span></span>

<span data-ttu-id="b63eb-104">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="b63eb-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b63eb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b63eb-105">Properties</span></span>
|<span data-ttu-id="b63eb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b63eb-106">Property</span></span>|<span data-ttu-id="b63eb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b63eb-107">Type</span></span>|<span data-ttu-id="b63eb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b63eb-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b63eb-109">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="b63eb-109">activeHoursStart</span></span>|<span data-ttu-id="b63eb-110">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b63eb-110">TimeOfDay</span></span>|<span data-ttu-id="b63eb-111">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="b63eb-111">Active Hours Start</span></span>|
|<span data-ttu-id="b63eb-112">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="b63eb-112">activeHoursEnd</span></span>|<span data-ttu-id="b63eb-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b63eb-113">TimeOfDay</span></span>|<span data-ttu-id="b63eb-114">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="b63eb-114">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="b63eb-115">Связи</span><span class="sxs-lookup"><span data-stu-id="b63eb-115">Relationships</span></span>
<span data-ttu-id="b63eb-116">Нет</span><span class="sxs-lookup"><span data-stu-id="b63eb-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b63eb-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b63eb-117">JSON Representation</span></span>
<span data-ttu-id="b63eb-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b63eb-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



