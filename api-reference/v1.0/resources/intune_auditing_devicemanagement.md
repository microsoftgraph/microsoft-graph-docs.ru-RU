# <a name="devicemanagement-resource-type"></a><span data-ttu-id="5beb6-101">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="5beb6-101">deviceManagement resource type</span></span>

> <span data-ttu-id="5beb6-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5beb6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5beb6-103">Одноэлементный объект, служащий контейнером для всех функций управления приложениями на устройствах.</span><span class="sxs-lookup"><span data-stu-id="5beb6-103">Singleton entity that acts as a container for all device app management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="5beb6-104">Методы</span><span class="sxs-lookup"><span data-stu-id="5beb6-104">Methods</span></span>
|<span data-ttu-id="5beb6-105">Метод</span><span class="sxs-lookup"><span data-stu-id="5beb6-105">Method</span></span>|<span data-ttu-id="5beb6-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5beb6-106">Return Type</span></span>|<span data-ttu-id="5beb6-107">Описание</span><span class="sxs-lookup"><span data-stu-id="5beb6-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5beb6-108">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="5beb6-108">Get deviceManagement</span></span>](../api/intune_auditing_devicemanagement_get.md)|[<span data-ttu-id="5beb6-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="5beb6-109">deviceManagement</span></span>](../resources/intune_auditing_devicemanagement.md)|<span data-ttu-id="5beb6-110">Чтение свойств и связей объекта [deviceManagement](../resources/intune_auditing_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="5beb6-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_auditing_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="5beb6-111">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="5beb6-111">Update deviceManagement</span></span>](../api/intune_auditing_devicemanagement_update.md)|[<span data-ttu-id="5beb6-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="5beb6-112">deviceManagement</span></span>](../resources/intune_auditing_devicemanagement.md)|<span data-ttu-id="5beb6-113">Обновление свойств объекта [deviceManagement](../resources/intune_auditing_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="5beb6-113">Update the properties of a [calendar](../resources/intune_auditing_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5beb6-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="5beb6-114">Properties</span></span>
|<span data-ttu-id="5beb6-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="5beb6-115">Property</span></span>|<span data-ttu-id="5beb6-116">Тип</span><span class="sxs-lookup"><span data-stu-id="5beb6-116">Type</span></span>|<span data-ttu-id="5beb6-117">Описание</span><span class="sxs-lookup"><span data-stu-id="5beb6-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5beb6-118">id</span><span class="sxs-lookup"><span data-stu-id="5beb6-118">id</span></span>|<span data-ttu-id="5beb6-119">String</span><span class="sxs-lookup"><span data-stu-id="5beb6-119">String</span></span>|<span data-ttu-id="5beb6-120">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5beb6-120">Key of the setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5beb6-121">Связи</span><span class="sxs-lookup"><span data-stu-id="5beb6-121">Relationships</span></span>
|<span data-ttu-id="5beb6-122">Связь</span><span class="sxs-lookup"><span data-stu-id="5beb6-122">Relationship</span></span>|<span data-ttu-id="5beb6-123">Тип</span><span class="sxs-lookup"><span data-stu-id="5beb6-123">Type</span></span>|<span data-ttu-id="5beb6-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5beb6-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5beb6-125">auditEvents</span><span class="sxs-lookup"><span data-stu-id="5beb6-125">auditEvents</span></span>|<span data-ttu-id="5beb6-126">Коллекция [auditEvent](../resources/intune_auditing_auditevent.md)</span><span class="sxs-lookup"><span data-stu-id="5beb6-126">[auditEvent](../resources/intune_auditing_auditevent.md) collection</span></span>|<span data-ttu-id="5beb6-127">События аудита</span><span class="sxs-lookup"><span data-stu-id="5beb6-127">The Audit Events</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5beb6-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5beb6-128">JSON Representation</span></span>
<span data-ttu-id="5beb6-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5beb6-129">Here is a JSON representation of the resource.</span></span>
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



