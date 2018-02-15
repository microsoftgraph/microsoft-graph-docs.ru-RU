# <a name="devicemanagement-resource-type"></a><span data-ttu-id="c8118-101">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c8118-101">deviceManagement resource type</span></span>

> <span data-ttu-id="c8118-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c8118-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8118-103">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="c8118-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="c8118-104">Методы</span><span class="sxs-lookup"><span data-stu-id="c8118-104">Methods</span></span>
|<span data-ttu-id="c8118-105">Метод</span><span class="sxs-lookup"><span data-stu-id="c8118-105">Method</span></span>|<span data-ttu-id="c8118-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c8118-106">Return Type</span></span>|<span data-ttu-id="c8118-107">Описание</span><span class="sxs-lookup"><span data-stu-id="c8118-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c8118-108">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c8118-108">Get deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_get.md)|[<span data-ttu-id="c8118-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c8118-109">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="c8118-110">Чтение свойств и связей объекта [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="c8118-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="c8118-111">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c8118-111">Update deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_update.md)|[<span data-ttu-id="c8118-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c8118-112">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="c8118-113">Обновление свойств объекта [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="c8118-113">Update the properties of a [calendar](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c8118-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8118-114">Properties</span></span>
|<span data-ttu-id="c8118-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8118-115">Property</span></span>|<span data-ttu-id="c8118-116">Тип</span><span class="sxs-lookup"><span data-stu-id="c8118-116">Type</span></span>|<span data-ttu-id="c8118-117">Описание</span><span class="sxs-lookup"><span data-stu-id="c8118-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8118-118">id</span><span class="sxs-lookup"><span data-stu-id="c8118-118">id</span></span>|<span data-ttu-id="c8118-119">String</span><span class="sxs-lookup"><span data-stu-id="c8118-119">String</span></span>|<span data-ttu-id="c8118-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c8118-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8118-121">Связи</span><span class="sxs-lookup"><span data-stu-id="c8118-121">Relationships</span></span>
|<span data-ttu-id="c8118-122">Связь</span><span class="sxs-lookup"><span data-stu-id="c8118-122">Relationship</span></span>|<span data-ttu-id="c8118-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c8118-123">Type</span></span>|<span data-ttu-id="c8118-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c8118-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8118-125">troubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="c8118-125">troubleshootingEvents</span></span>|<span data-ttu-id="c8118-126">Коллекция [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c8118-126">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="c8118-127">Список событий устранения неполадок для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8118-127">The list of troubleshooting events for the tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c8118-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c8118-128">JSON Representation</span></span>
<span data-ttu-id="c8118-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8118-129">Here is a JSON representation of the resource.</span></span>
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



