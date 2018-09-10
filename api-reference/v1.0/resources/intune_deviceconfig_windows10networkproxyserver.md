# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="e80e1-101">Тип ресурса windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="e80e1-101">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="e80e1-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e80e1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e80e1-103">Политика прокси-сервера сети.</span><span class="sxs-lookup"><span data-stu-id="e80e1-103">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="e80e1-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="e80e1-104">Properties</span></span>
|<span data-ttu-id="e80e1-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="e80e1-105">Property</span></span>|<span data-ttu-id="e80e1-106">Тип</span><span class="sxs-lookup"><span data-stu-id="e80e1-106">Type</span></span>|<span data-ttu-id="e80e1-107">Описание</span><span class="sxs-lookup"><span data-stu-id="e80e1-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e80e1-108">address</span><span class="sxs-lookup"><span data-stu-id="e80e1-108">address</span></span>|<span data-ttu-id="e80e1-109">String</span><span class="sxs-lookup"><span data-stu-id="e80e1-109">String</span></span>|<span data-ttu-id="e80e1-110">Адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="e80e1-110">Address to the proxy server.</span></span> <span data-ttu-id="e80e1-111">Укажите адрес в формате <server>\[":"<port>\]</span><span class="sxs-lookup"><span data-stu-id="e80e1-111">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="e80e1-112">exceptions</span><span class="sxs-lookup"><span data-stu-id="e80e1-112">exceptions</span></span>|<span data-ttu-id="e80e1-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e80e1-113">String collection</span></span>|<span data-ttu-id="e80e1-114">Адреса, которые не должны использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="e80e1-114">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="e80e1-115">Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.</span><span class="sxs-lookup"><span data-stu-id="e80e1-115">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="e80e1-116">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="e80e1-116">useForLocalAddresses</span></span>|<span data-ttu-id="e80e1-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="e80e1-117">Boolean</span></span>|<span data-ttu-id="e80e1-118">Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).</span><span class="sxs-lookup"><span data-stu-id="e80e1-118">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e80e1-119">Связи</span><span class="sxs-lookup"><span data-stu-id="e80e1-119">Relationships</span></span>
<span data-ttu-id="e80e1-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e80e1-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e80e1-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e80e1-121">JSON Representation</span></span>
<span data-ttu-id="e80e1-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e80e1-122">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10NetworkProxyServer"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10NetworkProxyServer",
  "address": "String",
  "exceptions": [
    "String"
  ],
  "useForLocalAddresses": true
}
```








