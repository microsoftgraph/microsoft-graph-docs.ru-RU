# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="a2227-101">Тип ресурса iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="a2227-101">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="a2227-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a2227-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2227-103">Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="a2227-103">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="a2227-104">Наследуется от [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a2227-104">Inherits from [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a2227-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2227-105">Properties</span></span>
|<span data-ttu-id="a2227-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2227-106">Property</span></span>|<span data-ttu-id="a2227-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a2227-107">Type</span></span>|<span data-ttu-id="a2227-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a2227-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2227-109">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="a2227-109">vpnConfigurationId</span></span>|<span data-ttu-id="a2227-110">String</span><span class="sxs-lookup"><span data-stu-id="a2227-110">String</span></span>|<span data-ttu-id="a2227-111">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="a2227-111">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2227-112">Связи</span><span class="sxs-lookup"><span data-stu-id="a2227-112">Relationships</span></span>
<span data-ttu-id="a2227-113">Нет</span><span class="sxs-lookup"><span data-stu-id="a2227-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a2227-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a2227-114">JSON Representation</span></span>
<span data-ttu-id="a2227-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2227-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.mobileAppAssignmentSettings",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```



