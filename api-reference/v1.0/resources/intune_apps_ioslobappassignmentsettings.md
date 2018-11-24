# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="2157b-101">Тип ресурса iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="2157b-101">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="2157b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2157b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2157b-103">Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="2157b-103">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="2157b-104">Наследуется от [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="2157b-104">Inherits from [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2157b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2157b-105">Properties</span></span>
|<span data-ttu-id="2157b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2157b-106">Property</span></span>|<span data-ttu-id="2157b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2157b-107">Type</span></span>|<span data-ttu-id="2157b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2157b-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2157b-109">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="2157b-109">vpnConfigurationId</span></span>|<span data-ttu-id="2157b-110">String</span><span class="sxs-lookup"><span data-stu-id="2157b-110">String</span></span>|<span data-ttu-id="2157b-111">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="2157b-111">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2157b-112">Связи</span><span class="sxs-lookup"><span data-stu-id="2157b-112">Relationships</span></span>
<span data-ttu-id="2157b-113">Нет</span><span class="sxs-lookup"><span data-stu-id="2157b-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2157b-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2157b-114">JSON Representation</span></span>
<span data-ttu-id="2157b-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2157b-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```



