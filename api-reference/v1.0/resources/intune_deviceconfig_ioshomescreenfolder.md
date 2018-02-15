# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="df5f8-101">Тип ресурса iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="df5f8-101">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="df5f8-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="df5f8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df5f8-103">Папка, содержащая страницы приложений на начальном экране</span><span class="sxs-lookup"><span data-stu-id="df5f8-103">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="df5f8-104">Наследуется от [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="df5f8-104">Inherits from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="df5f8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="df5f8-105">Properties</span></span>
|<span data-ttu-id="df5f8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="df5f8-106">Property</span></span>|<span data-ttu-id="df5f8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="df5f8-107">Type</span></span>|<span data-ttu-id="df5f8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="df5f8-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df5f8-109">displayName</span><span class="sxs-lookup"><span data-stu-id="df5f8-109">displayName</span></span>|<span data-ttu-id="df5f8-110">String</span><span class="sxs-lookup"><span data-stu-id="df5f8-110">String</span></span>|<span data-ttu-id="df5f8-111">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="df5f8-111">Name of the app Inherited from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="df5f8-112">pages</span><span class="sxs-lookup"><span data-stu-id="df5f8-112">pages</span></span>|<span data-ttu-id="df5f8-113">Коллекция [iosHomeScreenFolderPage](../resources/intune_deviceconfig_ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="df5f8-113">[iosHomeScreenFolderPage](../resources/intune_deviceconfig_ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="df5f8-114">Страницы значков на начальном экране, которые должны относиться к типу приложения.</span><span class="sxs-lookup"><span data-stu-id="df5f8-114">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="df5f8-115">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="df5f8-115">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df5f8-116">Связи</span><span class="sxs-lookup"><span data-stu-id="df5f8-116">Relationships</span></span>
<span data-ttu-id="df5f8-117">Нет</span><span class="sxs-lookup"><span data-stu-id="df5f8-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="df5f8-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="df5f8-118">JSON Representation</span></span>
<span data-ttu-id="df5f8-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df5f8-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
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
```



