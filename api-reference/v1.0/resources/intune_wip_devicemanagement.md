# <a name="devicemanagement-resource-type"></a><span data-ttu-id="cb150-101">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="cb150-101">deviceManagement resource type</span></span>

> <span data-ttu-id="cb150-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cb150-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb150-103">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="cb150-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="cb150-104">Методы</span><span class="sxs-lookup"><span data-stu-id="cb150-104">Methods</span></span>
|<span data-ttu-id="cb150-105">Метод</span><span class="sxs-lookup"><span data-stu-id="cb150-105">Method</span></span>|<span data-ttu-id="cb150-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cb150-106">Return Type</span></span>|<span data-ttu-id="cb150-107">Описание</span><span class="sxs-lookup"><span data-stu-id="cb150-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cb150-108">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="cb150-108">Get deviceManagement</span></span>](../api/intune_wip_devicemanagement_get.md)|[<span data-ttu-id="cb150-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="cb150-109">deviceManagement</span></span>](../resources/intune_wip_devicemanagement.md)|<span data-ttu-id="cb150-110">Чтение свойств и связей объекта [deviceManagement](../resources/intune_wip_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="cb150-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_wip_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="cb150-111">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="cb150-111">Update deviceManagement</span></span>](../api/intune_wip_devicemanagement_update.md)|[<span data-ttu-id="cb150-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="cb150-112">deviceManagement</span></span>](../resources/intune_wip_devicemanagement.md)|<span data-ttu-id="cb150-113">Обновление свойств объекта [deviceManagement](../resources/intune_wip_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="cb150-113">Update the properties of a [calendar](../resources/intune_wip_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cb150-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb150-114">Properties</span></span>
|<span data-ttu-id="cb150-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb150-115">Property</span></span>|<span data-ttu-id="cb150-116">Тип</span><span class="sxs-lookup"><span data-stu-id="cb150-116">Type</span></span>|<span data-ttu-id="cb150-117">Описание</span><span class="sxs-lookup"><span data-stu-id="cb150-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb150-118">id</span><span class="sxs-lookup"><span data-stu-id="cb150-118">id</span></span>|<span data-ttu-id="cb150-119">String</span><span class="sxs-lookup"><span data-stu-id="cb150-119">String</span></span>|<span data-ttu-id="cb150-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cb150-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb150-121">Связи</span><span class="sxs-lookup"><span data-stu-id="cb150-121">Relationships</span></span>
|<span data-ttu-id="cb150-122">Связь</span><span class="sxs-lookup"><span data-stu-id="cb150-122">Relationship</span></span>|<span data-ttu-id="cb150-123">Тип</span><span class="sxs-lookup"><span data-stu-id="cb150-123">Type</span></span>|<span data-ttu-id="cb150-124">Описание</span><span class="sxs-lookup"><span data-stu-id="cb150-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb150-125">windowsInformationProtectionAppLearningSummaries</span><span class="sxs-lookup"><span data-stu-id="cb150-125">windowsInformationProtectionAppLearningSummaries</span></span>|<span data-ttu-id="cb150-126">Коллекция [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)</span><span class="sxs-lookup"><span data-stu-id="cb150-126">[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) collection</span></span>|<span data-ttu-id="cb150-127">Сводки по обучению Windows Information Protection для приложений.</span><span class="sxs-lookup"><span data-stu-id="cb150-127">The windows information protection app learning summaries.</span></span>|
|<span data-ttu-id="cb150-128">windowsInformationProtectionNetworkLearningSummaries</span><span class="sxs-lookup"><span data-stu-id="cb150-128">windowsInformationProtectionNetworkLearningSummaries</span></span>|<span data-ttu-id="cb150-129">Коллекция [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)</span><span class="sxs-lookup"><span data-stu-id="cb150-129">[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) collection</span></span>|<span data-ttu-id="cb150-130">Сводки по обучению Windows Information Protection для сетей.</span><span class="sxs-lookup"><span data-stu-id="cb150-130">The windows information protection network learning summaries.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb150-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb150-131">JSON Representation</span></span>
<span data-ttu-id="cb150-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb150-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



