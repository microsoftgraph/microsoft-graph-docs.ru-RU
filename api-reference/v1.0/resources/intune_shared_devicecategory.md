# <a name="devicecategory-resource-type"></a><span data-ttu-id="1eb3e-101">Тип ресурса deviceCategory</span><span class="sxs-lookup"><span data-stu-id="1eb3e-101">deviceCategory resource type</span></span>

> <span data-ttu-id="1eb3e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1eb3e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1eb3e-103">Категории устройств используются для упорядочивания устройств.</span><span class="sxs-lookup"><span data-stu-id="1eb3e-103">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="1eb3e-104">Используя категории устройств, администраторы могут определить собственные категории, применимые к их организации.</span><span class="sxs-lookup"><span data-stu-id="1eb3e-104">Using device categories, company administrators can define their own categories that make sense to their company.</span></span> <span data-ttu-id="1eb3e-105">Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем.</span><span class="sxs-lookup"><span data-stu-id="1eb3e-105">These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="1eb3e-106">На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1eb3e-106">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="1eb3e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="1eb3e-107">Methods</span></span>
|<span data-ttu-id="1eb3e-108">Метод</span><span class="sxs-lookup"><span data-stu-id="1eb3e-108">Method</span></span>|<span data-ttu-id="1eb3e-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1eb3e-109">Return Type</span></span>|<span data-ttu-id="1eb3e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1eb3e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1eb3e-111">[Список объектов deviceCategories](../api/intune_shared_devicecategory_list.md)</span><span class="sxs-lookup"><span data-stu-id="1eb3e-111">[List deviceCategories](../api/intune_shared_devicecategory_list.md) objects.</span></span>|
|<span data-ttu-id="1eb3e-112">[Получение объекта deviceCategory](../api/intune_shared_devicecategory_get.md)</span><span class="sxs-lookup"><span data-stu-id="1eb3e-112">[Get deviceCategory](../api/intune_shared_devicecategory_get.md) object.</span></span>|
|<span data-ttu-id="1eb3e-113">[Создание объекта deviceCategory](../api/intune_shared_devicecategory_create.md)</span><span class="sxs-lookup"><span data-stu-id="1eb3e-113">Create a new [deviceCategory](../api/intune_shared_devicecategory_create.md) object.</span></span>|
|<span data-ttu-id="1eb3e-114">[Удаление объекта deviceCategory](../api/intune_shared_devicecategory_delete.md)</span><span class="sxs-lookup"><span data-stu-id="1eb3e-114">Delete deviceCategory</span></span>|
|<span data-ttu-id="1eb3e-115">[Обновление объекта deviceCategory](../api/intune_shared_devicecategory_update.md)</span><span class="sxs-lookup"><span data-stu-id="1eb3e-115">Update the properties of a [deviceCategory](../api/intune_shared_devicecategory_update.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1eb3e-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="1eb3e-116">Properties</span></span>
|<span data-ttu-id="1eb3e-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="1eb3e-117">Property</span></span>|<span data-ttu-id="1eb3e-118">Тип</span><span class="sxs-lookup"><span data-stu-id="1eb3e-118">Type</span></span>|<span data-ttu-id="1eb3e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1eb3e-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1eb3e-120">id</span><span class="sxs-lookup"><span data-stu-id="1eb3e-120">id</span></span>|<span data-ttu-id="1eb3e-121">String</span><span class="sxs-lookup"><span data-stu-id="1eb3e-121">String</span></span>|<span data-ttu-id="1eb3e-122">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="1eb3e-122">Unique identifier for the device category.</span></span> <span data-ttu-id="1eb3e-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1eb3e-123">Read-only.</span></span>|
|<span data-ttu-id="1eb3e-124">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="1eb3e-124">**On-boarding**</span></span>|
|<span data-ttu-id="1eb3e-125">displayName</span><span class="sxs-lookup"><span data-stu-id="1eb3e-125">displayName</span></span>|<span data-ttu-id="1eb3e-126">String</span><span class="sxs-lookup"><span data-stu-id="1eb3e-126">String</span></span>|<span data-ttu-id="1eb3e-127">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="1eb3e-127">Display name for the device category.</span></span>|
|<span data-ttu-id="1eb3e-128">description</span><span class="sxs-lookup"><span data-stu-id="1eb3e-128">description</span></span>|<span data-ttu-id="1eb3e-129">String</span><span class="sxs-lookup"><span data-stu-id="1eb3e-129">String</span></span>|<span data-ttu-id="1eb3e-130">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="1eb3e-130">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1eb3e-131">Связи</span><span class="sxs-lookup"><span data-stu-id="1eb3e-131">Relationships</span></span>
<span data-ttu-id="1eb3e-132">Нет</span><span class="sxs-lookup"><span data-stu-id="1eb3e-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1eb3e-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1eb3e-133">JSON Representation</span></span>
<span data-ttu-id="1eb3e-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1eb3e-134">Here is a JSON representation of the resource.</span></span>
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



