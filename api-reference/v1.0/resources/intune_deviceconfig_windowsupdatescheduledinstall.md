# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="0fc22-101">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="0fc22-101">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="0fc22-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0fc22-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0fc22-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0fc22-103">Not yet documented</span></span>

<span data-ttu-id="0fc22-104">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="0fc22-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0fc22-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0fc22-105">Properties</span></span>
|<span data-ttu-id="0fc22-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0fc22-106">Property</span></span>|<span data-ttu-id="0fc22-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0fc22-107">Type</span></span>|<span data-ttu-id="0fc22-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0fc22-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fc22-109">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="0fc22-109">scheduledInstallDay</span></span>|[<span data-ttu-id="0fc22-110">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="0fc22-110">weeklySchedule</span></span>](../resources/intune_deviceconfig_weeklyschedule.md)|<span data-ttu-id="0fc22-p101">Запланированный день установки. Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="0fc22-p101">Scheduled Install Day in week Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="0fc22-113">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="0fc22-113">scheduledInstallTime</span></span>|<span data-ttu-id="0fc22-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0fc22-114">TimeOfDay</span></span>|<span data-ttu-id="0fc22-115">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="0fc22-115">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fc22-116">Связи</span><span class="sxs-lookup"><span data-stu-id="0fc22-116">Relationships</span></span>
<span data-ttu-id="0fc22-117">Нет</span><span class="sxs-lookup"><span data-stu-id="0fc22-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0fc22-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0fc22-118">JSON Representation</span></span>
<span data-ttu-id="0fc22-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0fc22-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```








