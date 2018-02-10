# <a name="ipv6range-resource-type"></a><span data-ttu-id="71d46-101">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="71d46-101">iPv6Range resource type</span></span>

> <span data-ttu-id="71d46-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="71d46-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71d46-103">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="71d46-103">IP V6 range</span></span>

<span data-ttu-id="71d46-104">Наследуется от ресурса [ipRange](../resources/intune_mam_iprange.md)</span><span class="sxs-lookup"><span data-stu-id="71d46-104">Inherits from [ipRange](../resources/intune_mam_iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="71d46-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="71d46-105">Properties</span></span>
|<span data-ttu-id="71d46-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="71d46-106">Property</span></span>|<span data-ttu-id="71d46-107">Тип</span><span class="sxs-lookup"><span data-stu-id="71d46-107">Type</span></span>|<span data-ttu-id="71d46-108">Описание</span><span class="sxs-lookup"><span data-stu-id="71d46-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71d46-109">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="71d46-109">lowerAddress</span></span>|<span data-ttu-id="71d46-110">Строка</span><span class="sxs-lookup"><span data-stu-id="71d46-110">String</span></span>|<span data-ttu-id="71d46-111">Нижней IP-адрес</span><span class="sxs-lookup"><span data-stu-id="71d46-111">Lower IP Address</span></span>|
|<span data-ttu-id="71d46-112">upperAddress</span><span class="sxs-lookup"><span data-stu-id="71d46-112">upperAddress</span></span>|<span data-ttu-id="71d46-113">Строка</span><span class="sxs-lookup"><span data-stu-id="71d46-113">String</span></span>|<span data-ttu-id="71d46-114">Верхний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="71d46-114">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="71d46-115">Связи</span><span class="sxs-lookup"><span data-stu-id="71d46-115">Relationships</span></span>
<span data-ttu-id="71d46-116">Нет</span><span class="sxs-lookup"><span data-stu-id="71d46-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="71d46-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71d46-117">JSON Representation</span></span>
<span data-ttu-id="71d46-118">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71d46-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



