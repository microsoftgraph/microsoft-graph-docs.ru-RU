# <a name="proxieddomain-resource-type"></a><span data-ttu-id="e84f6-101">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="e84f6-101">proxiedDomain resource type</span></span>

> <span data-ttu-id="e84f6-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e84f6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e84f6-103">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="e84f6-103">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="e84f6-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="e84f6-104">Properties</span></span>
|<span data-ttu-id="e84f6-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="e84f6-105">Property</span></span>|<span data-ttu-id="e84f6-106">Тип</span><span class="sxs-lookup"><span data-stu-id="e84f6-106">Type</span></span>|<span data-ttu-id="e84f6-107">Описание</span><span class="sxs-lookup"><span data-stu-id="e84f6-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e84f6-108">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="e84f6-108">ipAddressOrFQDN</span></span>|<span data-ttu-id="e84f6-109">Строка</span><span class="sxs-lookup"><span data-stu-id="e84f6-109">String</span></span>|<span data-ttu-id="e84f6-110">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="e84f6-110">The IP address or FQDN</span></span>|
|<span data-ttu-id="e84f6-111">proxy</span><span class="sxs-lookup"><span data-stu-id="e84f6-111">web proxy</span></span>|<span data-ttu-id="e84f6-112">Строка</span><span class="sxs-lookup"><span data-stu-id="e84f6-112">String</span></span>|<span data-ttu-id="e84f6-113">IP-адрес прокси-сервера</span><span class="sxs-lookup"><span data-stu-id="e84f6-113">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="e84f6-114">Связи</span><span class="sxs-lookup"><span data-stu-id="e84f6-114">Relationships</span></span>
<span data-ttu-id="e84f6-115">Нет</span><span class="sxs-lookup"><span data-stu-id="e84f6-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e84f6-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e84f6-116">JSON Representation</span></span>
<span data-ttu-id="e84f6-117">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e84f6-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



