# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="9307b-101">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="9307b-101">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="9307b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9307b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9307b-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9307b-103">Not yet documented</span></span>

<span data-ttu-id="9307b-104">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="9307b-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9307b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9307b-105">Properties</span></span>
|<span data-ttu-id="9307b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9307b-106">Property</span></span>|<span data-ttu-id="9307b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9307b-107">Type</span></span>|<span data-ttu-id="9307b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9307b-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9307b-109">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="9307b-109">scheduledInstallDay</span></span>|[<span data-ttu-id="9307b-110">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="9307b-110">weeklySchedule</span></span>](../resources/intune_deviceconfig_weeklyschedule.md)|<span data-ttu-id="9307b-111">День недели, запланированный для установки.</span><span class="sxs-lookup"><span data-stu-id="9307b-111">Scheduled Install Day in week Possible values are: , , , , , , , , .</span></span> <span data-ttu-id="9307b-112">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="9307b-112">The possible values are `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, , , or .</span></span>|
|<span data-ttu-id="9307b-113">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="9307b-113">scheduledInstallTime</span></span>|<span data-ttu-id="9307b-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9307b-114">TimeOfDay</span></span>|<span data-ttu-id="9307b-115">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="9307b-115">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="9307b-116">Связи</span><span class="sxs-lookup"><span data-stu-id="9307b-116">Relationships</span></span>
<span data-ttu-id="9307b-117">Нет</span><span class="sxs-lookup"><span data-stu-id="9307b-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9307b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9307b-118">JSON Representation</span></span>
<span data-ttu-id="9307b-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9307b-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.windowsUpdateInstallScheduleType",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```



