# <a name="rgbcolor-resource-type"></a><span data-ttu-id="f8a10-101">Тип ресурса rgbColor</span><span class="sxs-lookup"><span data-stu-id="f8a10-101">rgbColor resource type</span></span>

> <span data-ttu-id="f8a10-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f8a10-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8a10-103">Цвет в формате RGB.</span><span class="sxs-lookup"><span data-stu-id="f8a10-103">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="f8a10-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="f8a10-104">Properties</span></span>
|<span data-ttu-id="f8a10-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8a10-105">Property</span></span>|<span data-ttu-id="f8a10-106">Тип</span><span class="sxs-lookup"><span data-stu-id="f8a10-106">Type</span></span>|<span data-ttu-id="f8a10-107">Описание</span><span class="sxs-lookup"><span data-stu-id="f8a10-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8a10-108">r</span><span class="sxs-lookup"><span data-stu-id="f8a10-108">r</span></span>|<span data-ttu-id="f8a10-109">Байт</span><span class="sxs-lookup"><span data-stu-id="f8a10-109">Byte</span></span>|<span data-ttu-id="f8a10-110">Значение красного</span><span class="sxs-lookup"><span data-stu-id="f8a10-110">Red Value</span></span>|
|<span data-ttu-id="f8a10-111">g</span><span class="sxs-lookup"><span data-stu-id="f8a10-111">g</span></span>|<span data-ttu-id="f8a10-112">Байт</span><span class="sxs-lookup"><span data-stu-id="f8a10-112">Byte</span></span>|<span data-ttu-id="f8a10-113">Значение зеленого</span><span class="sxs-lookup"><span data-stu-id="f8a10-113">Green Value</span></span>|
|<span data-ttu-id="f8a10-114">b</span><span class="sxs-lookup"><span data-stu-id="f8a10-114">b</span></span>|<span data-ttu-id="f8a10-115">Байт</span><span class="sxs-lookup"><span data-stu-id="f8a10-115">Byte</span></span>|<span data-ttu-id="f8a10-116">Значение синего</span><span class="sxs-lookup"><span data-stu-id="f8a10-116">Blue Value</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8a10-117">Связи</span><span class="sxs-lookup"><span data-stu-id="f8a10-117">Relationships</span></span>
<span data-ttu-id="f8a10-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f8a10-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f8a10-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f8a10-119">JSON Representation</span></span>
<span data-ttu-id="f8a10-120">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8a10-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.rgbColor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rgbColor",
  "r": 1024,
  "g": 1024,
  "b": 1024
}
```



