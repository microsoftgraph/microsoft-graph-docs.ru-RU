# <a name="devicemanagement-resource-type"></a><span data-ttu-id="cd1f1-101">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="cd1f1-101">deviceManagement resource type</span></span>

> <span data-ttu-id="cd1f1-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cd1f1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd1f1-103">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="cd1f1-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="cd1f1-104">Методы</span><span class="sxs-lookup"><span data-stu-id="cd1f1-104">Methods</span></span>
|<span data-ttu-id="cd1f1-105">Метод</span><span class="sxs-lookup"><span data-stu-id="cd1f1-105">Method</span></span>|<span data-ttu-id="cd1f1-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cd1f1-106">Return Type</span></span>|<span data-ttu-id="cd1f1-107">Описание</span><span class="sxs-lookup"><span data-stu-id="cd1f1-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cd1f1-108">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="cd1f1-108">Get deviceManagement</span></span>](../api/intune_tem_devicemanagement_get.md)|[<span data-ttu-id="cd1f1-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="cd1f1-109">deviceManagement</span></span>](../resources/intune_tem_devicemanagement.md)|<span data-ttu-id="cd1f1-110">Чтение свойств и связей объекта [deviceManagement](../resources/intune_tem_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="cd1f1-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_tem_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="cd1f1-111">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="cd1f1-111">Update deviceManagement</span></span>](../api/intune_tem_devicemanagement_update.md)|[<span data-ttu-id="cd1f1-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="cd1f1-112">deviceManagement</span></span>](../resources/intune_tem_devicemanagement.md)|<span data-ttu-id="cd1f1-113">Обновление свойств объекта [deviceManagement](../resources/intune_tem_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="cd1f1-113">Update the properties of a [calendar](../resources/intune_tem_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cd1f1-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd1f1-114">Properties</span></span>
|<span data-ttu-id="cd1f1-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd1f1-115">Property</span></span>|<span data-ttu-id="cd1f1-116">Тип</span><span class="sxs-lookup"><span data-stu-id="cd1f1-116">Type</span></span>|<span data-ttu-id="cd1f1-117">Описание</span><span class="sxs-lookup"><span data-stu-id="cd1f1-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd1f1-118">id</span><span class="sxs-lookup"><span data-stu-id="cd1f1-118">id</span></span>|<span data-ttu-id="cd1f1-119">String</span><span class="sxs-lookup"><span data-stu-id="cd1f1-119">String</span></span>|<span data-ttu-id="cd1f1-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cd1f1-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd1f1-121">Связи</span><span class="sxs-lookup"><span data-stu-id="cd1f1-121">Relationships</span></span>
|<span data-ttu-id="cd1f1-122">Связь</span><span class="sxs-lookup"><span data-stu-id="cd1f1-122">Relationship</span></span>|<span data-ttu-id="cd1f1-123">Тип</span><span class="sxs-lookup"><span data-stu-id="cd1f1-123">Type</span></span>|<span data-ttu-id="cd1f1-124">Описание</span><span class="sxs-lookup"><span data-stu-id="cd1f1-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd1f1-125">telecomExpenseManagementPartners</span><span class="sxs-lookup"><span data-stu-id="cd1f1-125">telecomExpenseManagementPartners</span></span>|<span data-ttu-id="cd1f1-126">Коллекция [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)</span><span class="sxs-lookup"><span data-stu-id="cd1f1-126">[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) collection</span></span>|<span data-ttu-id="cd1f1-127">Партнеры по управлению затратами на телекоммуникации.</span><span class="sxs-lookup"><span data-stu-id="cd1f1-127">The telecom expense management partners.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd1f1-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd1f1-128">JSON Representation</span></span>
<span data-ttu-id="cd1f1-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd1f1-129">Here is a JSON representation of the resource.</span></span>
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



