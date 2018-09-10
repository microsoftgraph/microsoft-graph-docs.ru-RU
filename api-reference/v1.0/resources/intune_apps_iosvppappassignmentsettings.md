# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="9369b-101">Тип ресурса iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="9369b-101">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="9369b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9369b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9369b-103">Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="9369b-103">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="9369b-104">Наследуется от [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="9369b-104">Inherits from [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9369b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9369b-105">Properties</span></span>
|<span data-ttu-id="9369b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9369b-106">Property</span></span>|<span data-ttu-id="9369b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9369b-107">Type</span></span>|<span data-ttu-id="9369b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9369b-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9369b-109">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="9369b-109">useDeviceLicensing</span></span>|<span data-ttu-id="9369b-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="9369b-110">Boolean</span></span>|<span data-ttu-id="9369b-111">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="9369b-111">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="9369b-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="9369b-112">vpnConfigurationId</span></span>|<span data-ttu-id="9369b-113">String</span><span class="sxs-lookup"><span data-stu-id="9369b-113">String</span></span>|<span data-ttu-id="9369b-114">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="9369b-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9369b-115">Связи</span><span class="sxs-lookup"><span data-stu-id="9369b-115">Relationships</span></span>
<span data-ttu-id="9369b-116">Нет</span><span class="sxs-lookup"><span data-stu-id="9369b-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9369b-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9369b-117">JSON Representation</span></span>
<span data-ttu-id="9369b-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9369b-118">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String"
}
```








