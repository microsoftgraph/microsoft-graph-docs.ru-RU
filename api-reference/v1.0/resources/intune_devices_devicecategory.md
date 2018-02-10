# <a name="devicecategory-resource-type"></a><span data-ttu-id="1d683-101">Тип ресурса deviceCategory</span><span class="sxs-lookup"><span data-stu-id="1d683-101">deviceCategory resource type</span></span>

> <span data-ttu-id="1d683-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1d683-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d683-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1d683-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="1d683-104">Методы</span><span class="sxs-lookup"><span data-stu-id="1d683-104">Methods</span></span>
|<span data-ttu-id="1d683-105">Метод</span><span class="sxs-lookup"><span data-stu-id="1d683-105">Method</span></span>|<span data-ttu-id="1d683-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1d683-106">Return Type</span></span>|<span data-ttu-id="1d683-107">Описание</span><span class="sxs-lookup"><span data-stu-id="1d683-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1d683-108">Получение объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="1d683-108">Get deviceCategory</span></span>](../api/intune_devices_devicecategory_get.md)|[<span data-ttu-id="1d683-109">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="1d683-109">deviceCategory</span></span>](../resources/intune_devices_devicecategory.md)|<span data-ttu-id="1d683-110">Чтение свойств и связей объекта [deviceCategory](../resources/intune_devices_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="1d683-110">Read properties and relationships of [plannerPlanDetails](../resources/intune_devices_devicecategory.md) object.</span></span>|
|[<span data-ttu-id="1d683-111">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="1d683-111">Update deviceCategory</span></span>](../api/intune_devices_devicecategory_update.md)|[<span data-ttu-id="1d683-112">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="1d683-112">deviceCategory</span></span>](../resources/intune_devices_devicecategory.md)|<span data-ttu-id="1d683-113">Обновление свойств объекта [deviceCategory](../resources/intune_devices_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="1d683-113">Update the properties of a [calendar](../resources/intune_devices_devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1d683-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d683-114">Properties</span></span>
|<span data-ttu-id="1d683-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d683-115">Property</span></span>|<span data-ttu-id="1d683-116">Тип</span><span class="sxs-lookup"><span data-stu-id="1d683-116">Type</span></span>|<span data-ttu-id="1d683-117">Описание</span><span class="sxs-lookup"><span data-stu-id="1d683-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d683-118">id</span><span class="sxs-lookup"><span data-stu-id="1d683-118">id</span></span>|<span data-ttu-id="1d683-119">Строка</span><span class="sxs-lookup"><span data-stu-id="1d683-119">String</span></span>|<span data-ttu-id="1d683-120">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="1d683-120">Unique identifier for the device category.</span></span> <span data-ttu-id="1d683-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d683-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d683-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="1d683-122">Relationships</span></span>
<span data-ttu-id="1d683-123">Нет</span><span class="sxs-lookup"><span data-stu-id="1d683-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1d683-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d683-124">JSON Representation</span></span>
<span data-ttu-id="1d683-125">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d683-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)"
}
```



