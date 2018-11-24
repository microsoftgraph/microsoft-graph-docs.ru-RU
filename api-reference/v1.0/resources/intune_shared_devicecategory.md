# <a name="devicecategory-resource-type"></a><span data-ttu-id="7e5d5-101">Тип ресурса deviceCategory</span><span class="sxs-lookup"><span data-stu-id="7e5d5-101">deviceCategory resource type</span></span>

> <span data-ttu-id="7e5d5-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7e5d5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e5d5-103">Категории устройств используются для упорядочивания устройств.</span><span class="sxs-lookup"><span data-stu-id="7e5d5-103">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="7e5d5-104">Используя категории устройств, администраторы могут определить собственные категории, применимые к их организации.</span><span class="sxs-lookup"><span data-stu-id="7e5d5-104">Using device categories, company administrators can define their own categories that make sense to their company.</span></span><span data-ttu-id="7e5d5-105">Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем.</span><span class="sxs-lookup"><span data-stu-id="7e5d5-105"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="7e5d5-106">На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7e5d5-106">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="7e5d5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="7e5d5-107">Methods</span></span>
|<span data-ttu-id="7e5d5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="7e5d5-108">Method</span></span>|<span data-ttu-id="7e5d5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7e5d5-109">Return Type</span></span>|<span data-ttu-id="7e5d5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7e5d5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e5d5-111">[Список deviceCategories](../api/intune_shared_devicecategory_list.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="7e5d5-111">[List deviceCategories](../api/intune_shared_devicecategory_list.md) collection</span></span>|<span data-ttu-id="7e5d5-112">Список свойств и связей объектов [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="7e5d5-112">List properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="7e5d5-113">Получение объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="7e5d5-113">Get deviceCategory</span></span>](../api/intune_shared_devicecategory_get.md)|<span data-ttu-id="7e5d5-114">Чтение свойств и связей объекта [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="7e5d5-114">Read properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>|
|[<span data-ttu-id="7e5d5-115">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="7e5d5-115">Create deviceCategory</span></span>](../api/intune_shared_devicecategory_create.md)|<span data-ttu-id="7e5d5-116">Создание объекта [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="7e5d5-116">Create a new [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>|
|<span data-ttu-id="7e5d5-117">[Удаление deviceCategory](../api/intune_shared_devicecategory_delete.md).</span><span class="sxs-lookup"><span data-stu-id="7e5d5-117">[Delete deviceCategory](../api/intune_shared_devicecategory_delete.md).</span></span>|
|[<span data-ttu-id="7e5d5-118">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="7e5d5-118">Update deviceCategory</span></span>](../api/intune_shared_devicecategory_update.md)|<span data-ttu-id="7e5d5-119">Обновление свойств объекта [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="7e5d5-119">Update the properties of a [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7e5d5-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e5d5-120">Properties</span></span>
|<span data-ttu-id="7e5d5-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e5d5-121">Property</span></span>|<span data-ttu-id="7e5d5-122">Тип</span><span class="sxs-lookup"><span data-stu-id="7e5d5-122">Type</span></span>|<span data-ttu-id="7e5d5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7e5d5-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e5d5-124">id</span><span class="sxs-lookup"><span data-stu-id="7e5d5-124">id</span></span>|<span data-ttu-id="7e5d5-125">String</span><span class="sxs-lookup"><span data-stu-id="7e5d5-125">String</span></span>|<span data-ttu-id="7e5d5-126">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="7e5d5-126">Unique identifier for the device category.</span></span> <span data-ttu-id="7e5d5-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7e5d5-127">Read-only.</span></span>|
|<span data-ttu-id="7e5d5-128">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="7e5d5-128">**Onboarding**</span></span>|
|<span data-ttu-id="7e5d5-129">displayName</span><span class="sxs-lookup"><span data-stu-id="7e5d5-129">displayName</span></span>|<span data-ttu-id="7e5d5-130">String</span><span class="sxs-lookup"><span data-stu-id="7e5d5-130">String</span></span>|<span data-ttu-id="7e5d5-131">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="7e5d5-131">Display name for the device category.</span></span>|
|<span data-ttu-id="7e5d5-132">описание</span><span class="sxs-lookup"><span data-stu-id="7e5d5-132">description</span></span>|<span data-ttu-id="7e5d5-133">String</span><span class="sxs-lookup"><span data-stu-id="7e5d5-133">String</span></span>|<span data-ttu-id="7e5d5-134">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="7e5d5-134">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e5d5-135">Связи</span><span class="sxs-lookup"><span data-stu-id="7e5d5-135">Relationships</span></span>
<span data-ttu-id="7e5d5-136">None</span><span class="sxs-lookup"><span data-stu-id="7e5d5-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e5d5-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e5d5-137">JSON Representation</span></span>
<span data-ttu-id="7e5d5-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e5d5-138">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



