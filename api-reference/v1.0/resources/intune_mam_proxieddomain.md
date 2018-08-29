# <a name="proxieddomain-resource-type"></a><span data-ttu-id="290d5-101">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="290d5-101">proxiedDomain resource type</span></span>

> <span data-ttu-id="290d5-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="290d5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="290d5-103">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="290d5-103">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="290d5-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="290d5-104">Properties</span></span>
|<span data-ttu-id="290d5-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="290d5-105">Property</span></span>|<span data-ttu-id="290d5-106">Тип</span><span class="sxs-lookup"><span data-stu-id="290d5-106">Type</span></span>|<span data-ttu-id="290d5-107">Описание</span><span class="sxs-lookup"><span data-stu-id="290d5-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="290d5-108">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="290d5-108">ipAddressOrFQDN</span></span>|<span data-ttu-id="290d5-109">Строка</span><span class="sxs-lookup"><span data-stu-id="290d5-109">String</span></span>|<span data-ttu-id="290d5-110">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="290d5-110">The IP address or FQDN</span></span>|
|<span data-ttu-id="290d5-111">proxy</span><span class="sxs-lookup"><span data-stu-id="290d5-111">proxy</span></span>|<span data-ttu-id="290d5-112">Строка</span><span class="sxs-lookup"><span data-stu-id="290d5-112">String</span></span>|<span data-ttu-id="290d5-113">IP-адрес прокси-сервера</span><span class="sxs-lookup"><span data-stu-id="290d5-113">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="290d5-114">Связи</span><span class="sxs-lookup"><span data-stu-id="290d5-114">Relationships</span></span>
<span data-ttu-id="290d5-115">Нет</span><span class="sxs-lookup"><span data-stu-id="290d5-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="290d5-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="290d5-116">JSON Representation</span></span>
<span data-ttu-id="290d5-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="290d5-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```



