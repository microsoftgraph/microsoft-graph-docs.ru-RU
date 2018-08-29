# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="514af-101">Тип ресурса iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="514af-101">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="514af-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="514af-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="514af-103">Папка, содержащая приложения с начального экрана</span><span class="sxs-lookup"><span data-stu-id="514af-103">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="514af-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="514af-104">Properties</span></span>
|<span data-ttu-id="514af-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="514af-105">Property</span></span>|<span data-ttu-id="514af-106">Тип</span><span class="sxs-lookup"><span data-stu-id="514af-106">Type</span></span>|<span data-ttu-id="514af-107">Описание</span><span class="sxs-lookup"><span data-stu-id="514af-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="514af-108">displayName</span><span class="sxs-lookup"><span data-stu-id="514af-108">displayName</span></span>|<span data-ttu-id="514af-109">String</span><span class="sxs-lookup"><span data-stu-id="514af-109">String</span></span>|<span data-ttu-id="514af-110">Имя страницы папки</span><span class="sxs-lookup"><span data-stu-id="514af-110">Name of the folder page</span></span>|
|<span data-ttu-id="514af-111">apps</span><span class="sxs-lookup"><span data-stu-id="514af-111">apps</span></span>|<span data-ttu-id="514af-112">Коллекция [iosHomeScreenApp](../resources/intune_deviceconfig_ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="514af-112">[iosHomeScreenApp](../resources/intune_deviceconfig_ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="514af-113">Список приложений, которые отображаются на странице в папке.</span><span class="sxs-lookup"><span data-stu-id="514af-113">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="514af-114">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="514af-114">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="514af-115">Связи</span><span class="sxs-lookup"><span data-stu-id="514af-115">Relationships</span></span>
<span data-ttu-id="514af-116">Нет</span><span class="sxs-lookup"><span data-stu-id="514af-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="514af-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="514af-117">JSON Representation</span></span>
<span data-ttu-id="514af-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="514af-118">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String"
    }
  ]
}
```



