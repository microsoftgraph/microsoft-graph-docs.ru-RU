# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="51193-101">Тип ресурса iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="51193-101">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="51193-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="51193-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51193-103">Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="51193-103">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="51193-104">Наследуется от [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="51193-104">Inherits from [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="51193-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="51193-105">Properties</span></span>
|<span data-ttu-id="51193-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="51193-106">Property</span></span>|<span data-ttu-id="51193-107">Тип</span><span class="sxs-lookup"><span data-stu-id="51193-107">Type</span></span>|<span data-ttu-id="51193-108">Описание</span><span class="sxs-lookup"><span data-stu-id="51193-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51193-109">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="51193-109">useDeviceLicensing</span></span>|<span data-ttu-id="51193-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="51193-110">Boolean</span></span>|<span data-ttu-id="51193-111">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="51193-111">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="51193-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="51193-112">vpnConfigurationId</span></span>|<span data-ttu-id="51193-113">String</span><span class="sxs-lookup"><span data-stu-id="51193-113">String</span></span>|<span data-ttu-id="51193-114">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="51193-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51193-115">Связи</span><span class="sxs-lookup"><span data-stu-id="51193-115">Relationships</span></span>
<span data-ttu-id="51193-116">Нет</span><span class="sxs-lookup"><span data-stu-id="51193-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="51193-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51193-117">JSON Representation</span></span>
<span data-ttu-id="51193-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51193-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.mobileAppAssignmentSettings",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String"
}
```



