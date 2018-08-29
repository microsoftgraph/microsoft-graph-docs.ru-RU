# <a name="ipv4range-resource-type"></a><span data-ttu-id="a6c61-101">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="a6c61-101">iPv4Range resource type</span></span>

> <span data-ttu-id="a6c61-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a6c61-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6c61-103">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="a6c61-103">IP V4 range</span></span>

<span data-ttu-id="a6c61-104">Наследуется от [ipRange](../resources/intune_mam_iprange.md)</span><span class="sxs-lookup"><span data-stu-id="a6c61-104">Inherits from [ipRange](../resources/intune_mam_iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a6c61-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6c61-105">Properties</span></span>
|<span data-ttu-id="a6c61-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6c61-106">Property</span></span>|<span data-ttu-id="a6c61-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a6c61-107">Type</span></span>|<span data-ttu-id="a6c61-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a6c61-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6c61-109">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="a6c61-109">lowerAddress</span></span>|<span data-ttu-id="a6c61-110">String</span><span class="sxs-lookup"><span data-stu-id="a6c61-110">String</span></span>|<span data-ttu-id="a6c61-111">Нижний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="a6c61-111">Lower IP Address</span></span>|
|<span data-ttu-id="a6c61-112">upperAddress</span><span class="sxs-lookup"><span data-stu-id="a6c61-112">upperAddress</span></span>|<span data-ttu-id="a6c61-113">String</span><span class="sxs-lookup"><span data-stu-id="a6c61-113">String</span></span>|<span data-ttu-id="a6c61-114">Верхний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="a6c61-114">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6c61-115">Связи</span><span class="sxs-lookup"><span data-stu-id="a6c61-115">Relationships</span></span>
<span data-ttu-id="a6c61-116">Нет</span><span class="sxs-lookup"><span data-stu-id="a6c61-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a6c61-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6c61-117">JSON Representation</span></span>
<span data-ttu-id="a6c61-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6c61-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.ipRange",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



