# <a name="devicemanagement-resource-type"></a><span data-ttu-id="28d3b-101">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="28d3b-101">deviceManagement resource type</span></span>

> <span data-ttu-id="28d3b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="28d3b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28d3b-103">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="28d3b-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="28d3b-104">Методы</span><span class="sxs-lookup"><span data-stu-id="28d3b-104">Methods</span></span>
|<span data-ttu-id="28d3b-105">Метод</span><span class="sxs-lookup"><span data-stu-id="28d3b-105">Method</span></span>|<span data-ttu-id="28d3b-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="28d3b-106">Return Type</span></span>|<span data-ttu-id="28d3b-107">Описание</span><span class="sxs-lookup"><span data-stu-id="28d3b-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="28d3b-108">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="28d3b-108">Get deviceManagement</span></span>](../api/intune_endpointprotection_devicemanagement_get.md)|[<span data-ttu-id="28d3b-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="28d3b-109">deviceManagement</span></span>](../resources/intune_endpointprotection_devicemanagement.md)|<span data-ttu-id="28d3b-110">Чтение свойств и связей объекта [deviceManagement](../resources/intune_endpointprotection_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="28d3b-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_endpointprotection_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="28d3b-111">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="28d3b-111">Update deviceManagement</span></span>](../api/intune_endpointprotection_devicemanagement_update.md)|[<span data-ttu-id="28d3b-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="28d3b-112">deviceManagement</span></span>](../resources/intune_endpointprotection_devicemanagement.md)|<span data-ttu-id="28d3b-113">Обновление свойств объекта [deviceManagement](../resources/intune_endpointprotection_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="28d3b-113">Update the properties of a [calendar](../resources/intune_endpointprotection_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="28d3b-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="28d3b-114">Properties</span></span>
|<span data-ttu-id="28d3b-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="28d3b-115">Property</span></span>|<span data-ttu-id="28d3b-116">Тип</span><span class="sxs-lookup"><span data-stu-id="28d3b-116">Type</span></span>|<span data-ttu-id="28d3b-117">Описание</span><span class="sxs-lookup"><span data-stu-id="28d3b-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28d3b-118">id</span><span class="sxs-lookup"><span data-stu-id="28d3b-118">id</span></span>|<span data-ttu-id="28d3b-119">Строка</span><span class="sxs-lookup"><span data-stu-id="28d3b-119">String</span></span>|<span data-ttu-id="28d3b-120">Уникальный идентификатор</span><span class="sxs-lookup"><span data-stu-id="28d3b-120">Unique Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="28d3b-121">Связи</span><span class="sxs-lookup"><span data-stu-id="28d3b-121">Relationships</span></span>
<span data-ttu-id="28d3b-122">Нет</span><span class="sxs-lookup"><span data-stu-id="28d3b-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="28d3b-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28d3b-123">JSON Representation</span></span>
<span data-ttu-id="28d3b-124">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28d3b-124">Here is a JSON representation of the resource.</span></span>
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



