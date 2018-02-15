# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="a43b9-101">Тип ресурса deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a43b9-101">deviceAppManagement resource type</span></span>

> <span data-ttu-id="a43b9-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a43b9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a43b9-103">Одноэлементный объект, служащий контейнером для всех функций управления приложениями на устройствах.</span><span class="sxs-lookup"><span data-stu-id="a43b9-103">Singleton entity that acts as a container for all device app management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="a43b9-104">Методы</span><span class="sxs-lookup"><span data-stu-id="a43b9-104">Methods</span></span>
|<span data-ttu-id="a43b9-105">Метод</span><span class="sxs-lookup"><span data-stu-id="a43b9-105">Method</span></span>|<span data-ttu-id="a43b9-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a43b9-106">Return Type</span></span>|<span data-ttu-id="a43b9-107">Описание</span><span class="sxs-lookup"><span data-stu-id="a43b9-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a43b9-108">Получение объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a43b9-108">Get deviceAppManagement</span></span>](../api/intune_books_deviceappmanagement_get.md)|[<span data-ttu-id="a43b9-109">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a43b9-109">deviceAppManagement</span></span>](../resources/intune_books_deviceappmanagement.md)|<span data-ttu-id="a43b9-110">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune_books_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="a43b9-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_books_deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="a43b9-111">Обновление объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a43b9-111">Update deviceAppManagement</span></span>](../api/intune_books_deviceappmanagement_update.md)|[<span data-ttu-id="a43b9-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a43b9-112">deviceAppManagement</span></span>](../resources/intune_books_deviceappmanagement.md)|<span data-ttu-id="a43b9-113">Обновление свойств объекта [deviceAppManagement](../resources/intune_books_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="a43b9-113">Update the properties of a [calendar](../resources/intune_books_deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a43b9-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="a43b9-114">Properties</span></span>
|<span data-ttu-id="a43b9-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="a43b9-115">Property</span></span>|<span data-ttu-id="a43b9-116">Тип</span><span class="sxs-lookup"><span data-stu-id="a43b9-116">Type</span></span>|<span data-ttu-id="a43b9-117">Описание</span><span class="sxs-lookup"><span data-stu-id="a43b9-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a43b9-118">id</span><span class="sxs-lookup"><span data-stu-id="a43b9-118">id</span></span>|<span data-ttu-id="a43b9-119">String</span><span class="sxs-lookup"><span data-stu-id="a43b9-119">String</span></span>|<span data-ttu-id="a43b9-120">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a43b9-120">Key of the setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a43b9-121">Связи</span><span class="sxs-lookup"><span data-stu-id="a43b9-121">Relationships</span></span>
|<span data-ttu-id="a43b9-122">Связь</span><span class="sxs-lookup"><span data-stu-id="a43b9-122">Relationship</span></span>|<span data-ttu-id="a43b9-123">Тип</span><span class="sxs-lookup"><span data-stu-id="a43b9-123">Type</span></span>|<span data-ttu-id="a43b9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a43b9-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a43b9-125">managedEBooks</span><span class="sxs-lookup"><span data-stu-id="a43b9-125">managedEBooks</span></span>|<span data-ttu-id="a43b9-126">Коллекция [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="a43b9-126">[managedEBook](../resources/intune_books_managedebook.md) collection</span></span>|<span data-ttu-id="a43b9-127">Управляемая электронная книга.</span><span class="sxs-lookup"><span data-stu-id="a43b9-127">The Managed eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a43b9-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a43b9-128">JSON Representation</span></span>
<span data-ttu-id="a43b9-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a43b9-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```



