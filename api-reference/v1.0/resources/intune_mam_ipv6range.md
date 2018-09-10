# <a name="ipv6range-resource-type"></a><span data-ttu-id="2fae6-101">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="2fae6-101">iPv6Range resource type</span></span>

> <span data-ttu-id="2fae6-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2fae6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2fae6-103">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="2fae6-103">IP V6 range</span></span>

<span data-ttu-id="2fae6-104">Наследуется от ресурса [ipRange](../resources/intune_mam_iprange.md)</span><span class="sxs-lookup"><span data-stu-id="2fae6-104">Inherits from [ipRange](../resources/intune_mam_iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2fae6-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2fae6-105">Properties</span></span>
|<span data-ttu-id="2fae6-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2fae6-106">Property</span></span>|<span data-ttu-id="2fae6-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2fae6-107">Type</span></span>|<span data-ttu-id="2fae6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2fae6-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fae6-109">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="2fae6-109">lowerAddress</span></span>|<span data-ttu-id="2fae6-110">String</span><span class="sxs-lookup"><span data-stu-id="2fae6-110">String</span></span>|<span data-ttu-id="2fae6-111">Нижний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="2fae6-111">Lower IP Address</span></span>|
|<span data-ttu-id="2fae6-112">upperAddress</span><span class="sxs-lookup"><span data-stu-id="2fae6-112">upperAddress</span></span>|<span data-ttu-id="2fae6-113">String</span><span class="sxs-lookup"><span data-stu-id="2fae6-113">String</span></span>|<span data-ttu-id="2fae6-114">Верхний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="2fae6-114">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fae6-115">Связи</span><span class="sxs-lookup"><span data-stu-id="2fae6-115">Relationships</span></span>
<span data-ttu-id="2fae6-116">Нет</span><span class="sxs-lookup"><span data-stu-id="2fae6-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2fae6-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2fae6-117">JSON Representation</span></span>
<span data-ttu-id="2fae6-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2fae6-118">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv6Range"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```








