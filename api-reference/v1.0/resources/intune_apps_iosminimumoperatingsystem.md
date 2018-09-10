# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="68937-101">Тип ресурса iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="68937-101">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="68937-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="68937-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68937-103">Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.</span><span class="sxs-lookup"><span data-stu-id="68937-103">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="68937-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="68937-104">Properties</span></span>
|<span data-ttu-id="68937-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="68937-105">Property</span></span>|<span data-ttu-id="68937-106">Тип</span><span class="sxs-lookup"><span data-stu-id="68937-106">Type</span></span>|<span data-ttu-id="68937-107">Описание</span><span class="sxs-lookup"><span data-stu-id="68937-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68937-108">v8_0</span><span class="sxs-lookup"><span data-stu-id="68937-108">v8_0</span></span>|<span data-ttu-id="68937-109">Boolean</span><span class="sxs-lookup"><span data-stu-id="68937-109">Boolean</span></span>|<span data-ttu-id="68937-110">Версия 8.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="68937-110">Version 8.0 or later.</span></span>|
|<span data-ttu-id="68937-111">v9_0</span><span class="sxs-lookup"><span data-stu-id="68937-111">v9_0</span></span>|<span data-ttu-id="68937-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="68937-112">Boolean</span></span>|<span data-ttu-id="68937-113">Версия 9.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="68937-113">Version 9.0 or later.</span></span>|
|<span data-ttu-id="68937-114">v10_0</span><span class="sxs-lookup"><span data-stu-id="68937-114">v10_0</span></span>|<span data-ttu-id="68937-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="68937-115">Boolean</span></span>|<span data-ttu-id="68937-116">Версия 10.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="68937-116">Version 10.0 or later.</span></span>|
|<span data-ttu-id="68937-117">v11_0</span><span class="sxs-lookup"><span data-stu-id="68937-117">v11_0</span></span>|<span data-ttu-id="68937-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="68937-118">Boolean</span></span>|<span data-ttu-id="68937-119">Версия 11.0 или выше.</span><span class="sxs-lookup"><span data-stu-id="68937-119">Version 11.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68937-120">Связи</span><span class="sxs-lookup"><span data-stu-id="68937-120">Relationships</span></span>
<span data-ttu-id="68937-121">Нет</span><span class="sxs-lookup"><span data-stu-id="68937-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="68937-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="68937-122">JSON Representation</span></span>
<span data-ttu-id="68937-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68937-123">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true
}
```








