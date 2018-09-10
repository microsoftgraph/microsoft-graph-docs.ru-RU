# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="d4853-101">Тип ресурса iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="d4853-101">iosDeviceType resource type</span></span>

> <span data-ttu-id="d4853-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d4853-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4853-103">Содержит свойства возможных типов устройств iOS, на которых может работать мобильное приложение.</span><span class="sxs-lookup"><span data-stu-id="d4853-103">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="d4853-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4853-104">Properties</span></span>
|<span data-ttu-id="d4853-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4853-105">Property</span></span>|<span data-ttu-id="d4853-106">Тип</span><span class="sxs-lookup"><span data-stu-id="d4853-106">Type</span></span>|<span data-ttu-id="d4853-107">Описание</span><span class="sxs-lookup"><span data-stu-id="d4853-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4853-108">iPad</span><span class="sxs-lookup"><span data-stu-id="d4853-108">iPad</span></span>|<span data-ttu-id="d4853-109">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4853-109">Boolean</span></span>|<span data-ttu-id="d4853-110">Указывает, должно ли приложение работать на iPad.</span><span class="sxs-lookup"><span data-stu-id="d4853-110">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="d4853-111">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="d4853-111">iPhoneAndIPod</span></span>|<span data-ttu-id="d4853-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4853-112">Boolean</span></span>|<span data-ttu-id="d4853-113">Указывает, должно ли приложение работать на iPhone и iPod.</span><span class="sxs-lookup"><span data-stu-id="d4853-113">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4853-114">Связи</span><span class="sxs-lookup"><span data-stu-id="d4853-114">Relationships</span></span>
<span data-ttu-id="d4853-115">Нет</span><span class="sxs-lookup"><span data-stu-id="d4853-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d4853-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4853-116">JSON Representation</span></span>
<span data-ttu-id="d4853-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4853-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosDeviceType"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceType",
  "iPad": true,
  "iPhoneAndIPod": true
}
```








