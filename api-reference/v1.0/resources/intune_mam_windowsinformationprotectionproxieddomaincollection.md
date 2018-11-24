# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="4cae8-101">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="4cae8-101">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="4cae8-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4cae8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4cae8-103">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="4cae8-103">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="4cae8-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="4cae8-104">Properties</span></span>
|<span data-ttu-id="4cae8-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="4cae8-105">Property</span></span>|<span data-ttu-id="4cae8-106">Тип</span><span class="sxs-lookup"><span data-stu-id="4cae8-106">Type</span></span>|<span data-ttu-id="4cae8-107">Описание</span><span class="sxs-lookup"><span data-stu-id="4cae8-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cae8-108">displayName</span><span class="sxs-lookup"><span data-stu-id="4cae8-108">displayName</span></span>|<span data-ttu-id="4cae8-109">Строка</span><span class="sxs-lookup"><span data-stu-id="4cae8-109">String</span></span>|<span data-ttu-id="4cae8-110">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="4cae8-110">Display name</span></span>|
|<span data-ttu-id="4cae8-111">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="4cae8-111">proxiedDomains</span></span>|<span data-ttu-id="4cae8-112">Коллекция объектов [proxiedDomain](../resources/intune_mam_proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="4cae8-112">[proxiedDomain](../resources/intune_mam_proxieddomain.md) collection</span></span>|<span data-ttu-id="4cae8-113">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="4cae8-113">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cae8-114">Связи</span><span class="sxs-lookup"><span data-stu-id="4cae8-114">Relationships</span></span>
<span data-ttu-id="4cae8-115">Нет</span><span class="sxs-lookup"><span data-stu-id="4cae8-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4cae8-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4cae8-116">JSON Representation</span></span>
<span data-ttu-id="4cae8-117">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4cae8-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
  "displayName": "String",
  "proxiedDomains": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ]
}
```



