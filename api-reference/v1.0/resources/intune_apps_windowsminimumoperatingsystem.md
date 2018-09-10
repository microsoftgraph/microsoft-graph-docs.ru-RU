# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="0f6dd-101">Тип ресурса windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0f6dd-101">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="0f6dd-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0f6dd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f6dd-103">Минимальная версия операционной системы, необходимая мобильному приложению для Windows.</span><span class="sxs-lookup"><span data-stu-id="0f6dd-103">The minimum operating system required for a Windows mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="0f6dd-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f6dd-104">Properties</span></span>
|<span data-ttu-id="0f6dd-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f6dd-105">Property</span></span>|<span data-ttu-id="0f6dd-106">Тип</span><span class="sxs-lookup"><span data-stu-id="0f6dd-106">Type</span></span>|<span data-ttu-id="0f6dd-107">Описание</span><span class="sxs-lookup"><span data-stu-id="0f6dd-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f6dd-108">v8_0</span><span class="sxs-lookup"><span data-stu-id="0f6dd-108">v8_0</span></span>|<span data-ttu-id="0f6dd-109">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f6dd-109">Boolean</span></span>|<span data-ttu-id="0f6dd-110">Windows 8.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="0f6dd-110">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="0f6dd-111">v8_1</span><span class="sxs-lookup"><span data-stu-id="0f6dd-111">v8_1</span></span>|<span data-ttu-id="0f6dd-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f6dd-112">Boolean</span></span>|<span data-ttu-id="0f6dd-113">Windows 8.1 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="0f6dd-113">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="0f6dd-114">v10_0</span><span class="sxs-lookup"><span data-stu-id="0f6dd-114">v10_0</span></span>|<span data-ttu-id="0f6dd-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f6dd-115">Boolean</span></span>|<span data-ttu-id="0f6dd-116">Windows 10.0 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="0f6dd-116">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f6dd-117">Связи</span><span class="sxs-lookup"><span data-stu-id="0f6dd-117">Relationships</span></span>
<span data-ttu-id="0f6dd-118">Нет</span><span class="sxs-lookup"><span data-stu-id="0f6dd-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0f6dd-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f6dd-119">JSON Representation</span></span>
<span data-ttu-id="0f6dd-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f6dd-120">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true
}
```








