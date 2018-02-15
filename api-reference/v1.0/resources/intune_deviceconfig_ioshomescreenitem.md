# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="e9a26-101">Тип ресурса iosHomeScreenItem</span><span class="sxs-lookup"><span data-stu-id="e9a26-101">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="e9a26-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e9a26-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9a26-103">Представляет элемент на начальном экране iOS</span><span class="sxs-lookup"><span data-stu-id="e9a26-103">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="e9a26-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9a26-104">Properties</span></span>
|<span data-ttu-id="e9a26-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9a26-105">Property</span></span>|<span data-ttu-id="e9a26-106">Тип</span><span class="sxs-lookup"><span data-stu-id="e9a26-106">Type</span></span>|<span data-ttu-id="e9a26-107">Описание</span><span class="sxs-lookup"><span data-stu-id="e9a26-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9a26-108">displayName</span><span class="sxs-lookup"><span data-stu-id="e9a26-108">displayName</span></span>|<span data-ttu-id="e9a26-109">String</span><span class="sxs-lookup"><span data-stu-id="e9a26-109">String</span></span>|<span data-ttu-id="e9a26-110">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="e9a26-110">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9a26-111">Связи</span><span class="sxs-lookup"><span data-stu-id="e9a26-111">Relationships</span></span>
<span data-ttu-id="e9a26-112">Нет</span><span class="sxs-lookup"><span data-stu-id="e9a26-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e9a26-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9a26-113">JSON Representation</span></span>
<span data-ttu-id="e9a26-114">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9a26-114">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```



