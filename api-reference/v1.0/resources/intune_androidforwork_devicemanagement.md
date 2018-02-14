# <a name="devicemanagement-resource-type"></a><span data-ttu-id="63399-101">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="63399-101">deviceManagement resource type</span></span>

> <span data-ttu-id="63399-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="63399-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63399-103">Одноэлементный объект, служащий контейнером для функций параметров Android for Work в управлении устройства.</span><span class="sxs-lookup"><span data-stu-id="63399-103">Singleton entity that acts as a container for Android for Work settings functionality under device management.</span></span>
## <a name="methods"></a><span data-ttu-id="63399-104">Методы</span><span class="sxs-lookup"><span data-stu-id="63399-104">Methods</span></span>
|<span data-ttu-id="63399-105">Метод</span><span class="sxs-lookup"><span data-stu-id="63399-105">Method</span></span>|<span data-ttu-id="63399-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="63399-106">Return Type</span></span>|<span data-ttu-id="63399-107">Описание</span><span class="sxs-lookup"><span data-stu-id="63399-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="63399-108">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="63399-108">Get deviceManagement</span></span>](../api/intune_androidforwork_devicemanagement_get.md)|[<span data-ttu-id="63399-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="63399-109">deviceManagement</span></span>](../resources/intune_androidforwork_devicemanagement.md)|<span data-ttu-id="63399-110">Чтение свойств и связей объекта [deviceManagement](../resources/intune_androidforwork_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="63399-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_androidforwork_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="63399-111">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="63399-111">Update deviceManagement</span></span>](../api/intune_androidforwork_devicemanagement_update.md)|[<span data-ttu-id="63399-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="63399-112">deviceManagement</span></span>](../resources/intune_androidforwork_devicemanagement.md)|<span data-ttu-id="63399-113">Обновление свойств объекта [deviceManagement](../resources/intune_androidforwork_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="63399-113">Update the properties of a [calendar](../resources/intune_androidforwork_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="63399-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="63399-114">Properties</span></span>
|<span data-ttu-id="63399-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="63399-115">Property</span></span>|<span data-ttu-id="63399-116">Тип</span><span class="sxs-lookup"><span data-stu-id="63399-116">Type</span></span>|<span data-ttu-id="63399-117">Описание</span><span class="sxs-lookup"><span data-stu-id="63399-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63399-118">id</span><span class="sxs-lookup"><span data-stu-id="63399-118">id</span></span>|<span data-ttu-id="63399-119">String</span><span class="sxs-lookup"><span data-stu-id="63399-119">String</span></span>|<span data-ttu-id="63399-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="63399-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="63399-121">Связи</span><span class="sxs-lookup"><span data-stu-id="63399-121">Relationships</span></span>
|<span data-ttu-id="63399-122">Связь</span><span class="sxs-lookup"><span data-stu-id="63399-122">Relationship</span></span>|<span data-ttu-id="63399-123">Тип</span><span class="sxs-lookup"><span data-stu-id="63399-123">Type</span></span>|<span data-ttu-id="63399-124">Описание</span><span class="sxs-lookup"><span data-stu-id="63399-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63399-125">androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="63399-125">androidForWorkSettings</span></span>|[<span data-ttu-id="63399-126">androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="63399-126">androidForWorkSettings</span></span>](../resources/intune_androidforwork_androidforworksettings.md)|<span data-ttu-id="63399-127">Одноэлементная сущность параметров Android for Work.</span><span class="sxs-lookup"><span data-stu-id="63399-127">The singleton Android for Work settings entity.</span></span>|
|<span data-ttu-id="63399-128">androidForWorkAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="63399-128">androidForWorkAppConfigurationSchemas</span></span>|<span data-ttu-id="63399-129">Коллекция [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md)</span><span class="sxs-lookup"><span data-stu-id="63399-129">[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) collection</span></span>|<span data-ttu-id="63399-130">Сущности схемы конфигурации в приложении Android for Work.</span><span class="sxs-lookup"><span data-stu-id="63399-130">Android for Work app configuration schema entities.</span></span>|
|<span data-ttu-id="63399-131">androidForWorkEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="63399-131">androidForWorkEnrollmentProfiles</span></span>|<span data-ttu-id="63399-132">Коллекция [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="63399-132">[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) collection</span></span>|<span data-ttu-id="63399-133">Сущности профиля регистрации Android for Work.</span><span class="sxs-lookup"><span data-stu-id="63399-133">Android for Work enrollment profile entities.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="63399-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="63399-134">JSON Representation</span></span>
<span data-ttu-id="63399-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63399-135">Here is a JSON representation of the resource.</span></span>
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



