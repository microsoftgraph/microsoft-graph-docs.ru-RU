# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="404f6-101">Тип ресурса iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="404f6-101">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="404f6-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="404f6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="404f6-103">Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.</span><span class="sxs-lookup"><span data-stu-id="404f6-103">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="404f6-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="404f6-104">Properties</span></span>
|<span data-ttu-id="404f6-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="404f6-105">Property</span></span>|<span data-ttu-id="404f6-106">Тип</span><span class="sxs-lookup"><span data-stu-id="404f6-106">Type</span></span>|<span data-ttu-id="404f6-107">Описание</span><span class="sxs-lookup"><span data-stu-id="404f6-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="404f6-108">managedApps</span><span class="sxs-lookup"><span data-stu-id="404f6-108">managedApps</span></span>|<span data-ttu-id="404f6-109">Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="404f6-109">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="404f6-110">Сведения об управляемых приложениях, к которым применяется это правило.</span><span class="sxs-lookup"><span data-stu-id="404f6-110">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="404f6-111">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="404f6-111">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="404f6-112">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="404f6-112">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="404f6-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="404f6-113">Boolean</span></span>|<span data-ttu-id="404f6-114">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в роуминге.</span><span class="sxs-lookup"><span data-stu-id="404f6-114">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="404f6-115">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="404f6-115">cellularDataBlocked</span></span>|<span data-ttu-id="404f6-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="404f6-116">Boolean</span></span>|<span data-ttu-id="404f6-117">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в любое время.</span><span class="sxs-lookup"><span data-stu-id="404f6-117">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="404f6-118">Связи</span><span class="sxs-lookup"><span data-stu-id="404f6-118">Relationships</span></span>
<span data-ttu-id="404f6-119">Нет</span><span class="sxs-lookup"><span data-stu-id="404f6-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="404f6-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="404f6-120">JSON Representation</span></span>
<span data-ttu-id="404f6-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="404f6-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosNetworkUsageRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNetworkUsageRule",
  "managedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "cellularDataBlockWhenRoaming": true,
  "cellularDataBlocked": true
}
```



