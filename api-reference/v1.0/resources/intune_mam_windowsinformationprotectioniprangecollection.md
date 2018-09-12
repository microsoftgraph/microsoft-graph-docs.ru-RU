# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="f7a47-101">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="f7a47-101">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="f7a47-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f7a47-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7a47-103">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="f7a47-103">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="f7a47-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7a47-104">Properties</span></span>
|<span data-ttu-id="f7a47-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7a47-105">Property</span></span>|<span data-ttu-id="f7a47-106">Тип</span><span class="sxs-lookup"><span data-stu-id="f7a47-106">Type</span></span>|<span data-ttu-id="f7a47-107">Описание</span><span class="sxs-lookup"><span data-stu-id="f7a47-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7a47-108">displayName</span><span class="sxs-lookup"><span data-stu-id="f7a47-108">displayName</span></span>|<span data-ttu-id="f7a47-109">Строка</span><span class="sxs-lookup"><span data-stu-id="f7a47-109">String</span></span>|<span data-ttu-id="f7a47-110">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="f7a47-110">Display name</span></span>|
|<span data-ttu-id="f7a47-111">ranges</span><span class="sxs-lookup"><span data-stu-id="f7a47-111">ranges</span></span>|<span data-ttu-id="f7a47-112">Коллекция объектов [ipRange](../resources/intune_mam_iprange.md)</span><span class="sxs-lookup"><span data-stu-id="f7a47-112">[ipRange](../resources/intune_mam_iprange.md) collection</span></span>|<span data-ttu-id="f7a47-113">Коллекция диапазонов IP-адресов</span><span class="sxs-lookup"><span data-stu-id="f7a47-113">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7a47-114">Связи</span><span class="sxs-lookup"><span data-stu-id="f7a47-114">Relationships</span></span>
<span data-ttu-id="f7a47-115">Нет</span><span class="sxs-lookup"><span data-stu-id="f7a47-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f7a47-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f7a47-116">JSON Representation</span></span>
<span data-ttu-id="f7a47-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7a47-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionIPRangeCollection",
  "displayName": "String",
  "ranges": [
    {
      "@odata.type": "microsoft.graph.ipRange",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```








