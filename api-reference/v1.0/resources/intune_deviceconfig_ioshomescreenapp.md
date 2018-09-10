# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="585d9-101">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="585d9-101">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="585d9-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="585d9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="585d9-103">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="585d9-103">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="585d9-104">Наследуется от [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="585d9-104">Inherits from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="585d9-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="585d9-105">Properties</span></span>
|<span data-ttu-id="585d9-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="585d9-106">Property</span></span>|<span data-ttu-id="585d9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="585d9-107">Type</span></span>|<span data-ttu-id="585d9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="585d9-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="585d9-109">displayName</span><span class="sxs-lookup"><span data-stu-id="585d9-109">displayName</span></span>|<span data-ttu-id="585d9-110">String</span><span class="sxs-lookup"><span data-stu-id="585d9-110">String</span></span>|<span data-ttu-id="585d9-111">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="585d9-111">Name of the app Inherited from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="585d9-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="585d9-112">bundleID</span></span>|<span data-ttu-id="585d9-113">String</span><span class="sxs-lookup"><span data-stu-id="585d9-113">String</span></span>|<span data-ttu-id="585d9-114">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="585d9-114">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="585d9-115">Связи</span><span class="sxs-lookup"><span data-stu-id="585d9-115">Relationships</span></span>
<span data-ttu-id="585d9-116">Нет</span><span class="sxs-lookup"><span data-stu-id="585d9-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="585d9-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="585d9-117">JSON Representation</span></span>
<span data-ttu-id="585d9-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="585d9-118">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```








