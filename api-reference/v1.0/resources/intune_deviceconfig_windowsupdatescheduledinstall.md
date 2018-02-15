# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="e98f2-101">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="e98f2-101">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="e98f2-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e98f2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e98f2-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e98f2-103">Not yet documented</span></span>

<span data-ttu-id="e98f2-104">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="e98f2-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e98f2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e98f2-105">Properties</span></span>
|<span data-ttu-id="e98f2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e98f2-106">Property</span></span>|<span data-ttu-id="e98f2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e98f2-107">Type</span></span>|<span data-ttu-id="e98f2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e98f2-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e98f2-109">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="e98f2-109">scheduledInstallDay</span></span>|<span data-ttu-id="e98f2-110">String</span><span class="sxs-lookup"><span data-stu-id="e98f2-110">String</span></span>|<span data-ttu-id="e98f2-111">День недели, на который запланирована установка. Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="e98f2-111">Scheduled Install Day in week Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="e98f2-112">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="e98f2-112">scheduledInstallTime</span></span>|<span data-ttu-id="e98f2-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="e98f2-113">TimeOfDay</span></span>|<span data-ttu-id="e98f2-114">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="e98f2-114">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="e98f2-115">Связи</span><span class="sxs-lookup"><span data-stu-id="e98f2-115">Relationships</span></span>
<span data-ttu-id="e98f2-116">Нет</span><span class="sxs-lookup"><span data-stu-id="e98f2-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e98f2-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e98f2-117">JSON Representation</span></span>
<span data-ttu-id="e98f2-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e98f2-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```



