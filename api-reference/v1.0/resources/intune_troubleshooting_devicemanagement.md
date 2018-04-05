# <a name="devicemanagement-resource-type"></a><span data-ttu-id="6c92b-101">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="6c92b-101">deviceManagement resource type</span></span>

> <span data-ttu-id="6c92b-102">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6c92b-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c92b-103">Использование этих API в рабочих приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c92b-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c92b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6c92b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c92b-105">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="6c92b-105">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="6c92b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="6c92b-106">Methods</span></span>
|<span data-ttu-id="6c92b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="6c92b-107">Method</span></span>|<span data-ttu-id="6c92b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6c92b-108">Return Type</span></span>|<span data-ttu-id="6c92b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6c92b-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6c92b-110">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="6c92b-110">Get deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_get.md)|[<span data-ttu-id="6c92b-111">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="6c92b-111">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="6c92b-112">Чтение свойств и связей объекта [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="6c92b-112">Read properties and relationships of the [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="6c92b-113">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="6c92b-113">Update deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_update.md)|[<span data-ttu-id="6c92b-114">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="6c92b-114">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="6c92b-115">Обновление свойств объекта [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="6c92b-115">Update the properties of a [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c92b-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c92b-116">Properties</span></span>
|<span data-ttu-id="6c92b-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c92b-117">Property</span></span>|<span data-ttu-id="6c92b-118">Тип</span><span class="sxs-lookup"><span data-stu-id="6c92b-118">Type</span></span>|<span data-ttu-id="6c92b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6c92b-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c92b-120">id</span><span class="sxs-lookup"><span data-stu-id="6c92b-120">id</span></span>|<span data-ttu-id="6c92b-121">String</span><span class="sxs-lookup"><span data-stu-id="6c92b-121">String</span></span>|<span data-ttu-id="6c92b-122">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6c92b-122">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c92b-123">Связи</span><span class="sxs-lookup"><span data-stu-id="6c92b-123">Relationships</span></span>
|<span data-ttu-id="6c92b-124">Связь</span><span class="sxs-lookup"><span data-stu-id="6c92b-124">Relationship</span></span>|<span data-ttu-id="6c92b-125">Тип</span><span class="sxs-lookup"><span data-stu-id="6c92b-125">Type</span></span>|<span data-ttu-id="6c92b-126">Описание</span><span class="sxs-lookup"><span data-stu-id="6c92b-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c92b-127">troubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="6c92b-127">troubleshootingEvents</span></span>|<span data-ttu-id="6c92b-128">Коллекция [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="6c92b-128">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="6c92b-129">Список событий устранения неполадок для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c92b-129">The list of troubleshooting events for the tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c92b-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6c92b-130">JSON Representation</span></span>
<span data-ttu-id="6c92b-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c92b-131">Here is a JSON representation of the resource.</span></span>
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



