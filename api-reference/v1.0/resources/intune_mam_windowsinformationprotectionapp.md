# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="189e5-101">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="189e5-101">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="189e5-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="189e5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="189e5-103">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="189e5-103">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="189e5-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="189e5-104">Properties</span></span>
|<span data-ttu-id="189e5-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="189e5-105">Property</span></span>|<span data-ttu-id="189e5-106">Тип</span><span class="sxs-lookup"><span data-stu-id="189e5-106">Type</span></span>|<span data-ttu-id="189e5-107">Описание</span><span class="sxs-lookup"><span data-stu-id="189e5-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="189e5-108">displayName</span><span class="sxs-lookup"><span data-stu-id="189e5-108">displayName</span></span>|<span data-ttu-id="189e5-109">String</span><span class="sxs-lookup"><span data-stu-id="189e5-109">String</span></span>|<span data-ttu-id="189e5-110">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="189e5-110">App display name.</span></span>|
|<span data-ttu-id="189e5-111">description</span><span class="sxs-lookup"><span data-stu-id="189e5-111">description</span></span>|<span data-ttu-id="189e5-112">String</span><span class="sxs-lookup"><span data-stu-id="189e5-112">String</span></span>|<span data-ttu-id="189e5-113">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="189e5-113">The app's description.</span></span>|
|<span data-ttu-id="189e5-114">publisherName</span><span class="sxs-lookup"><span data-stu-id="189e5-114">publisherName</span></span>|<span data-ttu-id="189e5-115">String</span><span class="sxs-lookup"><span data-stu-id="189e5-115">String</span></span>|<span data-ttu-id="189e5-116">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="189e5-116">The publisher name</span></span>|
|<span data-ttu-id="189e5-117">productName</span><span class="sxs-lookup"><span data-stu-id="189e5-117">productName</span></span>|<span data-ttu-id="189e5-118">String</span><span class="sxs-lookup"><span data-stu-id="189e5-118">String</span></span>|<span data-ttu-id="189e5-119">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="189e5-119">The product name.</span></span>|
|<span data-ttu-id="189e5-120">denied</span><span class="sxs-lookup"><span data-stu-id="189e5-120">denied</span></span>|<span data-ttu-id="189e5-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="189e5-121">Boolean</span></span>|<span data-ttu-id="189e5-122">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="189e5-122">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="189e5-123">Связи</span><span class="sxs-lookup"><span data-stu-id="189e5-123">Relationships</span></span>
<span data-ttu-id="189e5-124">Нет</span><span class="sxs-lookup"><span data-stu-id="189e5-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="189e5-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="189e5-125">JSON Representation</span></span>
<span data-ttu-id="189e5-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="189e5-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```



