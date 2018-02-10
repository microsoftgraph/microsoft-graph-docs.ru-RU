# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="e52c5-101">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="e52c5-101">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="e52c5-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e52c5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e52c5-103">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="e52c5-103">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="e52c5-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="e52c5-104">Properties</span></span>
|<span data-ttu-id="e52c5-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="e52c5-105">Property</span></span>|<span data-ttu-id="e52c5-106">Тип</span><span class="sxs-lookup"><span data-stu-id="e52c5-106">Type</span></span>|<span data-ttu-id="e52c5-107">Описание</span><span class="sxs-lookup"><span data-stu-id="e52c5-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e52c5-108">displayName</span><span class="sxs-lookup"><span data-stu-id="e52c5-108">displayName</span></span>|<span data-ttu-id="e52c5-109">Строка</span><span class="sxs-lookup"><span data-stu-id="e52c5-109">String</span></span>|<span data-ttu-id="e52c5-110">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="e52c5-110">Display name</span></span>|
|<span data-ttu-id="e52c5-111">ranges</span><span class="sxs-lookup"><span data-stu-id="e52c5-111">ranges</span></span>|<span data-ttu-id="e52c5-112">Коллекция объектов [ipRange](../resources/intune_mam_iprange.md)</span><span class="sxs-lookup"><span data-stu-id="e52c5-112">[ipRange](../resources/intune_mam_iprange.md) collection</span></span>|<span data-ttu-id="e52c5-113">Коллекция диапазонов IP-адресов</span><span class="sxs-lookup"><span data-stu-id="e52c5-113">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="e52c5-114">Связи</span><span class="sxs-lookup"><span data-stu-id="e52c5-114">Relationships</span></span>
<span data-ttu-id="e52c5-115">Нет</span><span class="sxs-lookup"><span data-stu-id="e52c5-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e52c5-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e52c5-116">JSON Representation</span></span>
<span data-ttu-id="e52c5-117">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e52c5-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionIPRangeCollection",
  "displayName": "String",
  "ranges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```



