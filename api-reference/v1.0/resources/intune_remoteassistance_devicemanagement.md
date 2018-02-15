# <a name="devicemanagement-resource-type"></a><span data-ttu-id="90ac5-101">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="90ac5-101">deviceManagement resource type</span></span>

> <span data-ttu-id="90ac5-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="90ac5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="90ac5-103">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="90ac5-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="90ac5-104">Методы</span><span class="sxs-lookup"><span data-stu-id="90ac5-104">Methods</span></span>
|<span data-ttu-id="90ac5-105">Метод</span><span class="sxs-lookup"><span data-stu-id="90ac5-105">Method</span></span>|<span data-ttu-id="90ac5-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="90ac5-106">Return Type</span></span>|<span data-ttu-id="90ac5-107">Описание</span><span class="sxs-lookup"><span data-stu-id="90ac5-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="90ac5-108">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="90ac5-108">Get deviceManagement</span></span>](../api/intune_remoteassistance_devicemanagement_get.md)|[<span data-ttu-id="90ac5-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="90ac5-109">deviceManagement</span></span>](../resources/intune_remoteassistance_devicemanagement.md)|<span data-ttu-id="90ac5-110">Чтение свойств и связей объекта [deviceManagement](../resources/intune_remoteassistance_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="90ac5-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_remoteassistance_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="90ac5-111">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="90ac5-111">Update deviceManagement</span></span>](../api/intune_remoteassistance_devicemanagement_update.md)|[<span data-ttu-id="90ac5-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="90ac5-112">deviceManagement</span></span>](../resources/intune_remoteassistance_devicemanagement.md)|<span data-ttu-id="90ac5-113">Обновление свойств объекта [deviceManagement](../resources/intune_remoteassistance_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="90ac5-113">Update the properties of a [calendar](../resources/intune_remoteassistance_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="90ac5-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="90ac5-114">Properties</span></span>
|<span data-ttu-id="90ac5-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="90ac5-115">Property</span></span>|<span data-ttu-id="90ac5-116">Тип</span><span class="sxs-lookup"><span data-stu-id="90ac5-116">Type</span></span>|<span data-ttu-id="90ac5-117">Описание</span><span class="sxs-lookup"><span data-stu-id="90ac5-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90ac5-118">id</span><span class="sxs-lookup"><span data-stu-id="90ac5-118">id</span></span>|<span data-ttu-id="90ac5-119">String</span><span class="sxs-lookup"><span data-stu-id="90ac5-119">String</span></span>|<span data-ttu-id="90ac5-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="90ac5-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="90ac5-121">Связи</span><span class="sxs-lookup"><span data-stu-id="90ac5-121">Relationships</span></span>
|<span data-ttu-id="90ac5-122">Связь</span><span class="sxs-lookup"><span data-stu-id="90ac5-122">Relationship</span></span>|<span data-ttu-id="90ac5-123">Тип</span><span class="sxs-lookup"><span data-stu-id="90ac5-123">Type</span></span>|<span data-ttu-id="90ac5-124">Описание</span><span class="sxs-lookup"><span data-stu-id="90ac5-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90ac5-125">remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="90ac5-125">remoteAssistancePartners</span></span>|<span data-ttu-id="90ac5-126">Коллекция [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)</span><span class="sxs-lookup"><span data-stu-id="90ac5-126">[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="90ac5-127">Партнеры по удаленной помощи.</span><span class="sxs-lookup"><span data-stu-id="90ac5-127">The remote assist partners.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90ac5-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="90ac5-128">JSON Representation</span></span>
<span data-ttu-id="90ac5-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90ac5-129">Here is a JSON representation of the resource.</span></span>
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



