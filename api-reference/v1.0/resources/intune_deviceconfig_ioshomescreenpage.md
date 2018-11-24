# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="e8b57-101">Тип ресурса iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="e8b57-101">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="e8b57-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e8b57-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8b57-103">Страница, содержащая приложения и папки с начального экрана</span><span class="sxs-lookup"><span data-stu-id="e8b57-103">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="e8b57-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="e8b57-104">Properties</span></span>
|<span data-ttu-id="e8b57-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8b57-105">Property</span></span>|<span data-ttu-id="e8b57-106">Тип</span><span class="sxs-lookup"><span data-stu-id="e8b57-106">Type</span></span>|<span data-ttu-id="e8b57-107">Описание</span><span class="sxs-lookup"><span data-stu-id="e8b57-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8b57-108">displayName</span><span class="sxs-lookup"><span data-stu-id="e8b57-108">displayName</span></span>|<span data-ttu-id="e8b57-109">String</span><span class="sxs-lookup"><span data-stu-id="e8b57-109">String</span></span>|<span data-ttu-id="e8b57-110">Имя страницы</span><span class="sxs-lookup"><span data-stu-id="e8b57-110">Name of the page</span></span>|
|<span data-ttu-id="e8b57-111">icons</span><span class="sxs-lookup"><span data-stu-id="e8b57-111">icons</span></span>|<span data-ttu-id="e8b57-112">Коллекция [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="e8b57-112">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="e8b57-113">Список приложений и папок, отображающихся на странице.</span><span class="sxs-lookup"><span data-stu-id="e8b57-113">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="e8b57-114">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e8b57-114">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8b57-115">Связи</span><span class="sxs-lookup"><span data-stu-id="e8b57-115">Relationships</span></span>
<span data-ttu-id="e8b57-116">Нет</span><span class="sxs-lookup"><span data-stu-id="e8b57-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e8b57-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e8b57-117">JSON Representation</span></span>
<span data-ttu-id="e8b57-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8b57-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenPage",
  "displayName": "String",
  "icons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenItem",
      "displayName": "String",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "String",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "String",
              "bundleID": "String"
            }
          ]
        }
      ]
    }
  ]
}
```



