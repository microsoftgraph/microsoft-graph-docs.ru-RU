# <a name="proxieddomain-resource-type"></a><span data-ttu-id="ff7a4-101">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="ff7a4-101">proxiedDomain resource type</span></span>

> <span data-ttu-id="ff7a4-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ff7a4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff7a4-103">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="ff7a4-103">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="ff7a4-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff7a4-104">Properties</span></span>
|<span data-ttu-id="ff7a4-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff7a4-105">Property</span></span>|<span data-ttu-id="ff7a4-106">Тип</span><span class="sxs-lookup"><span data-stu-id="ff7a4-106">Type</span></span>|<span data-ttu-id="ff7a4-107">Описание</span><span class="sxs-lookup"><span data-stu-id="ff7a4-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff7a4-108">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="ff7a4-108">ipAddressOrFQDN</span></span>|<span data-ttu-id="ff7a4-109">Строка</span><span class="sxs-lookup"><span data-stu-id="ff7a4-109">String</span></span>|<span data-ttu-id="ff7a4-110">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="ff7a4-110">The IP address or FQDN</span></span>|
|<span data-ttu-id="ff7a4-111">proxy</span><span class="sxs-lookup"><span data-stu-id="ff7a4-111">proxy</span></span>|<span data-ttu-id="ff7a4-112">Строка</span><span class="sxs-lookup"><span data-stu-id="ff7a4-112">String</span></span>|<span data-ttu-id="ff7a4-113">IP-адрес прокси-сервера</span><span class="sxs-lookup"><span data-stu-id="ff7a4-113">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff7a4-114">Связи</span><span class="sxs-lookup"><span data-stu-id="ff7a4-114">Relationships</span></span>
<span data-ttu-id="ff7a4-115">Нет</span><span class="sxs-lookup"><span data-stu-id="ff7a4-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ff7a4-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff7a4-116">JSON Representation</span></span>
<span data-ttu-id="ff7a4-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff7a4-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.proxiedDomain"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```








